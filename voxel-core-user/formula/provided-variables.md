# Provided Variables

Some formula definitions will define a provided variable. Let's take a look how you can use them
Let's take an example of a dynamic requirement.
```yml
requirement: !variable
  variable: "currency_money"
  # Here we take the "value" as the provided variable
  requirement: "[value] > 1000"
```

As you can see the provided variables can be used by wrapping them in brackets `[variable]`