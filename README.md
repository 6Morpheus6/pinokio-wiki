# Pinokio Wiki

- [Pinokio Wiki](#pinokio-wiki)
  - [General](#general)
    - [Install Pinokio](#install-pinokio)
    - [Change the location where Apps are downloaded and installed (Home)](#change-the-location-where-apps-are-downloaded-and-installed-home)
    - [Install Apps with Pinokio](#install-apps-with-pinokio)
    - [Delete installed Apps](#delete-installed-apps)
    - [Upgrade Pinokio](#upgrade-pinokio)
    - [Uninstall Pinokio](#uninstall-pinokio)
    - [Report Bugs](#report-bugs)
  - [Pinokio](#pinokio)
    - [Home Screen](#home-screen)
    - [Settings](#settings)
    - [Discover Page](#discover-page)
    - [Application screen](#application-screen)
      - [Launching the App](#launching-the-app)
      - [Terminal](#terminal)
      - [Update, Reinstall, Factory Reset and Delete](#update-reinstall-factory-reset-and-delete)
      - [Files](#files)
    - [Model and File Management](#model-and-file-management)
  - [Applications](#applications)
    - [Stable Diffusion Models](#stable-diffusion-models)
    - [Download different models for Stable Diffusion, Fooocus and ComfyUI](#download-different-models-for-stable-diffusion-fooocus-and-comfyui)
  - [Troubleshooting](#troubleshooting)
  - [Requirements (not verified)](#requirements-not-verified)
    - [Stable Diffusion](#stable-diffusion)
    - [Fooocus](#fooocus)
    - [ComfyUI](#comfyui)
    - [InstantID](#instantid)
    - [IP-Adapter-FaceID](#ip-adapter-faceid)
    - [Video2Densepose](#video2densepose)
    - [Audio Gradio](#audio-gradio)
    - [Moore-AnimateAnyone / Moore-AnimateAnyone-Mini](#moore-animateanyone--moore-animateanyone-mini)

## General

### Install Pinokio

- Follow the instructions in [Pinokio Tutorial](https://docs.pinokio.computer/download/) to install Pinokio for [Windows](https://docs.pinokio.computer/download/windows.html), [Mac](https://docs.pinokio.computer/download/applemac.html), [Intel Mac](https://docs.pinokio.computer/download/intelmac.html) and [Linux](https://docs.pinokio.computer/download/linux.html).

### Change the location where Apps are downloaded and installed (Home)

The Home Directory is the place where all your Apps and needed components will be installed.  
The location of the Home Directory can be changed in Pinokio - Settings (The wheel in the top right corner on the Pinokio main page).

- The path to the new location may not contain spaces, special characters or non-Unicode letters. Underscores, dashes and numbers are allowed.
- The drive hosting your new Home Directory must be formatted with the NTFS file system.
- The new Home Directory folder must have read and write permissions for all users.
- The location of your new home may not yet exist.
- It's recommended to name your Home Directory Pinokio (e.g.: `C:\AI\pinokio`)
- The drive needs to have enough space. *Apps, models and components can have a size up to 100GB. (For most Apps a min. size of 50GB should be enough)*

Once you've set your new location, click the *Save* button and wait until Pinokio has finished to move your files to the new location.  
Depending on the amount of files this may take some time.  
**Don't abort** this process or turn off your computer until it has fully completed or Pinokio might not start properly next time.

### Install Apps with Pinokio

Visit the Discover page in Pinokio to install new Apps.  
Click on the Icon of the App you want to Install and click the Download button.  
Choose the default folder or set a new name for the App folder and click Install.

### Delete installed Apps

The `api`  folder contains all your installed Apps. Just delete the according app.Pinokio.git folder in your explorer.  
To delete an App simply go to `.\pinokio\api` If you don't know where to find this folder, just have a look at Pinokio - Settings (The wheel in the top right corner on the Pinokio main page).  
Navigate there with your Explorer or File Manager and in there you will see the `api` folder.

### Upgrade Pinokio

- Close Pinokio if it is still open.
- Go to [Pinokio Computer](https://github.com/pinokiocomputer/pinokio), click ***Latest*** on the right side of that page and choose the correct version for you system.
- Download and install Pinokio. This will replace your old Pinokio version with the new one without touching your installed Apps.
- Now you can start Pinokio again and move on with your new version.

### Uninstall Pinokio

You can uninstall Pinokio like any other program on your system.  
There is also an Uninstall Pinokio file in the same folder like the Pinokio program.  
On Windows it is located in: `C:\Users\YourName\AppData\Programs\Pinokio`  
On a Mac it is in: `~% / Applications/`  
This will only uninstall Pinokio ***not*** your Apps. Your Home directory will stay ***untouched***.  
To remove Pinokio and all its components completely from your system, you need to delete the `pinokio` folder of your home directory as well. Additionally you can search for *Pinokio* with your Explorer and delete everything you find.

### Report Bugs

If you find a bug, if anything isn't working as expected, or if you have issues running an Application, please visit the Pinokio Discord Server and post your issue in the #support channel.

- Describe your issue in [#quick-questions](https://discord.gg/U8X6uPtG3Z) and post a screenshot if possible (quickest way to get help).
- If you need help with any of the Applications, please visit the [#app-questions](https://discord.gg/5ssuhP5zwh) channel to ask for advice
- Or hit the report bug button at the top right corner on the Pinokio main page and post your logs in the [#forum](https://discord.gg/aHFHh2WSRq) and describe the issue or bug.

---

## Pinokio

### Home Screen

The Home screen of Pinokio is divided in 2 sections.  

- **Not Running** lists all downloaded and Installed Apps in Pinokio.  
- **Running** lists all Apps launched with their according Start / Launch button.

Currently running Apps are displayed with a green frame and a spinning circle at the top of the Home screen.  
*Although it is **technically possible** to run more than one Application at the same time, it **isn't recommended** since most of the Apps have a significant performance consumption.*

### Settings

The settings page displays the currently installed Pinokio version and can be reached by clicking the wheel at the top right corner of the home screen.
Here you can:

- Change the color theme
- [Change the location of your Home directory](#change-the-location-where-apps-are-downloaded-and-installed-home)

### Discover Page

The Discover page in Pinokio allows you to install new Apps. Click on an App's icon to view more details, then click the Download button. In the following window, choose a folder name and click **Download** to download the App with Pinokio.
All downloaded Apps will be displayed on the Pinokio home screen and can be installed from there.
> Note: Applications labeled with **VERSION 1** only work with **Pinokio 1.0.15** or higher!

Applications not created by a verified publisher and not tagged as ***Pinokio*** on GitHub don't appear on the Discover page. They can be still installed via the Download from URL button on the top of the Discover page.
*This method can also be used if the normal way to Download an App fails (e.g. because of a notification to update Pinokio although it is still up to date when trying to download an App the regular way on the Discover page).*  
> Note: Only Applications with a `pinokio.js` and respective *install.json* and *start.json* scripts etc. can be installed via Pinokio.  
To find out if an Application on GitHub that doesn't appear on the Discover page can be installed with Pinokio, have a look on the GitHub repo and check if it contains a *pinokio.js* script on the main page.  

### Application screen

Click an App on the Pinokio Home screen to see the Application screen

#### Launching the App

To start the application, click the *Start* / *Launch* button and wait until it is fully launched.  
Once launched, an **Open WebUI** or **Open Session** button will appear to use the App inside of Pinokio.  
To use the application in your default browser, click the **Open External** button above the user interface.

#### Terminal

The Terminal / Server displays all processes, errors and details about the App.  
Here you can also stop and restart the App again by clicking the **Stop** / **Run** button on the top.

#### Update, Reinstall, Factory Reset and Delete

- To update an App, close it if running and click the **Update** button. *This will update the app to the latest version.*  
- To reinstall an App, close it if running and click **Reinstall**. *This will reinstall the App without deleting any data or creations.*  
- A **Factory Reset** will delete the App but not the Pinokio scripts. *It will still be displayed on the Pinokio home screen and can be reinstalled any time.*  
Not all Apps come with an Update, Reinstall or Factory Reset button
- To delete an App, close it if running and click **Delete**. A window appears asking if you are really sure to delete the App and all its content. *This will delete the App completely and it will not be displayed on the Pinokio home screen anymore.*

#### Files

The Files button leads to the Pinokio scripts, App-folder, subfolders and all containing files. It is even possible to edit and save these files within Pinokio, although it is recommended to use an appropriate Editor or IDE for that purpose.  
This should only be done in exceptional cases and with caution since a mistake can easily break the App.  
*It's always wise to make a backup of the original files before modifying them.*
> **Note: A *Factory Reset will delete all files and folders* in the App folder *including your output and custom models! Always* make sure to *save all important files and models beforehand*!**

### Model and File Management

- Pinokio will be installed in
  - `C:\Users\YourName\AppData\Programs\Pinokio` on Windows  
  - `~% / Applications/` on Mac
- Applications will be installed in `.\pinokio\api`
  - Each App has their very own Outputs and models folder.
    - Output folder houses all generated files
    - Models are stored in the Models / Checkpoints folder  

>Note: If you delete an Application or click the ***Factory Reset*** Button, the Output and Models folder will be deleted as well.  
**Make sure to save any important *Output Files* and *Models* before you delete an App!**

- The **bin** folder `.\pinokio\bin` contains all required components for Applications. These *pre-requirements* (Conda, git, zip, etc.) will be installed in `.\pinokio\bin\miniconda`
- The **Logs** folder `.\pinokio\logs` stores all installation logs, launch protocols and system information needed to troubleshoot issues.  
  This folder will be automatically zipped when you hit the ***Report Bug Button***.
- Temporary files are stored in the **Cache** folder `.pinokio\Cache` e.g. *Pip_Cache* for components, *Temp* and *Gradio_Temp* for intermediate output files.  
An exception is *HF_Home* and *XDG_DATA_HOME*. Some Apps download their default models in there when they launch the first time.
*Principally it is possible to delete all files in the Cache folders, these files will be automatically downloaded if they are needed again.*

> Note: Some of these files, especially models, can be very large and should be kept to save time.

- The **drive** folder `.\pinokio\dirve` is a shared models folder used by Stable Diffusion based Applications to save drive space.
  Models, Loras, Embeddings and many more downloaded and stored in their according folders in `.\pinokio\drive\drives\peers\d1704581225212\` can be used by Automatic1111, Fooocus, and ComfyUI without moving or copying the models.

## Applications

### Stable Diffusion Models

### Download different models for Stable Diffusion, Fooocus and ComfyUI

If your computer doesn't have enough performance to use SDXL models, you can download finetuned **SD1.5** Models from [Civitai](https://civitai.com).
Everything there can be downloaded for free. But it's recommended to create a free account to see all available [models](https://civitai.com/models).  
***The new Stable Diffusion based **version 1.1** Apps come with a button allowing you to access Civitai directly within the App.***  

- On the Civitai [models](https://civitai.com/models) page filter the displayed models at the top right corner *("Filters")* to display only **SD1.5** models and check *Checkpoints*, *All* and *SD1.5*.
- Select an image that represents best what you have in mind and click it.
- On the following page you can scroll through different pictures created with that model.
Above these images you see different versions of that model. Most likely the latest version is the newest and best one.
- Choose your desired version and press the *Download* Button right beside the *Create* Button to download the model.
- Put it into `.\pinokio\drive\drives\peers\d1704581225212\checkpoints` on your computer.

Back in Stable Diffusion WebUI click the blue refresh button at the top left corner beside the *models dropdown menu*.  
After that you can choose your model from that dropdown menu.  
Lower the size of the images you want to create to 512 x 512 up to 800 x 800 pixel. SD1.5 models are trained on 512px images. Sizes bigger than 800px would lead to errors, mutations, mirror effects or double objects. Common horizontal and vertical formats like 600 x 800 or 768 x 512 work as well.

## Troubleshooting

Visual Buildtools fails to install on Windows

If Visual Buildtools fails to install, it often happen to a partly preinstalled version.
There are 3 ways to fix this:

- 1.) Uninstalling Visual Studio
  *(This should only be done if Visual Studio isn't needed by any other program on your computer)*
  - a.) Start the Visual Studio Installer (You find it by typing "Visual" in the search field of your Windows taskbar)
  - b.) Once it opened, uninstall **all** old Visual Studio versions.
  - c.) Once finished, close the installer
  - d.) Run Pinokio and install your app again
  
1.) a.) Visual Studio Installer  
![1.) a.) Visual Studio Installer](Images/visual_taskbar.png "Visual Studio Installer")  

1.) b.) Uninstall old versions  
![1.) b.) Uninstall old versions](Images/visual_uninstall.png "Uninstall old versions")  

- 2.) Manually add Visual Buildtools to your existing Visual Studios version
  - a.) Start the Visual Studio Installer
  - b.) Click "Modify"
  - c.) Select "Desktop Development C++" and check all components marked in screenshot 2.) c.)
  - d.) Click the "Modify" button at the bottom right corner to install the Visual Buildtools

2.) b.) Modify your Visual Studio installation  
![2.) b.) Modify](Images/visual_modify.png "Modify")

2.) c.) Desktop Development C++ and Components  
![2.) c.) Components](Images/components.png "Components")

- 3.) Manually install Visual Buildtools
  - a.) Start the Visual Studio Installer
  - b.) Click the "Available" tab and choose "Visual Studio Community 2022" and click "Install"
  - c.) Choose Desktop Development C++ and select all the components marked in screenshot 2.) c.)
  - d.) Click the "Install" button at the bottom right corner to install the Visual Buildtools

3.) b.) Available Tab![3.) b.) Available Tab](Images/available.png "Available Tab")

## Requirements (not verified)

### Stable Diffusion

- **Supported Systems**:

  - Window, Linux - NVIDIA, AMD, CPU
  - Apple (Silicon) - MPS
  - Intel Mac - CPU

- **Minimal Requirements**:

  - Stable Diffusion SD1.5 Models: NVIDIA 4GB VRAM, 16GB RAM  
  - Stable Diffusion SDXL Models: NVIDIA 8GB VRAM, 24 RAM

### Fooocus

- See [Fooocus Minimal Requirements](https://github.com/lllyasviel/Fooocus?tab=readme-ov-file#minimal-requirement)

### ComfyUI

- **Supported Systems**:

  - Window, Linux - NVIDIA, AMD, CPU
  - Apple (Silicon) - MPS
  - Intel Mac - CPU

- **Minimal Requirements**:

  - ComfyUI - SD1.5 Models: NVIDIA 4GB VRAM, 16GB RAM  
  - ComfyUI - SDXL Models: NVIDIA 8GB VRAM, 24 RAM

### InstantID

- **Supported Systems**:

  - Window, Linux - NVIDIA

- **Minimal Requirements**:

  - NVIDIA 12 GB VRAM

### IP-Adapter-FaceID

- **Supported Systems**:

  - Window, Linux - NVIDIA

- **Minimal Requirement**:

  - NVIDIA 8 GB VRAM

### Video2Densepose

- **Supported Systems**:

  - Window, Linux - NVIDIA only

- **Minimal Requirements**:

  - NVIDIA 8 GB VRAM

### Audio Gradio

- **Supported Systems**:

  - Window, Linux - NVIDIA only

- **Minimal Requirements**:

  - NVIDIA 8GB VRAM

### Moore-AnimateAnyone / Moore-AnimateAnyone-Mini

- **Supported Systems**:

  - Window, Linux - NVIDIA only

- **Minimal Requirements**:

  - NVIDIA 12 GB VRAM
