All Picture Image Viewer

This is example how to create WPF application with F\# (F sharp) only
with

Dot Net Core 3.1

Create F\# Core 3.1 Console App (.Net Core) , give project name and
"Create".

![](media/image1.png){width="2.7503838582677167in"
height="1.458536745406824in"}

Right click on project and "Unload Project"

![](media/image2.png){width="2.6999682852143483in" height="3.78125in"}

![](media/image3.png){width="3.0105336832895886in"
height="1.7916666666666667in"}

And replace

\<Project Sdk=\"Microsoft.NET.Sdk\"\>

\<PropertyGroup\>

\<OutputType\>Exe\</OutputType\>

\<TargetFramework\>netcoreapp3.1\</TargetFramework\>

\</PropertyGroup\>

....

To this

\<Project Sdk=\"Microsoft.NET.Sdk.WindowsDesktop\"\>

\<PropertyGroup\>

\<OutputType\>WinExe\</OutputType\>

\<TargetFramework\>netcoreapp3.1\</TargetFramework\>

\<UseWPF\>true\</UseWPF\>

\</PropertyGroup\>

....

Save and reload project.

Mostly done.

For template or full working example please use this application.

![](media/image4.png){width="3.40625in" height="2.13951334208224in"}

For create subproject use absolutely same rule.

Add subproject like dependent.

Pay your attention about class Utilities (file Utilities.fs) it include
everything for download XAML file from assembly and convert it to
content, find user control...

-   For converting word doc to readme.nd file I used
    <https://pandoc.org/MANUAL.html>
