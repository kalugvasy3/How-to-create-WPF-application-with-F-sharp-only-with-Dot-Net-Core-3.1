## All Picture Image Viewer

This is example how to create WPF application with F\# (F sharp) only
with

Dot Net Core 3.1

Create F\# Core 3.1 Console App (.Net Core) , give project name and
"Create".

![](media/image1.png)


# Right click on project and "Unload Project"

![](media/image2.png)

![](media/image3.png)

# And replace

\<Project Sdk=\"Microsoft.NET.Sdk\"\>

\<PropertyGroup\>

\<OutputType\>Exe\</OutputType\>

\<TargetFramework\>netcoreapp3.1\</TargetFramework\>

\</PropertyGroup\>

....

# To this

\<Project Sdk=\"Microsoft.NET.Sdk.WindowsDesktop\"\>

\<PropertyGroup\>

\<OutputType\>WinExe\</OutputType\>

\<TargetFramework\>netcoreapp3.1\</TargetFramework\>

\<UseWPF\>true\</UseWPF\>

\</PropertyGroup\>

....

# Save and reload project.

# Mostly done.

# For template or full working example please use this application.

![](media/image4.png)

## For create subproject use absolutely same rule.

# Add subproject like dependent project.

# Pay your attention about class Utilities (file Utilities.fs) it include
# everything for download XAML file from assembly and convert it to
# content, find user control...

# All XAML file must be ## Embedded resource

![](media/image5.png)

-   For converting word doc to readme.nd file I used
    <https://pandoc.org/MANUAL.html>
