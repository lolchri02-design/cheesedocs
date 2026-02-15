# Rust - Rift

**Step 1: Installation**

**Preparing Your USB Drive**

1. Plug your USB drive into an available USB port on your computer
2. Press `Win + E` to open File Explorer and locate your USB drive under “This PC” or “My Computer”
3. Right-click on your USB drive and select **Format** from the dropdown menu

<figure><img src="https://3306193673-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F96BlnJqlAff52E9CJtGq%2Fuploads%2FsIdYpdWGWVDtJWTPzpvQ%2Fimage.png?alt=media&#x26;token=265e6b3f-774b-467a-9cc5-80eac0cbeebd" alt=""><figcaption></figcaption></figure>

4. In the Format window: Choose **FAT32** under the “File System” dropdown. Optionally, set a name for your drive in the “Volume Label” field
5. If you want a faster process, check the box for **Quick Format.** Leave it unchecked for a more thorough format
6. Click the **Start** button to begin the formatting process. A warning will pop up informing you that all data on the USB will be erased—ensure you’ve backed up important files
7. The format process will only take a few moments. Once finished, you’ll see a confirmation message

**Important Notes**

1. Formatting will erase all data on the USB drive. Ensure you back up important files before proceeding
2. If your USB drive is larger than 32GB, Windows may not offer FAT32 as an option. In this case, you can use third-party tools like Rufus or GUIFormat to format it

**Installing EFI Bootloader on USB**

1. Open your web browser and navigate to the download link: [Loader](https://user.mempatch.com/)
2. Press on Sign up to create a account with your license key or login if you already have made your account
3. After you logged in you press on the "Download EFI" button
4. The file will automatically start downloading. Once the download is complete, locate the `.zip` file in your Downloads folder or the specified download location
5. Right-click the downloaded `.zip` file and select **Extract All** or use a program like **7-Zip** to extract the contents
6. Choose your USB drive as the destination folder for the extraction. For example, if your USB drive is labeled "D:", extract the files directly to `D:\`&#x20;
7. Ensure the extracted contents are placed in the following folder structure: **D:\EFI\Boot\bootx64.efi**

<figure><img src="https://3306193673-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F96BlnJqlAff52E9CJtGq%2Fuploads%2FucZpP6WgJI4X1JgjFcbk%2Fimage.png?alt=media&#x26;token=b7d11bc4-0a62-45cf-9b0c-2d994731af1d" alt=""><figcaption></figcaption></figure>

<figure><img src="https://3306193673-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F96BlnJqlAff52E9CJtGq%2Fuploads%2FSnTYMqNgW7flv003EW5o%2Fimage.png?alt=media&#x26;token=a63c0700-8b9f-4311-b54d-f9d33ff11309" alt=""><figcaption></figcaption></figure>

**Booting from USB Drive**

Method 1:

1. Restart your Computer
2. Hold the Shift Key while restarting your Computer
3. Select the Boot Device

<figure><img src="https://3306193673-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F96BlnJqlAff52E9CJtGq%2Fuploads%2FANmSXglXgA9nge7tws2E%2Fimage.png?alt=media&#x26;token=daebd0a4-63d7-44d2-b092-f324c92d7e8b" alt=""><figcaption></figcaption></figure>

4. Choose your USB Drive from the list of available boot devices
5. Your computer will boot from the USB Drive, and EFI Bootloader will load.

Method 2:

1. Restart your Computer
2. Enter BIOS/UEFI Settings
3. Navigate to the Boot Menu
4. Change the Boot Order ➔ Move your USB drive to the top of the list

<figure><img src="https://3306193673-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F96BlnJqlAff52E9CJtGq%2Fuploads%2FU3B9hiNH7CegZFINCAwR%2Fimage.png?alt=media&#x26;token=30789065-ebdb-4855-9cd2-e201a8163bf4" alt=""><figcaption></figcaption></figure>

5. Save your changes and exit BIOS/UEFI
6. Your computer will now boot from the USB drive automatically, and the EFI Bootloader will load

**Step 2: Injecting**

1. Open your web browser and go to the following link: [Loader](https://user.mempatch.com/)
2. Press on Sign up and create a account with your license key or login if you already have made your account
3. After you logged in you press on the "Download Loader" button
4. Once the download is complete you open the loader as admin
5. Log in with your username and password you just created on this [website](https://user.mempatch.com/)
6. Press inject and wait for the loader to fully close
7. After the loader has close, open the game and follow the instructions from the message box
