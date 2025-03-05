---
order: 3
---

# Config Types

Whilst other plugins might prefer to use types as fields, we've decided to use the feature of `yml tags` to define types of our objects in configs.

### Example
Whilst a normal config would look like this:
```yml
  max_balance:
    # The type of registered value provider
    type: "permission"
    permission: "currency.maxbalance."
    default: "1k"
```

What our config looks like:
```yml
  max_balance: !permission
    permission: "currency.maxbalance."
    default: "1k"
```