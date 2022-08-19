<!-- default badges list -->
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T1106516)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->

# Grid for Blazor - How to implement filter operator selector

This example demonstrates how to implement a custom filter row to provide users with operator selector.

In each grid column, the [FilterRowCellTemplate](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn.FilterRowCellTemplate) property specifies a template for the filter row cell. The template contains the **OperatorType** component (see the [OperatorType.razor](./CS/DxGridFilterOperatorSelector/Components/OperatorType.razor) file). The component includes the DxButton that opens a dropdown window with a list of operators. When a user selects an operator, the column's [FilterRowOperatorType](http://docs.devexpress.devx/Blazor/DevExpress.Blazor.DxGridDataColumn.FilterRowOperatorType) property is set to the specified value and the column values are filtered.

![Grid with filter](image.png)

## Files to Look At

- [Grid.razor](./CS/DxGridFilterOperatorSelector/Pages/Grid.razor)
- [OperatorType.razor](./CS/DxGridFilterOperatorSelector/Components/OperatorType.razor)
