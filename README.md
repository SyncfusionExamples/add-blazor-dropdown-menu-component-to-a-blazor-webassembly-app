# How to Add the Syncfusion Blazor Dropdown Menu Component to a Blazor WebAssembly App

## Overview

This sample demonstrates how to integrate the Syncfusion [Blazor Dropdown Menu](https://www.syncfusion.com/blazor-components/blazor-dropdown-menu) component into a hosted Blazor WebAssembly application. The application showcases common menu customization scenarios that are frequently required in modern web applications, including menu item icons, icon positioning, navigation actions, horizontal menu layouts, hidden arrow indicators, and menu item click handling.

The sample serves as a practical reference for developers who want to implement command menus, navigation menus, or action-based dropdown interfaces using Syncfusion Blazor components. It also demonstrates the project structure commonly used in a hosted Blazor WebAssembly solution with Client, Server, and Shared projects.

## Key Features

- Configures the button text through the `Content` property.
- Displays a custom menu icon using the `IconCss` property and a custom icon font.
- Positions the icon on the left side of the button using `IconPosition="SplitButtonIconPosition.Left"`.
- Applies custom styling through the `CssClass` property to control menu appearance and hide the default caret icon.
- Uses the `DropDownMenuItems` collection to define multiple menu actions.
- Demonstrates menu item configuration using the `DropDownMenuItem` component and the `Text` property.
- Shows dynamic menu item enabling and disabling through the `Disabled` property.
- Handles the `OnOpen` event using `DropDownButtonEvents` to update menu-item state before the menu is displayed.
- Uses the `DisableListItem(BeforeOpenCloseMenuEventArgs args)` method to toggle the disabled state of the **Delete** menu item.
- Demonstrates menu-based navigation using the `Url` property to open an external webpage.
- Opens external links in a new browser tab using `target="_blank"`.
- Uses custom CSS to display menu items horizontally and apply customized visual styling.
- Includes a hosted Blazor WebAssembly sample with a Weather Forecast page that retrieves data from an ASP.NET Core Web API endpoint.
- Demonstrates asynchronous data retrieval using `HttpClient.GetFromJsonAsync<WeatherForecast[]>()`.
- Includes a server-side `WeatherForecastController` that generates and returns sample forecast data.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the `DropDownMenuSample.sln` solution file.
3. Restore all NuGet packages.
4. Set the hosted Blazor startup project if required by your environment.
5. Build the solution.
6. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository root folder in Visual Studio Code.
2. Navigate to the repository directory.

```bash
dotnet restore
dotnet run
```

3. Open the application URL displayed in the terminal.
4. Navigate to the page that hosts the Dropdown Menu sample.
5. Interact with the menu items and customization examples.

## Project Structure

- `DropDownMenuSample.sln` - Solution file for the hosted Blazor WebAssembly sample.

- `Client/Pages/Index.razor` - Main sample page demonstrating the Syncfusion `SfDropDownButton` component, menu-item configuration, custom icons, external navigation, horizontal menu styling, and `OnOpen` event handling.

- `Client/Pages/FetchData.razor` - Sample page that retrieves weather forecast data from the server using `HttpClient` and displays the results in a table.

- `Server/Controllers/WeatherForecastController.cs` - ASP.NET Core Web API controller that generates and returns forecast data consumed by the client application.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Official Syncfusion Dropdown Menu documentation: https://blazor.syncfusion.com/documentation/drop-down-menu/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.