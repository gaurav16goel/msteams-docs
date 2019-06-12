---
title: Developer Preview
description: Describes the features in the Public Developer Preview of Microsoft Teams
keywords: teams preview developer features
ms.date: 05/03/2019
---
# Public developer preview for Microsoft Teams

Developer Preview is a public program for developers which provides early access to unreleased features in Microsoft Teams. This allows you to explore and test upcoming features for potential inclusion in your Microsoft Teams app. We also welcome [feedback](~/feedback.md) on any feature in developer preview. Developer preview is enabled per Microsoft Teams client, so you don't need to worry about affecting your entire organization.

>[!NOTE]
>Features included in preview may not be complete, and may undergo changes before becoming available in the public release. They are provided for testing and exploration purposes only. They should not be used in production applications.

## Developer preview app manifest

Many features enabled in developer preview will require alterations to your app manifest JSON file. To do so you'll need to use the [developer preview manifest schema](~/resources/schema/manifest-schema-dev-preview.md) If you use this schema, you will not be able to use [App Studio](~/get-started/get-started-app-studio.md) to make these changes, nor will you be able to use it to upload your app for testing. To upload your app you'll need to click the `More apps` icon on the app bar, then select the `Upload a custom app link`. Using this method you can only upload a zipped version of your app package.

>[!NOTE]
>You may find it useful to use App Studio to create the non-developer preview portions of your app package, then export that package and manually edit the `manifest.json` file to add the developer preview features you wish to use. Once you've added developer preview features to the `manifest.json` file you will not be able to re-import the package into App Studio.

## Enable developer preview

>[!NOTE]
>Developer preview is enabled on a per-client basis. Uploading an app that uses developer preview features may cause clients that have not enabled developer preview to behave unexpectedly.

To enable the public developer preview on web/desktop clients, you need to do the following:

1. Turn on the setting for enabling uploading of apps in the admin console of your tenant as described [here](~/get-started/get-started-tenant.md).
2. Click on your profile (either in the upper right or lower left of the Teams interface) to display the Teams menu. The developer preview option is found in About → Developer preview. If you do not see an entry for developer preview the most likely reason is your organization is not configured for app uploading as described in step 

To enable the public developer preview on mobile app clients, you need to do the following:

1. Turn on the setting for enabling uploading of apps in the admin console of your tenant as described [here](~/get-started/get-started-tenant.md).
2. On Teams mobile apps developer preview mode is being released from June 2019 app builds.Steps to enable developer preview on mobile:
a) Download/Upgrade to latest Teams mobile app from play store/app store 
b) Developer preview option is found in Settings >About > Developer preview. If you do not see an entry for developer preview the most likely reason is your organization is not configured 1 

## Disable developer preview

Use the same menu item under About → Developer preview, and click on it to turn it off.

## Features available in developer preview

For a full list of the features currently enabled in developer preview see: [Features in the public developer preview](~/resources/dev-preview/developer-preview-features.md).
