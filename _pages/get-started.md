---
title:  "Get Started"
layout: single
permalink: /get-started/
author_profile: false
comments: false
---


# Installing the R-ArcGIS Bridge
Note: If you encounter problems, please create an issue so that we can take a look.

## Prerequisites

ArcMap 10.3.1 or later or ArcGIS Pro 1.1 or later (Don’t have it? Try a 60 day trial!).

R Statistical Computing Software, 3.2.2 or later (What is R?).

R has both a 64-bit and a 32-bit version. The 32-bit version of R is required for ArcMap, while the 64-bit version is required for ArcGIS Pro (Note: the installer will install both by default).
The 64-bit version of R can be used with ArcGIS Pro, or additionally, with ArcMap by installing Background Geoprocessing and configuring scripts to run in the background. (Note: Background Geoprocessing only allows using the bridge from ArcGIS, not from within R itself.)

## Installation
To start …
First, make sure you’ve installed an appropriate version of R, 3.2.2 or later.

Next, identify the appropriate section for your version of ArcMap or ArcGIS Pro, either ArcGIS 10.3.1 or later, ArcGIS Pro 1.1-1.4.1, or ArcGIS Pro 2.0, and follow those instructions.

### ArcGIS 10.3.1 or later

Go to the R-ArcGIS bridge installation page and click the Clone or download button and select to Download ZIP.

Locate the downloaded file on your computer. Right-click the r-bridge-install-master zipped folder and extract to a location you can easily find, such as your Documents folder.

Open ArcMap and if necessary, click on the Windows tab to open the Catalog pane for your project.

In the Catalog window, navigate to and add a folder connection to the folder location you extracted to which contains the Python Toolbox,  R Integration.pyt.

Open the toolbox, which should look as seen below, to view the four script tools it contains:


Run the Install R bindings script. You can then test that the bridge is able to see your R installation by running the Print R Version and  R Installation Details tools, and running the included sample tools.
The clip below shows the steps listed above and how to verify proper installation of the bridge:


### ArcGIS Pro 1.1 - 1.4.1

Go to the R-ArcGIS bridge installation page and click the Clone or download button and select to Download ZIP.

Locate the downloaded file on your computer. Right-click the r-bridge-install-master zipped folder and extract to a location you can easily find, such as your Documents folder.

Open ArcGIS Pro and if necessary, click on the View tab to open the Catalog pane for your project.

In the Catalog pane, navigate to and add a folder connection to the folder location you extracted to which contains the Python Toolbox,  R Integration.pyt.

Open the toolbox, which should look as seen below, to view the four script tools it contains:

Run the Install R bindings script. You can then test that the bridge is able to see your R installation by running the Print R Version and  R Installation Details tools, and running the included sample tools.
ArcGIS Pro 2.0+
Open ArcGIS Pro and click on the Project tab in your project.

Select Options on the blue left-hand side panel and in the pop-up window, under Application, select Geoprocessing.

Under the R-ArcGIS Support options, select your desired R home directory. (Note: All versions of R installed on your computer will appear in the drop-down menu. Make sure the version you select is R 3.2.2 or later.)

If you have previously installed the R-ArcGIS bridge, you will see an installed message that lets you know the version of your arcgisbinding package and allows you to check for updates, download the latest version, or update from a file. Check for updates and ensure you have the latest version of the arcgisbinding package. If prompted to update, click ‘Yes’ and the latest version will automatically be installed.

If you have never installed the R-ArcGIS bridge, you will see a warning indicating that you need to install the arcgisbinding R package, to enable R to connect with ArcGIS. As such, when you click on the icon next to the warning you will be presented with options to automatically download and install the arcgisbinding package, or to separately download the package, or to install the package from file. Select the first option to automatically download and install the arcgisbinding package.

### Offline Installation

From a machine that does have internet access:
Download this repository.
Download the latest version of the arcgisbinding R package. As of writing, this is arcgisbinding_1.0.0.125.zip.
Copy both zip files onto the machine that you’re performing the offline installation on. Extract the r-bridge-install zip into a folder you can easily locate and place the arcgisbinding_1.0.0.125.zip into the same folder location as the “R Integration” Python toolbox.
Run the installation procedure as listed above under either ArcGIS 10.3.1 or later if you are using ArcMap or under ArcGIS 1.1 - 1.4.1 if you are using Pro.
Problems Installing?
A few things to check :
All prerequisites have been met, such as the right version of R for your platform, and a current release of ArcGIS.
Make sure that your user has administrator access, and try running ArcGIS as an Administrator:
Start ArcGIS as an administrator, by right clicking the icon, selecting ‘Run as Administrator’, then trying the script
On Windows 7, KB2533623 must be installed. Without this hotfix, the library will generate the error “The procedure entry point AddDllDirectory could be located”.
Additionally, the release can be manually installed into R, as shown in this screencast. Use this if you’re planning on mostly working from R.
Still stuck? Add an issue and we’ll take a look. (More about GitHub Issues)
Next Steps
Additional resources and discussion on the bridge can be found at the R-ArcGIS project on GeoNet.

#### Want additional resources to learn how to use the bridge and about how it can extend your workflows?

Check out the Learn Lesson: Analyzing Crime Using Statistics and the R-ArcGIS Bridge
Check out the web course: Using the R-ArcGIS Bridge
Check out the web course: Integrating R Scripts into ArcGIS Geoprocessing Tools
Want to use tools others have developed?

See how complex problems can be solved with R and ArcGIS in the Sample Tools, such as model-based clustering and combining parametric and non-parametric models with semiparametric regression.
Check out the community page for more tools Coming Soon!
Want to develop new tools using R?

Learn about all the functions contained within the arcgisbinding package and how to use them for development in the package vignette.

Additional development resources can be found within the bridge repository and the package documentation.

## Credits
This toolbox depends on the R Statistical Computing Software:

Copyright (C) 2015 The R Foundation for Statistical Computing R is free software and comes with ABSOLUTELY NO WARRANTY. See the COPYRIGHTS file for details.