Default Behavior:

SGM and LSTATE rate plans should continue to default as Opted In (checked) with Rate Plan Type = Flat Amount

Updated Behavior on Dropdown Change:

If the Rate Plan Type is changed from Flat Amount to Percent off BAR, the Opt-In checkbox should remain checked.

Explicit User Action:

The Opt-In checkbox should only be unchecked if and only if the user manually clicks on the checkbox to deselect it.

Ensure this logic applies only to SGM and LSTATE rate plans in the Other Rate Plans section.

Testing should confirm that no regression occurs in the default selection or saving behavior of rate plans.
