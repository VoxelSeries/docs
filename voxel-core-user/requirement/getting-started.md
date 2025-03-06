---
order: 0
---

# Getting Started

Requirements in `VoxelSeries` is the core component for creating in-depth economies.

Every `module` defines requirement types most of them are defined at `code-time` whilst some are defined from `configs`.

## Optional Fields
`display ->`  
`pass`: [Text](../config-types#text) - displays whenever the requirement is met  
`fail`: [Text](../config-types#text) - displays whenever the requirement failed  
`simple`: [Text](../config-types#text) - displays whenever the requirement has not been tested  

In the displays of `pass` and `fail` you can use variables defined by the requirement types