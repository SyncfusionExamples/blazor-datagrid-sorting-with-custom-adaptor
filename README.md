# Blazor DataGrid - Sorting with Custom Adaptor

A comprehensive example demonstrating how to implement custom sorting operations in the [Blazor DataGrid](https://www.syncfusion.com/blazor-components/blazor-datagrid) component using a custom data adaptor.

## Overview

This project showcases best practices for working with the [Blazor DataGrid](https://www.syncfusion.com/blazor-components/blazor-datagrid) component. It provides a practical example of:

- Implementing a **custom data adaptor** that extends the `DataAdaptor` class
- Performing **server-side sorting** operations on your data
- Handling **pagination** alongside sorting
- Building a real-world data scenario with sample order data

The sample uses a `CustomAdaptor` to intercept and process DataGrid requests, allowing you to implement custom business logic for sorting and pagination operations.

## Features

- **Custom Data Adaptor**: Full implementation of a custom adaptor that handles Read operations
- **Server-Side Sorting**: Demonstrates how to apply sorting logic using `DataOperations.PerformSorting`
- **Pagination Support**: Implements paging functionality with `Skip`, `Take` operations
- **Interactive DataGrid**: A responsive grid displaying Order data with sortable columns

## Prerequisites

* [.NET SDK 10.0](https://dotnet.microsoft.com/en-us/download/dotnet/10.0) or later
* [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or later
* [Visual Studio Code](https://code.visualstudio.com/)

## Getting Started

### Clone the repository

```bash
git clone https://github.com/SyncfusionExamples/blazor-datagrid-sorting-with-custom-adaptor.git
cd blazor-datagrid-sorting-with-custom-adaptor
```

### Run with Visual Studio

1. Open the solution file using Visual Studio 2022 or later.
2. Restore the NuGet packages by rebuilding the solution.
3. Build the project to ensure there are no compilation errors.
4. Run the project.

### Run with .NET CLI

```bash
# Restore dependencies
dotnet restore

# Run the project
dotnet run
```
## References

**Documentation**: https://blazor.syncfusion.com/documentation/smith-chart/getting-started-webapp

**Online examples**: https://blazor.syncfusion.com/demos/smith-chart/default-functionalities?theme=fluent2