# AppImage-Quick-Launcher

Creates a GUI that lets you select which AppImage you want to run.

The idea of creating a sandbox/container for applications is a good development regarding security. The problem I encountered with AppImages was that every time I wanted to execute an AppImage, I had to navigate to its location to run it. This was becoming frustrating, so I created a script that generates a GUI to list all your AppImages, allowing you to select and run the desired one.

![AppImage-Quick-Launcher Screenshot](images/screenshot.png)

# Installation Guide

1. Place the `AppImage-Quick-Launcher` file in one of your `$PATH` directories, e.g., `/usr/bin/`.
2. Make the file executable:
    ```bash
    sudo chmod 700 /usr/bin/AppImage-Quick-Launcher
    ```

## Define Your Default AppImage Folder

In the file, change the `APPIMAGE_DIR` variable to point to the folder where you save your AppImages.

### Optional

Assign a shortcut key to your script. (I use Ubuntu, so here's how you can do it!)

1. Go to Settings.
2. On the left, select **Keyboard**.
3. Under **Keyboard Shortcuts**, select **View and Customize Shortcuts**.
4. Scroll down and select **Custom Shortcuts**.
5. Click **+** to add a new shortcut.
6. Enter the following details:
    - **Name**: Insert a name for this shortcut.
    - **Command**: `/usr/bin/AppImage-Quick-Launcher`
7. Click **Shortcut**.
8. You can now add your own shortcut key. This will launch the script.
