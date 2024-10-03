# Usage Guide for Remote File Sync Extension

[![Remote File Sync](https://katorymnd.com/tqc_images/How-to-Sync-Filez.png)](https://www.youtube.com/watch?v=fJLxWZzPWqI)

This section will guide you through the usage of the Remote File Sync extension for Visual Studio Code, explaining how to synchronize your local files with remote servers efficiently.

## Step 1: Open the Remote Files

After installing and configuring the extension, you can access the Remote Files like so:

1. Open Visual Studio Code and click on `Remote File Sync extension` icon.
2. Navigate to the sidebar on the left.
3. Click on the "**Open Sync Panel**" section to open the **File Synchronization** tab.

## Step 2: Set Up a New Connection

To start syncing files, you first need to set up a new connection to your remote server:

1. In the **File Synchronization** tab, use the dropdown menu to select your desired protocol. By default, the FTP protocol is selected, but you can choose from:
   - **FTP**
   - **SFTP**
   - **SSH**
   - **WebDAV**
   - **Google Drive**
2. Once you've selected the protocol, fill in the required details:
   - **Host:** Enter the hostname or IP address of the remote server.
   - **Port:** Specify the port number (default is 22 for SFTP/SSH, 21 for FTP).
   - **Username:** Enter your username for the remote server.
   - **Password/Key:** Enter the password or provide the path to your SSH key.
3. Click `Connect` to store the connection details.

After completing these steps, the connection will be saved, and you can begin syncing files with your chosen protocol.

## Step 3: Sync Files

After setting up the connection, you can start syncing files between your local machine and the remote server by following these steps:

1. By the **File Synchronization** tab saved connections. (Dont open the tab again).
2. Click on `Latest Connection` to select the most recently used connection
3. By your saved protocols, choose your desired connection protocol from the dropdown list:
   - **FTP**
   - **SFTP**
   - **SSH**
   - **WebDAV**
   - **Google Drive**
4. Click to connect. Once you see `FTP Connection to server initiated.` and `Connected to FTP server.` if your choice was FTP Protocol. Then click on `Remote Files` to display the recieved remote files.

## Step 4: Manage Files

Once all files are retrived by your selected protocol, you will be able see all remote files under `Remote Files`, navigate to any folder by clicking on it to display its files, as you do when viewing local files using vscode.

- **Right-click on Folder:** Right-click on a folder in the `Remote Files` file tree and you will be able to select and use `Upload to Server` any file(s) or folder,`Delete`, add `New File`, add `New folder`, also `Rename...` .

- **Right-click on File:** Right-click on a file in the `Remote Files` file tree and you will be able to select and use `Delete`, add also `Rename...` .

- **Click on File:** Depending on the supported file type, click on the file, and it will open in a new VS Code tab or window. Here, you can update the file and save it. Sometimes you might see this notice:

  ![Remote File Sync Overwrite](https://katorymnd.com/tqc_images/compare-save.png)

  Simply click the `overwrite` option. When the file is saved remotely, you will see the confirmation:

  ![Remote File Sync saved](https://katorymnd.com/tqc_images/save-success.png)

## Step 5: Troubleshooting

If you encounter issues while using the extension, refer to the [Troubleshooting Guide](troubleshooting.md) for common problems and solutions.
