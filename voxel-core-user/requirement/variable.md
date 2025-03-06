# Variable

Variable Requirement takes a variable as the matching against required value

## Fields
`variable`: [Global Variable](../global-variables)  
`required`: [Value Provider](../value-provider/constant.md)

## Example
```yml
requirement: !variable
  variable: "currency_money"
  required: "1k"
  
  display:
    met: "<green>1K moneyz"
    not_met: "<red>1K money"
```