---
order: 1
---
# Takeable

Some requirements are `takeable` which means they can be withdrawn from the user  
If the requirement is takeable, you can ensure it takes whilst defining a requirement

```js
requirement: !currency_money
  amount: 1000
  take: true //[!code focus]
```