# Day 02

## Installing Kali Linux in Oracle VirtualBox

There are mainly 3 things required to install Kali Linux on a Windows host machine:

1. **Downloading Kali Linux VirtualBox Image**  
   [Kali Linux VirtualBox Image](https://cdimage.kali.org/kali-2025.2/kali-linux-2025.2-virtualbox-amd64.7z)
2. **Downloading Oracle VirtualBox**  
   It is a general-purpose full virtualization software.  
   [Oracle VirtualBox Download](https://download.virtualbox.org/virtualbox/7.1.12/VirtualBox-7.1.12-169651-Win.exe)
3. **Downloading 7-Zip**  
   It is a free and open-source file archiver with a high compression ratio, used to extract the downloaded zip file.  
   [7-Zip Download](https://www.7-zip.org/a/7z2500-x64.exe)

> **Note:** Make sure you have at least **10–15 GB** of free space on your storage.

---

## Step 1: Installing Oracle VirtualBox on Windows

1. Run the downloaded VirtualBox installer.
2. Click **"Yes"** to grant administrator privileges.
3. After the installer dialog box appears, click **"Next"**.
4. On the **"Custom Setup"** page, keep the default settings and click **"Next"**.  
   *(The installation path is displayed at the bottom-left of the dialog box.)*
5. When the **"Warning! Network Interface"** page appears, click **"Yes"**.
6. When the **"Missing Dependencies"** page appears, click **"Yes"**.
7. On the **"Ready to Install"** page, click **"Install"**.
8. After installation, click **"Finish"**. VirtualBox is now installed.

### Troubleshooting Issues During/After Installation

**Problem 1: Missing 'Microsoft Visual C++ 2015-2022 Redistributable (x64) - 14.44.35211'**  
- Download the required dependency: [vc_redist.x64.exe](https://aka.ms/vs/17/release/vc_redist.x64.exe)  
- Install it and relaunch the Oracle VirtualBox installer.  
- Follow **Step 1** again.

**Problem 2: AMD-V is disabled in the BIOS (or by the Host OS)**  
1. Reboot your system into BIOS.  
   - To enter BIOS, check your device model and search for the BIOS key.  
     Common keys:  
     - **Dell:** F2 or F12  
     - **Lenovo:** F2 or Fn + F2 (laptops), F1 (desktops), Novo button  
     - **Acer:** F2 or DEL  
     - **HP:** Esc or F10
2. Navigate to **Advanced Settings** and enable **Virtualization** or **SVM Mode**.

---

## Step 2: Installing 7-Zip Tool

1. Right-click the downloaded 7-Zip installer and select **"Run as Administrator"**.
2. When the installer dialog box appears, click **"Install"**.
3. After installation, click **"Close"**.

---

## Step 3: Extracting the Kali Linux VirtualBox Image

1. Go to the directory where you downloaded the Kali Linux VirtualBox image.
2. Right-click the zip file → **"Show more options"** → hover over **7-Zip** → select **"Extract Here"**.
3. Wait for extraction to complete. This may take a few minutes.

---

## Step 4: Loading the Kali Linux VirtualBox Image

1. (Optional) Create a **separate partition** (10–15 GB) to store Kali Linux.  
   [Guide: Create a Partition](https://www.youtube.com/watch?v=HGqo17dGk0E)
2. Copy the extracted Kali Linux VirtualBox image file to the new partition.
3. Open the folder. You’ll find two files:  
   - **VirtualBox Machine Definition (.vbox)**
   - **Virtual Disk Image (.vdi)**
4. Double-click the **VirtualBox Machine Definition** file. Oracle VirtualBox will open.
5. Click **"Start"** to boot the virtual machine.  
   *(The first boot may take some time.)*
6. Log in with:  
   - **Username:** `kali`  
   - **Password:** `kali`

---
