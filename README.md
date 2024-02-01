# Pinokio Wiki

- [Pinokio Wiki](#pinokio-wiki)
  - [General](#general)
    - [Change the location where Apps are downloaded and installed (Home)](#change-the-location-where-apps-are-downloaded-and-installed-home)
    - [Install Apps with Pinokio](#install-apps-with-pinokio)
    - [Delete installed Apps](#delete-installed-apps)
    - [Upgrade Pinokio](#upgrade-pinokio)
    - [Uninstall Pinokio](#uninstall-pinokio)
  - [Pinokio](#pinokio)
    - [Home Screen](#home-screen)
    - [Settings](#settings)
    - [Discover Page](#discover-page)
    - [Application screen](#application-screen)
      - [Launching the App](#launching-the-app)
      - [Terminal](#terminal)
      - [Update, Reinstall and Factory Reset](#update-reinstall-and-factory-reset)
      - [Files](#files)
  - [Applications](#applications)
    - [Stable Diffusion Models](#stable-diffusion-models)
    - [Download different models for Stable Diffusion, Fooocus and ComfyUI](#download-different-models-for-stable-diffusion-fooocus-and-comfyui)
  - [Requirements](#requirements)
    - [Stable Diffusion](#stable-diffusion)
      - [**Supported Systems**](#supported-systems)
      - [**Minimal Requirements**](#minimal-requirements)
    - [Fooocus](#fooocus)
    - [ComfyUI](#comfyui)
      - [**Supported Systems**](#supported-systems-1)
      - [**Minimal Requirements**](#minimal-requirements-1)
    - [InstantID](#instantid)
      - [**Supported Systems**](#supported-systems-2)
      - [**Minimal Requirements**](#minimal-requirements-2)
    - [IP-Adapter-FaceID](#ip-adapter-faceid)
      - [**Supported Systems**](#supported-systems-3)
      - [**Minimal Requirement**](#minimal-requirement)

## General

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

#### Update, Reinstall and Factory Reset

- To update an App, close it if running and click the **Update** button. *This will update the app to the latest version.*  
- To reinstall an App, close it if running and click **Reinstall**. *This will reinstall the App without deleting any data or creations.*  
- A **Factory Reset** will delete the App but not the Pinokio scripts. *It will still be displayed on the Pinokio home screen and can be reinstalled any time.*  
***Note:*** Not all Apps come with an Update, Reinstall or Factory Reset button

#### Files

The Files button leads to the Pinokio scripts, App-folder and subfolders and all containing files. It is even possible to edit and save these files within Pinokio, although it's recommended to use an appropriate Editor or IDE for that purpose.  
This should only be done if stringently required and done with cautious since a mistake can easily break the App.  
*It's always wise to make a backup of the original files before modifying them.*

## Applications

### Stable Diffusion Models

### Download different models for Stable Diffusion, Fooocus and ComfyUI

The best place to download finetuned **SD1.5**, **SD2.1** and **SDXL** Models is [Civitai](https://civitai.com).
Everything there can be downloaded for free. But it's recommended to create a free account to see all available [models](https://civitai.com/models).  
Filter the displayed models and tools at the top right corner above the images (Symbol right beside the text *Month*). To display only **SD1.5** models click *Checkpoints*, *All* and *SD1.5*.
Select an image that represents best what you have in mind and click it.

On the following page you can scroll through different pics made with that model.
Above these pics you see different versions. Most likely the latest version is the newest and best one.
Press the *Download* Button right beside the *Create* Button to download your desired model.
Download it into:  `.\pinokio\drive\drives\peers\d1704581225212\checkpoints`

Back in Stable Diffusion WebUI click the blue refresh button at the top left corner beside the *models dropdown menu*.  
After that you can choose your model from that dropdown menu.

## Requirements

### Stable Diffusion

#### **Supported Systems**

- Window, Linux - NVIDIA, AMD, CPU
- Apple (Silicon) - MPS
- Intel Mac - CPU

#### **Minimal Requirements**

- Stable Diffusion SD1.5 Models: NVIDIA 4GB VRAM, 16GB RAM  
- Stable Diffusion SDXL Models: NVIDIA 8GB VRAM, 24 RAM

### Fooocus

- See [Fooocus Minimal Requirements](https://github.com/lllyasviel/Fooocus?tab=readme-ov-file#minimal-requirement)

### ComfyUI

#### **Supported Systems**

- Window, Linux - NVIDIA, AMD, CPU
- Apple (Silicon) - MPS
- Intel Mac - CPU

#### **Minimal Requirements**

- ComfyUI - SD1.5 Models: NVIDIA 4GB VRAM, 16GB RAM  
- ComfyUI - SDXL Models: NVIDIA 8GB VRAM, 24 RAM

### InstantID

#### **Supported Systems**

- Window, Linux - NVIDIA

#### **Minimal Requirements**

- NVIDIA 12 GB VRAM

### IP-Adapter-FaceID

#### **Supported Systems**

- Window, Linux - NVIDIA

#### **Minimal Requirement**

- NVIDIA 8 GB VRAM
