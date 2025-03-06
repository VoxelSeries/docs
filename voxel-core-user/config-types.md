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

### Numbers
Every number can be defined in a form of just a number, or a number with abbreviations  
So these are valid definitions:
- `1`
- `1k`
- `1.2k`

Abbreviations supported (case insensitive):
- K - thousand
- M - million
- B - billion
- T - trillion
- Qa - quadrillion
- Q - quintillion

### Time
Time can be defined in this format `[amount][s,h,d]...`

### Text
A text is a colored text that the player will see  
The format of the text is defined in [Mini Message](https://docs.advntr.dev/minimessage/format)  

::: tip
You can play around with the text before using it in [Mini Message Web Editor](https://webui.advntr.dev/)
:::