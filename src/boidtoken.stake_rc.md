# Action - `{{ stake }}`

This Contract is legally binding and can be used in the event of a dispute. Disputes shall be settled through the standard arbitration process established by EOS.IO.

### Description

The `{{ stake }}` action... 

INTENT: The intent of `{{ stake }}` is to allow users to move token awards from escrow to the staked token storage in the stakes table and to update the users next period stake amount. The users next payout is based on the additional tokens deposited by the system this action also serves to demark the line when the tokens move under user ownership and no longer subject to forfeiture for early withdrawal from the stake period. User participation is required for this action due to the BP-imposed timeout for transactions over 250ms, which will not allow a contract-driven global claim function to be fully executed when over 100 users have staked to the system.

TERM: This action lasts for the duration of the processing of the contract.

### Inputs and Input Types

The `{{ stake }}` action requires the following `inputs` and `input types`:

| Action | Input | Input Type |
|:--|:--|:--|
| `{{ claim }}` | `{{ _stake_account }}`<br/>`{{ _stake_period }}`<br/>`{{ _staked }}` | `{{ name }}`<br/>`{{ uint8_t }}`<br/>`{{ asset }}` |