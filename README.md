# Gigabyte-Z590i-Aorus-Ultra-OC8.4-Monterey

Within this repository I share my Hackintosh EFI for my newest build based on Intels Tager lake 10th Gen CPU.

<p align="center">
  <img src="ScreenShot/MacOs Gpu Info Screen Shot 2022-10-11 at 6.52.10 PM.png" width="100%" align=center alt="Z590i and 10100F running macOS Monterey">
</p>

# Hardware used in this build:

- CPU: Intel i3-10100F
- Board: Gigabyte Z590i Aorus Ultra
  - Audio: Realtek ALC1220-VB (Not Working)
  - 1 x 2.5GBase-T (Intel I225-V)
  - 1 x USB Type-C® port on the back panel, with USB 3.2 Gen 2x2 support
  - 1 x USB Type-C® port with USB 3.2 Gen 1 support, available through the internal USB header
  - 3 x USB 3.2 Gen 2 Type-A ports (red) on the back pane
  - 4 x USB 3.2 Gen 1 ports (2 ports on the back panel, 2 ports available through the internal USB header)
  - 2 x USB 2.0/1.1 ports on the back panel
  - 2x m.2 Slots
- RAM: 16GB x 2 = 32GB Crucial 3200Mhz DDR4 CL22
- GPU: AMD Radeon RX 470
- Wifi/BT: Intel AX200
- SSDs: 
    1x 1TB WDC WDS100T2B0C-00PXH0 M.2 MNVe SSD

# What is working:
- Except for audio, everything works, including sleep.
- USB-ports. Have created my custom USB port mapping with USBMap.command

# What is not working:
- Audio: Realtek ALC1220-VB

# MOBO Layout

<p align="center">
  <img src="ScreenShot/Mobo_Layout Screen Shot 2022-10-11 at 7.38.02 PM.png" width="100%" align=center alt="MOBO Layout Z590i Aorus Ultra">
</p>
<p align="center">
  <img src="ScreenShot/Mobo_Rear Screen Shot 2022-10-11 at 7.35.45 PM.png" width="100%" align=center alt="MOBO Rear Back Panel Z590i Aorus Ultra">
</p>

# USB Port Mapping

<p align="center">
  <img src="ScreenShot/USB Port Map Screen Shot 2022-10-11 at 7.30.38 PM.png" width="100%" align=center alt="USB Port Mapping Z590i Aorus Ultra">
</p>

# For Intel Wi-Fi 6 AX200 working

To make Intel Wifi and BT always work, download the latest version of Helli Port from the link below, and set it to start automatically when you log in to Users & Groups.

https://github.com/OpenIntelWireless/HeliPort#download

<p align="center">
  <img src="ScreenShot/Helli Port Screen Shot 2022-10-11 at 8.15.26 PM.png" width="100%" align=center alt="Helli Port Auto Running Set Z590i Aorus Ultra">
</p>


# Kext List

<p align="center">
  <img src="ScreenShot/Kext List Screen Shot 2022-10-11 at 7.28.07 PM.png" width="100%" align=center alt="Kext List Z590i Aorus Ultra">
</p>
<p align="center">
  <img src="ScreenShot/Kext Version Screen Shot 2022-10-11 at 7.31.20 PM.png" width="100%" align=center alt="Major Kext Version Z590i Aorus Ultra">
</p>


# BIOS-settings:
- Current BIOS version: F3
- **Load optimized defaults**
- Set **Above 4G Decoding** to Enabled
- Set **Legacy USB Support** to Disabled
- Set **Intel VT-D** to Enabled (DisableIOMapper is disabled, AppleVTD should be working)
- Set **Secure Boot** to Disabled
- Set **Windows 10 Features to Other OS
- Set **CSM Support to Disabled

<p align="center">
  <img src="BIOS_Settings/221011114438 copy.png" width="100%" align=center alt="BIOS settings #1">
  <img src="BIOS_Settings/221011114455 copy.png" width="100%" align=center alt="BIOS settings #2">
  <img src="BIOS_Settings/221011114512 copy.png" width="100%" align=center alt="BIOS settings #3">
  <img src="BIOS_Settings/221011114529 copy.png" width="100%" align=center alt="BIOS settings #4">
  <img src="BIOS_Settings/221011114550 copy.png" width="100%" align=center alt="BIOS settings #5">
</p>

# Credits:

- [SchmockLord](https://github.com/SchmockLord/Gigabyte-Z590i-Vision-D-11900k) Your Z590i Vision D config was very helpful!
- [Dortania](https://github.com/dortania) for this great OpenCore Desktop Guide
- [headkaze](https://github.com/headkaze) for Hackintool and our productive conversations :)
- [OpenCore project](https://github.com/OpenCorePkg) for this great bootloader
