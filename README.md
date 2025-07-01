# L380 Clover
<p align="center">
  <img src="https://github.com/user-attachments/assets/ed0a3865-b22c-4789-9b06-f363a8ef57e9" alt="L380 EFI" width="600"/>
</p>

<!-- Badges -->
<p>
  <img src="https://img.shields.io/badge/macOS-Big%20Sur-red" />
  <img src="https://img.shields.io/badge/macOS-Monterey-pink" />
  <img src="https://img.shields.io/badge/macOS-Ventura-orange" />
  <img src="https://img.shields.io/badge/macOS-Sonoma-green" />
  <img src="https://img.shields.io/badge/license-MIT-purple" />
</p>

<p align="center">
  <strong>Status:</strong> Maintained<br>
  <strong>Version:</strong> 1.0
</p>

# ⚠️ Disclaimer
This guide is only for the Lenovo ThinkPad T480. I am NOT responsible for any harm you cause to your device. This guide is provided "as-is" and all steps taken are done at your own risk.

# Introduction
This EFI is made with Clover and it works for Ventura and Sonoma.

[Download HeliPort -->](https://github.com/OpenIntelWireless/HeliPort/releases/download/v1.5.0/HeliPort.dmg)

<details>
  <summary>💻 My Hardware</summary>
  
| Category  | Component                   |
|-----------|-----------------------------|
| CPU       | Intel Core i5-8350U          |
| GPU       | Intel UHD Graphics 620       |
| SSD       | Intel 256GB M.2 SSD          |
| Memory    | 16GB DDR4 2400Mhz            |
| Camera    | 720p Camera                  |
| WiFi & BT | Intel 18265 Wifi (HeliPort)  |

</details>

<details>
  <summary>📸 Photos</summary>
  
  ![P7010069](https://github.com/user-attachments/assets/5e346b60-59d2-4c5d-bf8d-dd354759a186)

</details>

<details>
  <summary>🔧 Requirements</summary>

  - Lenovo ThinkPad L380  
  - 32GB Flash Drive  
  - Windows PC with Python  
  - An internet connection  
  - MiniTool Partition Wizard  
  - Balena Etcher  
  - [Sonoma](https://www.mediafire.com/file/8eq9rjvf9ef2xju/Olarila+Sonoma+14.7.5.raw/file)  
  - [Ventura](https://www.mediafire.com/file/9g0bfwjsaffo925/Olarila+Ventura+13.7.6+22H625.raw/file)

</details>

<details>
  <summary>💾 How to make USB</summary>

  1. Flash the `.raw` file (Sonoma or Ventura) to your USB drive using **Balena Etcher**.  
  2. Open **MiniTool Partition Wizard**.  
  3. Right-click the 200MB EFI partition on the USB and select **"Assign letter"**.  
  4. Download and unzip this repository.  
  5. Delete all existing files from the USB's EFI partition.  
  6. Copy the `EFI` folder from the repo into the USB’s EFI partition.

</details>

<details>
  <summary>🛠️ BIOS Settings</summary>

  Make sure the following settings are adjusted in your BIOS:

  - **Disable** Secure Boot  
  - **Disable** TPM (Trusted Platform Module)  
  - **Disable** Intel SGX (if available)  
  - **Enable** USB Boot  
  - **Enable** UEFI Boot Mode  
  - Set **SATA Controller Mode** to AHCI  
  - **Disable** Fast Boot  
  - Enable **Virtualization** (optional, for macOS performance)  

</details>
