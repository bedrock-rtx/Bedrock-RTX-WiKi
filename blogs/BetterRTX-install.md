---
tags: [guide, blog, installation]
---

[!badge variant="danger" text="#1"] [!badge variant="success" text="Author: 0x4a4b"]



# How to Run the BetterRTX Installer PowerShell Script

![BetterRTX On Logo](BetterRTXImages\BetterRTX_On.png)

## Prerequisites

1. **Windows Operating System**
2. **PowerShell**
3. **BetterRTX_Installer.zip** file
4. [**IOBit Unlocker**](https://www.iobit.com/en/iobit-unlocker.php) installed

## Downloading the Files

1. **From Discord:**
   - Navigate to the channel where the file is shared.
   - Click on the latest file to download `BetterRTX_Installer.zip`. <br>
     [!button variant="success" text="Minecraft RTX Discord Server"](https://discord.gg/minecraft-rtx-691547840463241267)<br><br>

   <!-- ![Download from Discord](BetterRTXImages/Download+from+Discord.webp) -->

2. **From GitHub:**
   - Go to the repository containing `BetterRTX_Installer.zip`.
   - Click on the file to download it. <br>
     [!button variant="success" text="Better RTX Repository"](https://github.com/BetterRTX/BetterRTX-Installer/releases/tag/v1.1.3)<br><br>

   <!-- ![Download from GitHub](BetterRTXImages/Download+from+GitHub.png) -->

## Extracting the ZIP File

1. Locate the downloaded `BetterRTX_Installer.zip` file.
2. Right-click on the file and select "Extract All".
3. Choose a destination folder and click "Extract".

## Installing IOBit Unlocker

1. Download **IOBit Unlocker** from the [official website](https://www.iobit.com/en/iobit-unlocker.php).
2. Run the installer and follow the prompts to complete the installation.

## Setting Up PowerShell Execution Policy

### Main Method

1. Open PowerShell with administrative privileges:
   - Click on the Start menu, type `PowerShell`.
   - Right-click on `Windows PowerShell` and select "Run as administrator".

   <!-- ![Run PowerShell as Admin](BetterRTXImages/Run+PowerShell+as+Admin.webp) -->

2. Run the following command to set the execution policy:
   ```powershell
   Set-ExecutionPolicy -Scope CurrentUser Unrestricted
   ```
   - Press `Y` and then `Enter` to confirm.

   <!-- ![Set Execution Policy](BetterRTXImages/Set+Execution+Policy.png) -->

3. Navigate to the folder where you extracted `BetterRTX_Installer.zip`.
4. Right-click on the `BetterRTX_Installer.ps1` file and select "Run with PowerShell".
   - Press `Y` if prompted.

   <!-- ![Run PowerShell Script](BetterRTXImages/Run+PowerShell+Script.png) -->

### Alternative Method

1. Open PowerShell with administrative privileges.
2. Run the following command to set the execution policy for the current process:
   ```powershell
   Set-ExecutionPolicy -Scope Process Bypass
   ```
   - Press `Y` to confirm.

   <!-- ![Set Execution Policy for Process](BetterRTXImages/Set+Execution+Policy+for+Process.png) -->

3. Navigate to the folder where you extracted `BetterRTX_Installer.zip`.
4. Right-click on the `BetterRTX_Installer.ps1` file and select "Copy as Path".

   <!-- ![Copy as Path](BetterRTXImages/Copy+as+Path.png) -->

5. In the PowerShell window, type a period `.` followed by a space, then paste the copied path:
   ```powershell
   . "C:\Path\to\BetterRTX_Installer.ps1"
   ```
   - Press `Enter` to run the script.

!!!Important
Better RTX is not a texture pack. It does not show in global resource packs. You need an RTX texture pack for this to work.
!!!

   <!-- ![Run Script with Path](BetterRTXImages/Run+Script+with+Path.png) -->

## Common Issues and Solutions

**Issue: PowerShell window closes immediately after opening**

**Solution:**
1. Ensure you run PowerShell with administrative privileges.
2. Verify the script is not being blocked by your antivirus.
3. Confirm the execution policy is set correctly (`Unrestricted` or `Bypass`).

**Issue: The Installer window says IOBit Unlocker not Installed**

**Solution:**
1. Ensure IOBit Unlocker is installed correctly.
2. If you changed the installation path, ensure the script points to the correct path.
