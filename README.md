# Blazor DataGrid - Sorting with Custom Adaptor

## Overview

This sample demonstrates how to perform sorting operations in the Syncfusion Blazor DataGrid while using a custom data adaptor. Instead of relying on a built-in data source, the DataGrid uses an `SfDataManager` configured with a custom adaptor that extends the `DataAdaptor` class. The sample shows how DataGrid sorting requests can be processed manually inside the adaptor by handling sort actions within the overridden `Read` method. This approach is useful when data must be processed through custom business logic, external services, or non-standard data sources while still supporting the built-in DataGrid sorting experience.

## Key Features

- Uses the Syncfusion `SfGrid` component with sorting enabled.
- Configures data binding through `SfDataManager`.
- Uses `Adaptor="Adaptors.CustomAdaptor"` and `AdaptorInstance="@typeof(CustomAdaptor)"`.
- Implements a custom data adaptor by extending the `DataAdaptor` class.
- Processes DataGrid requests inside the overridden `Read(DataManagerRequest dm, string key = null)` method.
- Demonstrates custom sorting logic executed through Syncfusion data processing operations.
- Supports paging together with sorting through the same custom adaptor implementation.

## Prerequisites

- Visual Studio 2022 or Visual Studio Code
- .NET SDK compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download the repository.
2. Open the solution file `SortingWithCustomAdaptor.sln`. `[VERIFY: solution name if repository structure differs]`
3. Restore all NuGet packages.
4. Set the `SortingWithCustomAdaptor` project as the startup project if required.
5. Build the solution.
6. Run the project using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open the integrated terminal.
3. Navigate to the project directory.

```bash
cd SortingWithCustomAdaptor/SortingWithCustomAdaptor
dotnet restore
dotnet run
```

4. Open the local URL displayed in the terminal after the application starts.

## Project Structure

- `SortingWithCustomAdaptor/SortingWithCustomAdaptor/Pages/Index.razor` — contains the `SfGrid` implementation, `SfDataManager` configuration, sample data generation, model definitions, and `CustomAdaptor` implementation used for sorting operations.
- `SortingWithCustomAdaptor/SortingWithCustomAdaptor/Data/` — contains supporting data-related files consumed by the sample application.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- For feature documentation, see the Syncfusion Blazor Custom Adaptor documentation: https://help.syncfusion.com/grid-sdk/blazor/data-grid/connecting-to-adaptors/custom-adaptor

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.