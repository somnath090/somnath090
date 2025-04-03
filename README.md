As a developer, 

I want to remove the Contract Executed field in HDS 

so that it does not show incorrect information on the UI.

Context:

The Contract Executed field in HDS is currently for display only. It does not update when a property becomes active, leading to incorrect information being displayed. The field is not utilized by any downstream applications, so its removal will not cause any issues.

Other information

Spike finding: SPIKE: Hotel Suite: Review and Update of "Contract Executed" Field in HDS (RND-18216)

Hotel Legal checks the franchiseStatus from the RSS prop_info_rss table to determine the value of contractExecuted.

The field is only updated when a property is “New” or “Terminated”.

The field is not sent to Edge, RSS, DAP, or SalesForce, indicating no downstream impact.

Hotel Legal checks if the franchiseStatus (from RSS prop_info_rss table) is not blank and not equal to “N”.

If both conditions are true, it sets contractExecuted to false.

Otherwise, it sets contractExecuted to true.

However, since Hotel Legal performs partial updates for properties that are “Inactive”, “Active”, or “Suspended”, the “contractExecuted” field is only set or updated when a property is “New” or “Terminated”. As a result, once a property becomes “Inactive”, this field retains the value assigned when the property was “New” and will only be updated again when the property is terminated.

 Downstream impact:

Edge: HDS adapter is not sending this field to Edge, therefore no impact

RSS: HCS-RSS-CONSUMER is not sending this field to RSS, therefore no impact

DAP: HCS sends the HDS hotel event without the “configuration” object, which contains “contractExecuted”, therefore no impact.

SalesForce: HCS sends the HDS hotel event without the “configuration” object, which contains “contractExecuted”, therefore no impact.

Conclusion:

Since this field is not utilized by any downstream services and appears to be only for display on the HDS UI, its removal will not cause any issues.

We could also include this field in the partial update list.
