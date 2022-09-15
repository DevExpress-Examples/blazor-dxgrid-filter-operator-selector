<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/520108155/21.2.3%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T1106516)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->

# Grid for Blazor - Incorporate a selector for filter row operator type

This example demonstrates how you can extend our Blazor Grid’s Filter Row with a custom operator selector.

Within each grid column, the [FilterRowCellTemplate](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn.FilterRowCellTemplate) property specifies the template used for the filter row cell. The template contains an **OperatorType** component (see the [OperatorType.razor](./CS/DxGridFilterOperatorSelector/Components/OperatorType.razor) file). The component includes a DxButton that activates a dropdown window with a list of operators. When a user selects an operator, the column's [FilterRowOperatorType](http://docs.devexpress.devx/Blazor/DevExpress.Blazor.DxGridDataColumn.FilterRowOperatorType) property is set to the specified value and the column values are filtered.

![Grid with filter](image.png)

## Files to Review

- [Grid.razor](./CS/DxGridFilterOperatorSelector/Pages/Grid.razor)
- [OperatorType.razor](./CS/DxGridFilterOperatorSelector/Components/OperatorType.razor)
