<a id="readme-top"></a>

# pXLabs MS Win32 Prep Tool GUI

This GUI has been written to allow you to quickly assemble and execute the `IntuneWinAppUtil.exe` command without the need to type or copy and paste the parameters needed to create an Intune `Windows app (Win32)` application.

![Screenshot](images/Interface.png?raw=true)

# Getting Started
To get started, you can either download and execute the `pXLabs MS Win32 Prep Tool GUI.ps1` script or grab the compiled executable in Releases.

## Prerequisites
* Powershell 5.1
* `IntuneWinAppUtil.exe` which can be downloaded from here: https://github.com/microsoft/Microsoft-Win32-Content-Prep-Tool

## Form Controls
Control | Command | Description 
|:----------|:--------|:-----------
Source Folder | -c <source_folder> | Folder that contains the installation content
Setup File | -s <source_setup_file> | Path to the installation file
Output Folder | -o <output_folder> | Destination folder for the resultant *.Intunewin file
Catalog Folder | -a <catalog_folder> | Optional folder that contains catalog files to include in the *.Intunewin file
Execute | Alt + e | Run IntuneWinAppUtil.exe using the values provided.
Show cmd | Alt + s | Display the fully formed IntuneWinAppUtil.exe command.
Open Intune | Alt + o | Copys intunewin file link to the clipboard and opens the Intune Apps link.
Quiet mode | -q | Run in 'quiet mode'. If the output file already exists, it will be overwritten. 
Copy | Alt + c | Copy the displayed output to the clipboard.
Exit | Alt + x | Exit the application
![Screenshot](images/Help.png?raw=true) | | Display GUI and command line help

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# Usage
Whether you choose to use the script or the executable, the process is the same once it is launched.

1. Copy the content you wish to package into it's own folder.
2. Open the application or script. 
   - If the working directory does not contain the `IntuneWinAppUtil.exe`, you will be asked to locate it. 
   - Once the `IntuneWinAppUtil.exe` is located and selected, you can choose to copy it to the working directory or you can leave it in it's current location.
3. Select the source folder that was identified in step 1.
4. Select the setup file.
5. Select the output folder.
   - If the output folder does not currently exist, you'll be asked if you wish to create it.
   - If you choose not create the folder, selecting quiet mode will allow the process to create it when it is executed.
6. If needed, select the catalog folder you wish to include in the *.Intunewin file.
7. At this point you can either choose to run the command by pressing `Execute` or you can click `Show cmd` and click `Copy` to copy the command to the clipboard.
8. If you choose to execute the command, it will execute, display the result and prompt to open the output folder.
9. If you are ready to publish the resulting `*.Intunewin` file, click `Open Intune`.
   - At this point the full `*.Intunewin` file path will be copied to the clipboard to be used when publishing the app in the opened Intune link.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Jeff Pollock - [@LinkedIn](https://www.linkedin.com/in/jeff-pollock-12b42a22/) - PhriendX@live.com

Project Link: [https://github.com/phriendX/pXWin32ContentPrepGUI](https://github.com/phriendX/pXWin32ContentPrepGUI)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
