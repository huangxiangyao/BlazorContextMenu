# Blazor Context Menu

A context menu for Blazor 


> ⚠️ Warning: This project is build on top of an experimental framework. There will probably be breaking changes from version to version.



## Installation

```
> dotnet add package Blazor.ContextMenu

OR

PM> Install-Package Blazor.ContextMenu
```
Nuget package page can be found [here](https://www.nuget.org/packages/Blazor.ContextMenu)

## Usage

### Basic usage

```xml
<ContextMenu Id="myMenu">
    <MenuItem Click="@OnClick">Item 1</MenuItem>
    <MenuItem Click="@OnClick">Item 2</MenuItem>
    <MenuItem Click="@OnClick" IsEnabled="false">Item 3 (disabled)</MenuItem>
    <MenuSeperator />
    <MenuItemWithSubMenu>Submenu
        <SubMenu>
            <MenuItem Click="@OnClick">Submenu Item 1</MenuItem>
            <MenuItem Click="@OnClick">Submenu Item 2</MenuItem>
        </SubMenu>
    </MenuItemWithSubMenu>
</ContextMenu>

<ContextMenuTrigger MenuId="myMenu">
    <p>Right-click on me to show the context menu !!</p>
</ContextMenuTrigger>

```


## Special Thanks
This project is inspired by https://github.com/fkhadra/react-contexify, a context menu for react.