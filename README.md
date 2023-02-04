<h1 align="center">我的Thinkpad X230 黑苹果EFI</h1>

<p align="center">
    <a href="https://www.apple.com/">
        <img src="https://img.shields.io/badge/Catalina-10.15.7-red.svg"/></a>
    <a href="https://www.apple.com/macos/big-sur/">
        <img src="https://img.shields.io/badge/Big_Sur-11.6.5-purple.svg"></a>
    <a href="https://www.apple.com/macos/monterey/">
        <img src="https://img.shields.io/badge/Monterey-12.3.1-brown"></a>
        <a href="https://www.apple.com/macos/ventura/">
        <img src="https://img.shields.io/badge/ventura-13.2-purple.svg"></a>
    <a href="https://psref.lenovo.com/syspool/Sys/PDF/withdrawnbook/ThinkPad_X230.pdf">
        <img src="https://img.shields.io/badge/ThinkPad-X230-blue"/></a>
    <a href="https://github.com/acidanthera/OpenCorePkg">
        <img src="https://img.shields.io/badge/OpenCore-0.8.5-blue"/></a>
</p>


<details>
<summary><strong> 我的X230配置 </strong></summary>
<br>

| Category  | THINKPAD X230            |
| --------- | ------------------------ |
| CPU       | Intel Core i5-3320M      |
| SSD       | Samsung 870 Evo 250GB    |
| Display   | 12.5' IPS HD (1366x1768) |
| WiFi & BT | BCM94360HMB              |

- 这个 [X230所有官方配置表](https://psref.lenovo.com/syspool/Sys/PDF/withdrawnbook/ThinkPad_X230.pdf) 可能对你有一点帮助.

</details>
> ## BIOS Settings

- At the minimum, these BIOS settings must be made to install and run macOS without any problems:

| Main Menu | Sub 1         | Sub 2         | Sub 3        | Setting       |
| --------- | ------------- | ------------- |------------- | ------------- |
| Config    | Network       | Wake On Lan   |              | `Disabled`    |
|           | USB           | USB UEFI BIOS Support |      | `Enabled`     |
|           |               | Always On USB |              | `Disabled`    |
|           | Serial ATA (SATA) | Mode      |              | `AHCI`        |
| Security  | Security Chip |               |              | `Disabled`    |
|           | Memory Protection | Execution Prevention |   | `Enabled`     |
|           | Anti-Theft    | Current Setting |            | `Disabled`    |
|           |               | Computrace    | Current Setting | `Disabled` |
|           | Secure Boot   |               |              | `Disabled`    |
| Startup   | UEFI/Legacy Boot |            |              | `UEFI Only`   |
|           |               | CSM Support   |              | `No`          |
|           | Boot Mode     |               |              | `Quick`       |

> ## Modding the BIOS

- A simple method to install a modified BIOS is available [here](https://github.com/n4ru/1vyrain/) (no external programmer required).

> ## Modded BIOS Settings

- The following are further optimization settings that can be figured once your BIOS is modded.

> ## These settings are universally recommended optimizations for your hackintosh

| Main Menu | Sub 1 | Sub 2 | Sub 3 | Setting |
|-----------|-------|------ |------ |-------- |
| Advanced  | System Agent (SA) configuration | Graphics Configuration | DVMT Pre-Allocated | `128MB` |
