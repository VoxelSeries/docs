# Permission 
::: warning
Permission value provider can only be used whilst `LuckPerms` is present
:::

Permission value provider can be used to compute the value based on their permission value

### Example
This provides the `max_balance` found by the maximum value of permissions starting with `currency.maxbalance.` defaulting to `1k` if no permissions are found
```yml
  max_balance: !permission
    permission: "currency.maxbalance."
    default: "1k"
```