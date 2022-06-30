# Eclipse Setup

Eclipse Setup for SAP Development Environment (ABAP)

## ABAP Developer Tools (ADT)

Latest pre-requisites for Eclipse can be found on the [SAP Development Site (ABAP)](https://tools.hana.ondemand.com/#abap)

In a nutshell:

- Latest version of Eclipse (2022-03 4.16 at time of writing)
- Java JRE 11 (remember to set **JAVA_HOME**)
- **ABAP Development Tools** (Help->Install) - <https://tools.hana.ondemand.com/latest>

## Editor

**Marketplace Plugins:**

- ABAP Code Insight
- ABAP Continuous Integration
- Darkest Dark Theme (DevStyle)
- Eclipse Web Developer Tools

<img src="https://github.com/aawa69/EclipseSetup/blob/master/images/MarketplacePlugins.png" width="80%">

- **Nightlion** theme via the **DevStyle** plugin from the Marketplace
- Set Pastel icons
- Enable the Breadcrumb
- Set Explorer font size to 14

<img src="https://github.com/aawa69/EclipseSetup/blob/master/images/EclipsePreferences.png" width="80%">

- See [EclipseSAPColorSettings.xml](<https://github.com/aawa69/EclipseSetup/blob/master/EclipseSAPColorSettings.xml>)

Example in Eclipse:

<img src="https://github.com/aawa69/EclipseSetup/blob/master/images/EclipseKeywords.png" width="80%">

- Change all fonts to Fira Code or Monaco size 14 (fonts may need to be downloaded, else Helvetica Neue should be available OFTB and isn't too bad)
- Editor font can be amended globally via **Preferences > General > Appearance > Colors and Fonts > Basic > Text Font**

- Amend CDS keyword to orange:

<img src="https://github.com/aawa69/EclipseSetup/blob/master/images/EclipsePreferencesCDS.png" width="80%">

## Java & JavaFX

SAPGUI for ADT requires JavaFX to execute and isn't part of the JRE 11 install (FYI, is bundled as part of the standalone SAPGUI 🙄)

See SAP community - [JavaFX 13 and Eclipse](https://answers.sap.com/questions/12960323/javafx-13-and-eclipse.html)

- Download the openjfx SDK from [openjfx.io](https://openjfx.io/) site (for mac was openjfx-18.0.1_osx-x64_bin-sdk.zip as time of writing)
- Move the SDK to your **JavaVirtualMachines** folder (for me; *~/Library/Java/JavaVirtualMachines/javafx-sdk-18.0.1*)
- Add an **Eclipse.ini** ref to the SDK path > right click **Eclipse app > Show Package Contents > Contents > Eclipse > Eclipse.ini**

<img src="https://github.com/aawa69/EclipseSetup/blob/master/images/EclipseIniJavaFXReference.png" width="80%">
