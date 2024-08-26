# Usage Guide for Remote File Sync Extension

This section will guide you through the usage of the Remote File Sync extension for Visual Studio Code, explaining how to synchronize your local files with remote servers efficiently.

## Step 1: Open the Remote File Sync Panel

After installing and configuring the extension, you can access the Remote File Sync panel:

1. Open Visual Studio Code.
2. Navigate to the sidebar on the left.
3. Click on the "Remote File Sync" icon to open the panel.

## Step 2: Set Up a New Connection

To start syncing files, you first need to set up a new connection to your remote server:

1. In the Remote File Sync panel, click on the `+` icon to add a new connection.
2. Fill in the required details:
   - **Protocol:** Select the protocol (FTP, SFTP, SSH, WebDAV, or Google Drive) based on your server.
   - **Host:** Enter the hostname or IP address of the remote server.
   - **Port:** Specify the port number (default is 22 for SFTP/SSH, 21 for FTP).
   - **Username:** Your username for the remote server.
   - **Password/Key:** Enter the password or provide the path to your SSH key.
3. Click `Connect` to store the connection details.

## Step 3: Configure the Extension

Once the extension is installed, you need to configure it to connect to your remote servers:

[![Remote File Sync](https://katorymnd.com/tqc_images/How-to-Sync-Filez.png)](https://www.youtube.com/watch?v=fJLxWZzPWqI)

## Step 4: Sync Files

After setting up the connection, you can start syncing files between your local machine and the remote server:

1. Select the connection from the list in the Remote File Sync panel.
2. Click on the `Latest Connection`.
3. Choose the direction of sync:
   - **Local to Remote:** Upload files from your local machine to the remote server.
   - **Remote to Local:** Download files from the remote server to your local machine.
4. Monitor the sync progress in the output panel.

## Step 5: Manage Files

You can also manage files directly from the Remote File Sync panel:

- **Upload:** Right-click on a file or folder in the local file tree and select `Upload`.
- **Download:** Right-click on a file or folder in the remote file tree and select `Download`.
- **Delete:** Right-click on a file or folder and select `Delete` to remove it from the remote server.
- **Rename:** Right-click on a file or folder and select `Rename`.

## Step 6: Troubleshooting

If you encounter issues while using the extension, refer to the [Troubleshooting Guide](troubleshooting.md) for common problems and solutions.
