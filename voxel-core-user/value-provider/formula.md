# Formula

Formula value provider can be used to compute a value based on global variables or provided ones.

### Example
A formula that computed `max_balance` based on their current `rank`
```yml
!formula "max(leveling_rank * 2, 10000)"
```