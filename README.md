# Pride Month Calendar PowerApp
Welcome to the Pride Month Calendar PowerApp. This PowerApp template provides an adjustable Pride Month calendar for your company or team. It can be easily imported into your (default) environment and shared within the organization with no additional connector needed.

**Content**
1. [Technical Requirements](#Technical-Requirements)
2. [Download](#Download)
3. [Installation](#Installation)
4. [Customization](#Customization)
    1. [Introduction text](#I-want-to-change-the-introduction-text-on-the-left-side)
    2. [Logo or background image](#I-want-to-change-the-logo-or-background-image)
    3. [Change content of the pride month calendar](#I-want-to-change-the-content-of-the-pride-month-calendar)
    4. [Change name, description, icon, or background color](#i-want-to-change-the-powerapp-icon-name-description-or-background-color-during-startup)
    5. [Republishing](#Republishing-the-app) 
5. [Content packs](#Content-packs)
6. [Customize the content](#Customize-the-content)
7. [Pin the Pride Month Calendar app in Teams for all users](https://github.com/nschreder/powerappadventcalendar/blob/main/Readme/Installation/pintoteams.md)

## Technical Requirements
* Power Platform license (dedicated license e.g., "Power Apps per User" or included with your Microsoft 365 license)
* Default, Microsoft Teams or dedicated environment
* Microsoft Excel (optional)
* Screen resolution of 1366x768 pixels (minimum)

## Download
There are multiple versions of the advent calendar app with content packs pre-installed:
- [Advent Calendar Teams Edition (German)](/App/AdventCalendarTeamsDE.zip).
- [Advent Calendar Teams Edition (English)](/App/AdventCalendarTeamsEN.zip).
- [Advent Calendar Power Platform Edition](/App/AdventCalendarPowerPlatform.zip).

![GitHub](https://github.com/nschreder/powerappadventcalendar/blob/main/Readme/Installation/Installation%20Download.png)

## Installation
1. Open the [PowerApps Studio](https://make.powerapps.com) and select your default/desired environment:

![PowerApps Studio](https://github.com/nschreder/powerappadventcalendar/blob/main/Readme/Installation/Installation%20Step%201.png)

2. In the left navigation bar, click on "Apps" and then "Import canvas app":

![PowerApps Studio](https://github.com/nschreder/powerappadventcalendar/blob/main/Readme/Installation/Installation%20Step%202.png)

3. Use the file picker, and choose the recently downloaded Power App zip file. Specify the "Import Setup" field (new if you install it the first time, upgrade if you already have a previous version installed) and click on "Import":

![PowerApps Studio](https://github.com/nschreder/powerappadventcalendar/blob/main/Readme/Installation/Installation%20Step%203.png)

4. After the import, you can customize the Pride Month calendar Power App using the "Open app" link or app explorer in the left navigation panel. Otherwise, you can share it immediately within your company and your colleagues:

![PowerApps Studio](https://github.com/nschreder/powerappadventcalendar/blob/main/Readme/Installation/Installation%20Step%204.png)

## Customization
You have several options available to customize the Pride Month calendar PowerApp. To start with the customization process, you must open the app in edit mode using [PowerApps Studio](https://make.powerapps.com):

![PowerApps Studio](/Readme/Customization/Customization%20Step%201.png)

**Information**: After customizing the PowerApp, you must [republish](#Republishing-the-app) your app again.

### I want to change the introduction text on the left side
To change the introduction text, you must click on "CalendarIntroLabel" (child of "CalendarIntroContainer") in the tree view on the left side of the PowerApps Studio. In the properties editor, you can change the text in the "Text" field.

![PowerApps Studio](/Readme/Customization/Customization%20Text%20Step%201.png)

### I want to change the logo or background image
To change the logo, you must click on "CompanyLogo" in the tree view on the left side of the PowerApps Studio. In the properties editor, you can change the image in the "Image" field by uploading a new image and selecting it.

![PowerApps Studio](/Readme/Customization/Customization%20Logo%20Step%201.png)

To change the background image, you must click on "CalendarScreen" in the tree view on the left side of the PowerApps Studio. In the properties editor, you can change the background image in the "Background image" field by uploading a new image and selecting it.

![PowerApps Studio](/Readme/Customization/Customization%20Background%20Step%201.png)

### I want to change the content of the Pride Month calendar
1. Open the data section on the left side and remove the existing "Content" data source by clicking on "..." and then "Remove":

![PowerApps Studio](/Readme/Customization/Customization%20Content%20Step%201.png)

2. Add your [customized](#Customize-the-content) or the [pre-defined](#Content-packs) content by clicking on "Add data" and searching for/selecting the "Import from Excel" data source:

![PowerApps Studio](/Readme/Customization/Customization%20Content%20Step%202.png)

3. Select your customized Excel spreadsheet and click on "Content" in the "Choose a table" panel. Click on "Connect" to import the Excel file:

![PowerApps Studio](/Readme/Customization/Customization%20Content%20Step%203.png)

4. To refresh your data in the PowerApp, click on "Tree View", select "App" by clicking on "..." next to it, and "Run OnStart":

![PowerApps Studio](/Readme/Customization/Customization%20Content%20Step%204.png)

### I want to change the PowerApp icon, name, description, or background color (during startup)
You can change the icon in the app described [here](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/set-name-tile).

### Republishing the app
1. Open the file menu by clicking on "File" in the menu:

![PowerApps Studio](/Readme/Customization/Customization%20Step%202.png)

2. In the save menu click on "Save" and then "Publish":

![PowerApps Studio](/Readme/Customization/Customization%20Step%203.png)

## Content packs
| Name | Description | Link |
|---|---|---|
| Pride | A content pack specific for the Pride Month. | TBA |

## Customize the content
If you want to customize the Pride Month calendar and import your content, you can start with downloading and editing the [template](https://github.com/nschreder/powerappadventcalendar/raw/main/Content/Template/Template.xlsx) in Microsoft Excel. After adjusting it you can [change the content of the Pride Month calendar](#I-want-to-change-the-content-of-the-pride-month-calendar).

![Excel](/Readme/Customization/Customization%20Content%20Step%205.png)

| Field | Description |
|---|---|
| Title | The title for the entry. |
| Day | The day for the entry. It only can be opend during/after the day. |
| Type | The Pride Month calendar can show different types of content. The types "Image", "Video", and "PDF" will open the content in the specific player/reader, and "URL" will redirect the user directly to the source by opening a new browser tab. |
| Content | The content shown after opening the entry (URL). |
| Link (optional) | This optional attribute shows a link below the content, and the user can get additional information (URL). |
| Index | The index of the entry. E.g., the first entry is "1", the 2nd entry in the 3rd line is "14". |

**Information:** Excel is formatting links differently as PowerApps is processing it. To ensure a working solution, make sure that you only include text values instead of links.

# Pin the Pride Month Calendar app in Teams for all users
How to [pin the Pride Month Calendar app in Teams for all users](https://github.com/nschreder/powerappadventcalendar/blob/main/Readme/Installation/pintoteams.md).
