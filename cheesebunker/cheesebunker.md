# 🚧 Getting Started

### Disable all antivirus on your computer (No we are not trying to "hack" you) this is to allow loaders to run properly <a href="#disable-all-antivirus-on-your-computer-no-we-are-not-trying-to-hack-you-this-is-to-allow-loaders-to" id="disable-all-antivirus-on-your-computer-no-we-are-not-trying-to-hack-you-this-is-to-allow-loaders-to"></a>

1. Go to your windows "Virus and Threat Protection" Settings - Turn off real time protection
2.  Download Dcontrol [here](https://drive.usercontent.google.com/download?id=1jxmKjN820qP_cLZLgbeBi-aP5DUbROle\&export=download\&authuser=0)

    1. Click the "Disable Windows Defender" Button if it works properly it should look like below:

    ![](https://team073.gitbook.io/~gitbook/image?url=https%3A%2F%2F1007964587-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FhVRvo5LSxJWykyo7Sd1t%252Fuploads%252Fgit-blob-5c8c02f055a2e40561f4440eea101c454569e935%252Fimage_2024-08-20_083859552.png%3Falt%3Dmedia\&width=768\&dpr=4\&quality=100\&sign=202f1d4c\&sv=2)
3. Uninstall any 3rd party Antivirus (Norton, Total AV, Aura, BitDefender, McAfee, etc )

![](https://team073.gitbook.io/~gitbook/image?url=https%3A%2F%2F1007964587-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FhVRvo5LSxJWykyo7Sd1t%252Fuploads%252Fk62zTLiQD3QAi6TsghlE%252Fins.webp%3Falt%3Dmedia%26token%3D73124cf1-8576-4f40-a8b7-685228818152\&width=768\&dpr=4\&quality=100\&sign=5cff29a3\&sv=2)

### Virtualization <a href="#virtualization" id="virtualization"></a>

This page will help you to turn on virtualization in BIOS.

* Firstly, let's check if you have Virtualization on already. You can do so by opening Task Manager, then opening the performance tab.

![](https://idupegtas-organization.gitbook.io/~gitbook/image?url=https%3A%2F%2F2627785555-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F4wPsTeF1bcWTyN6pIROn%252Fuploads%252FF0UKswyYPYc792BwuUPX%252Fvirtual.png%3Falt%3Dmedia%26token%3D938a9df1-3a4d-4975-97bd-326ae8456a62\&width=768\&dpr=4\&quality=100\&sign=a51bc3c7\&sv=1)

* If your Virtualization says it's disabled, then lets head to your BIOS to turn it on. If it is enabled, then you can go ahead and skip to the next step.
*   **Virtualization for Intel Users:**

    Once in your BIOS settings, head over to the advanced tab and select CPU configuration.

    From there, go to Intel Virtualization Technology, and enable it. Your BIOS settings may differ depending on your manufacturer. Do not exit BIOS, as the next step requires you to be in it.

![](https://idupegtas-organization.gitbook.io/~gitbook/image?url=https%3A%2F%2F2627785555-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F4wPsTeF1bcWTyN6pIROn%252Fuploads%252FbnsETZLPoTGttNCXjcEa%252Fimage%2520%281%29.png%3Falt%3Dmedia%26token%3De2e023c3-b0ae-438a-83f8-3ddeeda625c9\&width=768\&dpr=4\&quality=100\&sign=70d574b1\&sv=1)

* **Virtualization for AMD Users:**

Once in your BIOS settings, head over to the advanced tab and select CPU configuration.

From there, go to SVM Mode, and enable it. Your BIOS settings may differ depending on your manufacturer. Do not exit BIOS, as the next step requires you to be in it.

### Secure Boot <a href="#secure-boot" id="secure-boot"></a>

{% hint style="danger" %}
For Valorant you do not need to disable secure boot, and you don't need vanguard uninstalled obviously. Just make sure to have Memory Integrity ON. then follow through the rest of the steps below
{% endhint %}

This page explains how to disable Secure Boot.

* Find the **Secure Boot** setting in your BIOS menu. If possible, set it to **Disabled**. This option is usually in either the **Security** tab, the **Boot** tab, or the **Authentication** tab.
* Save changes and exit. The PC reboots.
* In some cases, you may need to change other settings in the firmware, such as enabling a Compatibility Support Module (CSM) to support legacy BIOS operating systems. To use a CSM, you may also need to reformat the hard drive using the Master Boot Record (MBR) format, and then reinstall Windows. For more info, see [Windows Setup: Installing using the MBR or GPT partition style](https://learn.microsoft.com/en-us/windows-hardware/manufacture/desktop/windows-setup-installing-using-the-mbr-or-gpt-partition-style?view=windows-11).

### Hyper-V <a href="#hyper-v" id="hyper-v"></a>

This page will help you turn off Hyper-V in Windows.

1. In order to turn off Hyper-V in Windows, we are going to start by opening a Windows Powershell as Admin. This can be done by typing powershell into your windows search, and pressing "Run as administrator" beside it.
2. Now that we have Powershell open, copy and paste the following lines of code separately, then press enter: `bcdedit /set hypervisorlaunchtype off Disable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V-All`
3. Getting an error that says "Disable-WindowsOptionalFeature : Feature name Microsoft-Hyper-V-All is unknown." on the above is completely normal, however, getting a success message is also normal. Once this is done, restart your PC for the changes to take affect.

### Antivirus <a href="#antivirus" id="antivirus"></a>

{% hint style="danger" %}
For Valorant you do not need to disable secure boot, and you don't need vanguard uninstalled obviously. Just make sure to have Memory Integrity ON. then follow through the rest of the steps below
{% endhint %}

This page will help you disable your Antivirus Software in Windows.

**3rd party Antivirus:**

* Press windows key, type "Add or remove program", and in that list of programs, delete any that are antivirus. Here's a list of them: [https://bestantivirus.com/antivirus-companies.html](https://bestantivirus.com/antivirus-companies.html)

**Windows Security:**

* You can use Defender Control to disable Windows Security if you are on Windows 10:
*   [https://www.sordum.org/downloads/?st-defender-control](https://www.sordum.org/downloads/?st-defender-control)

    Password: sordum

![](https://idupegtas-organization.gitbook.io/~gitbook/image?url=https%3A%2F%2F2627785555-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F4wPsTeF1bcWTyN6pIROn%252Fuploads%252FDx6h0zhhMjXCh3woquym%252Fimage%2520%282%29.png%3Falt%3Dmedia%26token%3D6e09ecbf-c56a-45fc-8f87-d18d455c570b\&width=768\&dpr=4\&quality=100\&sign=a207bb6\&sv=1)

If you aren't on Windows 10 then do the following:

* Disable Real-Time Protection in Windows Security
  * You can also add exclusions on the bottom of the page to keep your loaders from getting deleted occasionally.
* If you get "An error occurred while trying to load the driver, please contact support." or a DRIVER &#x30;_&#x78;_&#x31;001-&#x30;_&#x78;_&#x31;003 error, uninstall the latest security update installed on your computer.

![](https://idupegtas-organization.gitbook.io/~gitbook/image?url=https%3A%2F%2F2627785555-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F4wPsTeF1bcWTyN6pIROn%252Fuploads%252Fvnxl3de2YcM0SIDoLUQX%252FScreenshot%25202024-07-18%2520183904.png%3Falt%3Dmedia%26token%3D563df039-1202-400d-9a61-fb24a61d781a\&width=768\&dpr=4\&quality=100\&sign=7be846d4\&sv=1)

### Anticheat <a href="#anticheat" id="anticheat"></a>

This page describes how to disable all anti-cheat software on your PC.

1. Disable [Fast-Boot](https://support.lenovo.com/us/en/solutions/ht513773-how-to-enable-or-disable-fast-startup-on-windows-11)
2. Open your system configuration (press Win+R -> type msconfig -> press enter)
3. Navigate to the "Services" tab
4. Check the "Hide all Microsoft services" box
5. Search the list for: Easy Anti-Cheat, BattlEye etc.
6. Uncheck the services that are anti-cheats
7. Click apply
8. Restart your PC

**Valorant (Riot Vanguard), ESEA, FaceIT:**

{% hint style="danger" %}
For Valorant you do not need to disable secure boot, and you don't need vanguard uninstalled obviously. Just make sure to have Memory Integrity ON. then follow through the rest of the steps below
{% endhint %}

For Riot Vanguard, ESEA, and FaceIT, you will need to go into your Apps & Programs in Windows settings to uninstall it fully. They are very invasive and will block the driver from loading.

![](https://idupegtas-organization.gitbook.io/~gitbook/image?url=https%3A%2F%2F2627785555-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F4wPsTeF1bcWTyN6pIROn%252Fuploads%252Ftl64gRNWkL6CfxhMs77P%252Fimage%2520%283%29.png%3Falt%3Dmedia%26token%3D22351528-16fd-49de-bbcf-6e0c899d39ad\&width=768\&dpr=4\&quality=100\&sign=72b84739\&sv=1)

### Memory Integrity <a href="#memory-integrity" id="memory-integrity"></a>

{% hint style="danger" %}
For Valorant you do not need to disable secure boot, and you don't need vanguard uninstalled obviously. Just make sure to have Memory Integrity ON. then follow through the rest of the steps below
{% endhint %}

This page will help you disable memory integrity in Windows.

Head to the main menu of Windows Security, then click on Device Security. Click Core Isolation Details, then turn off Memory Integrity. Restart your PC after making these changes.

![](https://idupegtas-organization.gitbook.io/~gitbook/image?url=https%3A%2F%2F2627785555-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F4wPsTeF1bcWTyN6pIROn%252Fuploads%252FJHSVOH4hfIM5Yv6rj83T%252FScreenshot%25202024-07-18%2520184135.png%3Falt%3Dmedia%26token%3D3eefc38f-f690-4372-ab25-5fe868e986f8\&width=768\&dpr=4\&quality=100\&sign=f898b5fd\&sv=1)

### Driver Blocklist <a href="#driver-blocklist" id="driver-blocklist"></a>

This page will help you disable the Vulnerable Driver Blocklist in Windows.

* If you are Windows 11 22H2, then we need to also turn off Core Isolation. Head back to the main menu of Windows Security, then click on Device Security. Click Core Isolation Details, then turn off Memory Integrity. Restart your PC after making these changes.
* Now you must make sure you don't have any 3rd Party Antivirus software active. Press your windows key, type "Add or remove program", and in that list of programs, delete any that are antivirus. Here's a list of them - [https://tinyurl.com/yyasj83u](https://tinyurl.com/yyasj83u)
* Disable the Vulnerable Driver Blocklist (Only Required for Windows 11 22H2)
  * Start by opening a Command Prompt as Admin. Once open, copy and paste the following line of code, then type "y" or "yes" to confirm the changes: `reg add HKLM\SYSTEM\CurrentControlSet\Control\CI\Config /v VulnerableDriverBlocklistEnable /t REG_DWORD /d 0x000000`
  * It may ask you to overwrite/create a new registry key, which you can also type "y" or "yes" to confirm that. Restart your PC after making these changes. or run the following as admin. [https://mega.nz/file/QccXBTbT#CNAjOjDm\_ThhiKOPnqsIEosgnqLym8mIEOfUUwbtc-k](https://mega.nz/file/QccXBTbT#CNAjOjDm_ThhiKOPnqsIEosgnqLym8mIEOfUUwbtc-k)

### C++ Redistributables <a href="#c-redistributables" id="c-redistributables"></a>

This page explains how to install the VC runtimes.

1. Download the [Visual C++ Redistributables](https://mega.nz/file/NFMSgBoT#OSTJy8rRG7FCoIzIVy7T4ZP80RcLCRFoG2uNhZLBUU4)
2. Run the VCRHyb64.exe
3. It will go through and install all redistributables for you, just wait for it to finish.
4. Restart your PC

![](https://idupegtas-organization.gitbook.io/~gitbook/image?url=https%3A%2F%2F2627785555-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F4wPsTeF1bcWTyN6pIROn%252Fuploads%252FciAaepx8kSJuSMDjbsug%252Fimage%2520%285%29.png%3Falt%3Dmedia%26token%3De8ad019f-8b1a-4fb1-a36b-09f871f4b9e2\&width=768\&dpr=4\&quality=100\&sign=3d1c34fd\&sv=1)
