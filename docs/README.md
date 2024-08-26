# Remote File Sync

![Remote File Sync Banner](https://katorymnd.com/tqc_images/vscode-remote-file-sync-screen-shot.png)

Welcome to the "Remote File Sync" extension for Visual Studio Code. This extension provides seamless file synchronization between your local workspace and remote servers, leveraging FTP, SFTP, SSH, WebDAV, and Google Drive connections.

## Features

- **Remote File Synchronization:** Effortlessly sync files between your local workspace and remote servers.
- **Multiple Protocol Support:** Compatible with FTP, SFTP, SSH, WebDAV, and Google Drive.  
  ![Multiple Protocol Support](https://katorymnd.com/tqc_images/remote_file_sync.gif)
- **Connection Pooling:** Manage multiple connections efficiently without compromising performance.
- **Remote File Tree View:** Navigate remote directories and files without local cloning.
- **Sync Panel:** Real-time monitoring and management of file synchronization.

  ![Remote File Tree View](https://katorymnd.com/tqc_images/vscode-remote-file-tree.png)

> **Tip:** Use the Transfer Status to view updates on file synchronization dynamically.

## Requirements

Before using this extension, ensure you have:

- **VS Code**: Version 1.85.0 or newer.
- **Supported Protocols**: Confirm support for FTP, SFTP, SSH, WebDAV, or Google Drive API on your remote servers.

## Extension Settings

This extension contributes the following settings:

- `remotefilesync.openSyncPanel`: Opens the synchronization panel.
- `remotefilesync.transferStatus`: Displays the transfer status.

## Known Issues

- **Large File Handling:** Syncing very large files (>1GB) might impact performance. These files may also take longer to open.
- **Google Drive API Limits:** Be mindful of API rate limits when syncing a large number of files with Google Drive.

### Unsupported Files

Certain file types are not supported for synchronization, including:

**Executable Files:**

- `.exe`, `.dll`, `.so`

**Image Files:**

- `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.tif`

**Audio Files:**

- `.mp3`, `.wav`, `.aac`, `.flac`

**Video Files:**

- `.mp4`, `.avi`, `.mkv`, `.mov`, `.wmv`

**Document Files:**

- `.pdf`, `.doc`, `.docx`, `.ppt`, `.pptx`, `.xls`, `.xlsx`

**Compressed Files:**

- `.zip`, `.rar`, `.tar`, `.gz`

**Disk Image Files:**

- `.iso`, `.img`, `.dmg`

## Tutorials and Guides

Explore these resources to get started and make the most of Remote File Sync:

- [Getting Started with Remote File Sync](https://katorymnd.com/article/getting-started-with-remote-file-sync-installation-and-setup)
- [Configuring FTP, SFTP, SSH, and WebDAV](https://katorymnd.com/article/configuring-ftp-sftp-ssh-webdav-in-remote-file-sync)
  - [Setting up Google Drive](https://katorymnd.com/article/setting-up-google-drive-in-remote-file-sync-for-vs-code)
- [Using the Sync Panel](https://katorymnd.com/article/managing-remote-files-and-folders-in-vs-code-tree-view)
- [Common Troubleshooting Tips](https://katorymnd.com/article/common-troubleshooting-tips-for-remote-file-sync-for-vscode)

## Release Notes

### 0.0.1 - 0.0.4

- Initial releases: Core features like multi-protocol support and remote file tree view introduced.

### 1.0.1

- Synchronization panel display issues fixed.
- Enhanced stability for file synchronization.

### 1.1.1 - 1.3.4

- Enhanced configurations for FTP, SFTP, SSH, WebDAV, and Google Drive.
- Improved file transfer performance and synchronization.
- Bug fixes and documentation updates for better user guidance.

---

**Enjoy using Remote File Sync!**
