---
title: Tabs on mobile
description: Describes the guidelines for designing tabs that work on mobile.
keywords: teams design guidelines reference framework personal apps mobile tabs
---
# Tabs on mobile


Custom tabs can be part of a channel, group chat, or personal app (apps that contain static tabs and/or a one-to-one bot).

Personal apps are available on mobile clients in the App Drawer. They can only be installed from a desktop or web client, and can take up to 24 hours to appear on mobile clients.

Group and channel tabs are available on mobile clients as well. The default behavior is currently to use your `websiteUrl` to launch your tab in a browser window. However, they can be loaded on a mobile client by clicking the `...` overflow menu next to the tab and choosing **Open**, which will use your `contentUrl` to load the tab inside the Teams mobile client.

![mobile app drawer](~/assets/images/app-drawer.png)

## Developer considerations for mobile support

When you're building an app that includes a tab, you need to consider (and test) how your tab will function on both the Android and iOS Microsoft Teams clients. The sections below outline some of the key scenarios you need to consider.

### Testing on mobile clients

You need to validate that your tab functions properly on mobile devices of various sizes and qualities. For Android devices you can use the [DevTools](~/resources/dev-preview/developer-preview-tools.md) to debug your tab while it is running. We recommend that you test on both high and low performing devices, as well as on a tablet.

### Responsive design

Because your tab can be opened on devices with a wide range of screen sizes, it needs to follow [responsive design](https://www.w3schools.com/html/html_responsive.asp) principles. All of the key constructs should be accessible on mobile devices, and the views should not be distorted. Ensure that when your tab is loaded on a mobile device, all buttons and links are easily accessible using finger-based navigation.

### Authentication

For authentication to work on mobile clients, you must upgrade you Teams JS SDK to at least version 1.4.1.

### Low bandwith & intermittent connections

Mobile clients regularly need to function with low bandwith and intermittent connections. Your app should handle any timeouts appropriately by providing a contextual message to the user. You should also user progress indicators to provide feedback to your users for any long-running processes.

## Design considerations for mobile

Our mobile platform allows apps to be an immersive experience with the app content taking up all of the screen apart from main Teams navigation. To create an immersive experience that fits seamlessly within the Microsoft Teams client, follow the guidelines below.

### Layouts

Choosing the correct layout for your tab is important. You should consider the kind of information you're presenting, and choose a layout that organizes it for easy consumption. Some potential options are outlined below.

#### Single canvas

This is one large area where work gets done. The Wiki app follows this pattern. If you have an app that doesn’t separate content into smaller components this would be a good fit.

![single canvas layout](~/assets/images/mobile-single-canvas.png)

#### List

Lists are great for sorting and filtering large quantities of data and are great at keeping the most important things at the top. It is helpful to use sortable columns. Actions can be added to each list item under the ellipsis menu.

![list layout](~/assets/images/mobile-list.png)

#### Grid

Grids are useful for showing elements which are highly visual. It helps to include a filter or search control at the top.

![grid layout](~/assets/images/mobile-grid.png)

### Tabs with bots on mobile

The below is an example personal app that contains two static tabs and a bot.

![tabs and bots on mobile](~/assets/images/mobile-tab-with-bot.png)

### UI Components

#### Color palettes

Using our approved neutral palette for backgrounds, notifications, text, and buttons will help your app feel more at home in Teams. Since Teams mobile has two colour themes (light and dark), it’s a good idea to make sure your app looks great in both.

##### Light color

![light color palette](~/assets/images/light-color.png)

##### Dark color

![dark color palette](~/assets/images/dark-color.png)

#### Buttons and controls

The way buttons are styled helps communicate what kind of action they trigger. We maintain a wide range of buttons that are formatted to show different levels of emphasis. Buttons can have text, an icon, or a combination of text and an icon. To communicate different levels in a hierarchy, we designed primary and secondary buttons within each category.

![buttons](~/assets/images/buttons.png)

![selection controls](~/assets/images/selection-controls.png)

![chiclets and pills](~/assets/images/chiclets-and-pills.png)

#### Typography

Typography should be clear and purposeful. Emphasize important information and avoid using multiple fonts and sizes to reduce confusion. We recommend using sentence case and avoiding the usage of all caps for localization and legibility.

![mobile typograph](~/assets/images/mobile-typography.png)

#### Fields and Flyouts

Fields are areas where users can input text. Flyouts are more lightweight than dialogs, and appear from the top pane.

##### List controls

![mobile list controls](~/assets/images/mobile-list-controls.png)

##### Field controls

![mobile field controls](~/assets/images/mobile-field-controls.png)
