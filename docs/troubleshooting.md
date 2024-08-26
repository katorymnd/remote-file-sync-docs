# Troubleshooting Guide for Remote File Sync Extension

This section provides solutions to common problems you might encounter while using the Remote File Sync extension in Visual Studio Code. If your issue is not covered here, please refer to the [official site](https://katorymnd.com/vscode-remote-file-sync) or contact support.

## Common Issues and Solutions

### 1. **Connection Issues**

**Problem:** Unable to connect to the remote server.

**Possible Causes:**

- Incorrect protocol, hostname, port, or authentication details.
- Firewall or network restrictions blocking the connection.

**Solutions:**

- Double-check the connection details in the Remote File Sync panel.
- Verify that the server is online and accessible from your network.
- Ensure that the correct port is being used for the protocol (e.g., 22 for SFTP/SSH, 21 for FTP).
- If using an SSH key, ensure that the key path is correct and the key has the appropriate permissions.

### 2. **Authentication Failed**

**Problem:** Authentication fails when attempting to connect to the remote server.

**Possible Causes:**

- Incorrect username or password.
- Invalid SSH key or passphrase.
- Server-side restrictions (e.g., account locked, two-factor authentication).

**Solutions:**

- Re-enter the username and password, ensuring they are correct.
- If using an SSH key, make sure the key is valid and the passphrase (if required) is correctly entered.
- Check if the server requires additional authentication methods (like two-factor authentication) and configure accordingly.

### 3. **File Sync Issues**

**Problem:** Files are not syncing between the local machine and the remote server.

**Possible Causes:**

- Network interruption during the sync process.
- File path conflicts or permissions issues.

**Solutions:**

- Retry the sync operation to rule out temporary network issues.
- Ensure that you have the necessary permissions to read and write to the target directories.

### 4. **Slow Sync Performance**

**Problem:** Syncing files is taking longer than expected.

**Possible Causes:**

- Large file sizes or a large number of files being synced.
- Network bandwidth limitations.
- Server performance issues.

**Solutions:**

- Break down the sync operation into smaller batches, syncing a few files at a time.
- Check your network connection speed and try syncing during off-peak hours.
- Consider compressing large files before syncing or using a different protocol that may be faster.

### 5. **Permission Denied Errors**

**Problem:** Receiving "Permission Denied" errors when accessing or modifying files on the remote server.

**Possible Causes:**

- Insufficient permissions for the user account being used.
- Server-side restrictions on certain directories or files.
- Incorrect file or directory ownership on the server.

**Solutions:**

- Ensure your user account has the necessary permissions to access or modify the files.
- Contact your server administrator to verify permissions and ownership settings.
- Try running the sync operation as a different user with elevated privileges if possible.

### 6. **Unexpected Disconnections**

**Problem:** Connection to the remote server is unexpectedly dropped during a sync operation.

**Possible Causes:**

- Network instability or interruptions.
- Server-side timeout settings.
- Overloaded server or client machine.

**Solutions:**

- Check your network connection and ensure it is stable.
- Increase the timeout settings on the server, if possible.
- Reduce the load on your machine by closing unnecessary applications, or on the server by scheduling sync operations during off-peak hours.

## Advanced Troubleshooting

### Logging and Debugging

If you're still encountering issues, enabling detailed logging and using the developer debug tools can help diagnose the problem:

1. **Open Developer Tools:**

   - **Using the Command Palette:**
     - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS) to open the Command Palette.
     - Type `Developer: Toggle Developer Tools` and press `Enter`.
   - **Using a Keyboard Shortcut:**
     - On Windows/Linux: Press `Ctrl+Shift+I`.
     - On macOS: Press `Cmd+Option+I`.
   - **Using the Menu Bar:**
     - Click on the `Help` menu in the top bar.
     - Select `Toggle Developer Tools`.

2. **Reproduce the Issue:**

   - With the Developer Tools open and Verbose Logging enabled, reproduce the issue you’re encountering.
   - Check the **Console** tab in the Developer Tools for any error messages, warnings, or other relevant output that might help you understand what’s going wrong.

3. **Review and Analyze the Logs:**

   - The **Console** in the Developer Tools will display detailed logs, including any errors or warnings related to the Remote File Sync extension.
   - Look for any specific error messages or clues that could indicate the source of the problem.

4. **Take Action Based on the Logs:**
   - Use the information gathered from the logs to troubleshoot the issue.
   - If necessary, consult the extension’s documentation or support resources.

### Reinstalling the Extension

If all else fails, consider reinstalling the Remote File Sync extension:

1. Uninstall the extension from Visual Studio Code.
2. Restart Visual Studio Code.
3. Reinstall the extension from the marketplace.

## Getting Help

If the above solutions do not resolve your issue, consider the following options:

- **Community Support:** Visit forums or community platforms related to Visual Studio Code.
- **GitHub Issues:** If you believe you've encountered a bug, report it on the extension's GitHub repository by creating an issue [here](https://github.com/katorymnd/remote-file-sync-docs/issues).

- **Professional Support:** [Contact](https://katorymnd.com/contact-us) the extension developer or a professional for in-depth assistance.
