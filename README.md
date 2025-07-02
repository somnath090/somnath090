All phone fields in HDS UI deliver an Error message id: 1004 when the user adds a character/number in the International Dialing Code field.

Because the error message appears the interface is allowed to save any wrong data added to the International Dialing Code field.

The expected behavior for this field is that the user receives a US code suggestion when It writes any character/number. It only accepts US code when the user adds “US“ or “01“. 

If the user adds a different character or number than expected, the field deletes the value as soon the user clicks on a new field or different section on the screen. 
