---
order: 3
---
# Composite

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
      fail: "<red>No Admin"
      pass: "<green>Yes Admin"
      simple: "<green>Admin Permission"
```

This config would produce an output if displayed in lore if the user has enough money and admin perm:
```
| 100k Money
| Yes Admin
```

## Defaults config
Located in `VoxelSeries/config.yml -> requirement_display -> composite`
```yml
display:
  join_with: "|"
```