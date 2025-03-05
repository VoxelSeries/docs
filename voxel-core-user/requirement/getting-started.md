# Getting Started

Requirements in `VoxelSeries` is the core component for creating in-depth economies.

Every `module` defines requirement types most of them are defined at `code-time` whilst some are defined from `configs`.

## Takeable
Some requirements are `takeable` which means they can be withdrawn from the user  
If the requirement is takeable, you can ensure it takes whilst defining a requirement
```js
requirement: !currency_money
  amount: 1000
  take: true //[!code focus]
```

## Composite
You can combine requirements together
```yml
requirement: !composite
  display:
    join_with: "|"
  list:
  - !variable
    variable: "currency_money"
    requirement: "100k"
  - !permission
    permission: "voxelseries.admin"
    display:
      not_met: "<red>No Admin"
      met: "<green>Yes Admin"
```

This config would produce an output if displayed in lore if the user has enough money and admin perm:
```
| 100k Money
| Yes Admin
```