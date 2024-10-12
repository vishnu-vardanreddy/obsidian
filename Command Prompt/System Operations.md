### **Free Up Temporary Files**

- **Windows:**
    
    1. Open **Disk Cleanup**: Press `Win + R`, type `cleanmgr`, and press `Enter`.
    2. Select the drive you want to clean up (usually `C:`).
    3. Check the boxes for **Temporary files**, **Recycle Bin**, and other unnecessary files.
    4. Click **OK**, then **Delete Files**.

To improve your system's performance using the Command Prompt on Windows, you can run the following commands:

### 1. **Clean Up Temporary Files**
```bash
del /q /f /s %TEMP%\*
```
This command deletes all files in the temporary folder.

### 2. **Clean Up the System**
```bash
cleanmgr /sagerun:1
```
This command runs the Disk Cleanup tool with predefined settings. To configure these settings:
   - Run `cleanmgr /sageset:1` first to choose the options you want (like temporary files, system cache, etc.).
   - Then, run `cleanmgr /sagerun:1` to perform the cleanup.

### 3. **Check and Repair System Files**
```bash
sfc /scannow
```
This command checks for and repairs corrupted system files.

### 4. **Optimize Drives (Defragment)**
```bash
defrag C: /O
```
This command optimizes the drive, improving access times and overall performance. Replace `C:` with the drive letter you want to optimize.

### 5. **Disable Startup Programs**
   - Use `msconfig` to open the System Configuration tool, where you can disable unnecessary startup programs.
```bash
msconfig
```

### 6. **Check and Remove Malware**
   - Use Windows Defender to perform a quick scan for malware:
```bash
MpCmdRun -Scan -ScanType 1
```

### 7. **View and Stop Resource-Intensive Processes**
```bash
tasklist
```
   - Use `tasklist` to view all running processes.
   - To stop a resource-intensive process, use:
```bash
taskkill /F /PID <ProcessID>
```
   - Replace `<ProcessID>` with the actual Process ID from the `tasklist`.

### 8. **Flush DNS Cache**
```bash
ipconfig /flushdns
```
This command clears the DNS cache, which can resolve network-related slowdowns.

### 9. **Disable Hibernate (Optional)**
   - Disabling hibernate can free up disk space, especially on SSDs:
```bash
powercfg -h off
```

### 10. **Release Unused RAM**
   - You can clear the standby list, which holds inactive memory:
```bash
echo off | clip
```

These commands should help clean up your system and improve its performance.