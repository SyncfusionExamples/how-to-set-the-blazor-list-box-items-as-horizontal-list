# How to Set Syncfusion Blazor ListBox Items as a Horizontal List

## Overview

This sample demonstrates how to render Syncfusion [Blazor ListBox](https://www.syncfusion.com/blazor-components/blazor-listbox) items horizontally in a Blazor application by applying custom styling through the ListBox component configuration. The implementation uses the `CssClass` property to associate a custom CSS class with the component, allowing the default vertical item arrangement to be transformed into a horizontal layout.

This approach is useful when ListBox items should be presented in a compact row-based format, such as category selectors, tag pickers, navigation-style lists, or dashboard filters.

## Key Features

- Demonstrates the Syncfusion Blazor ListBox component configured with the `CssClass` property to render items in a horizontal layout.
- Uses the `SfListBox` component with `TValue="string[]"` and `TItem="DataValues"` for strongly typed item selection and data binding.
- Binds local data through the `DataSource` property using a collection of custom `DataValues` objects containing item text and identifier values.
- Initializes selected items using the `Value` property to preselect one or more ListBox entries when the component loads.
- Applies custom CSS to the ListBox container and internal item elements (`.e-list-parent` and `.e-list-item`) to replace the default vertical arrangement with a horizontal scrolling layout.
- Demonstrates horizontal alignment of ListBox items using the CSS `inline-flex` display mode for the ListBox item container.
- Includes a sample data model (`DataValues`) that illustrates binding custom business objects to ListBox items.
- Provides a Blazor routing example through the `@page` directive for component-based navigation.
- Includes a weather forecast sample page that demonstrates dependency injection, asynchronous data retrieval, and data rendering using `WeatherForecastService` and `WeatherForecast` model classes.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open `HorizontalListItem.sln`.
3. Restore NuGet packages.
4. Build the solution.
5. Run the project using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Navigate to the project directory.
3. Restore dependencies:

```bash
dotnet restore
```

4. Run the application:

```bash
dotnet run
```

5. Open the local URL displayed in the application output window.

## Project Structure

`Pages/Index.razor` - Main sample page that demonstrates the Syncfusion Blazor ListBox configured as a horizontal list using the `CssClass="e-horizontal-listbox"` property, local data binding through `DataSource`, item selection through `Value`, and custom CSS styling.

`Pages/FetchData.razor` - Additional Blazor sample page that demonstrates dependency injection, asynchronous data retrieval from `WeatherForecastService`, and rendering forecast data in a table.

`Data/WeatherForecast.cs` - Data model representing forecast records with `Date`, `TemperatureC`, calculated `TemperatureF`, and `Summary` properties.

`Data/WeatherForecastService.cs` - Service class that generates sample weather forecast data and exposes the `GetForecastAsync()` method consumed by `FetchData.razor`.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the Syncfusion Blazor ListBox documentation: https://blazor.syncfusion.com/documentation/listbox/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.