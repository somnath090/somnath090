Description

HCS errors were updated to include invalid master room type. This error now includes object trace. This is cosmetically undesirable, and the error should not have the object trace included. 
Acceptance Criteria

HCS master room type error message is sent in the response without the object trace.
Steps to Reproduce


Call HCS update with invalid room type code. 
