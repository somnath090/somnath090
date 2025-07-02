An error is currently being generated in Prop-EL at property MX241 when attempting to add an NDD room type with a decimal value in the "Total Area" field. The issue seems related to how Hotel Suite (HDS) handles the totalArea field — currently, it does not support decimal values.

Temporary workaround: Rounding the value or leaving the field empty allows the entry to succeed.

We need to determine:

Whether the totalArea field in Hotel Suite (HDS) can safely support decimal values without affecting downstream systems or integrations.

If downstream systems can accept decimal values, we can consider updating the backend to support it.

If decimal support cannot be added, we should update the Prop-EL UI to restrict users from entering decimal values in the Total Area field.

Scope of Investigation:

Review HDS schema – confirm current handling of totalArea values.

Trace downstream usage of the totalArea field:

Validate whether any external or internal systems consume this field and whether they allow decimals.

Identify any transformation or validation logic that could break.

Assess potential frontend impact in Prop-EL if decimals are allowed vs. disallowed.

Summarize the implications and recommend the best course of action.

