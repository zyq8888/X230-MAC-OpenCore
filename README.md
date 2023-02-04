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

<details>
<summary><strong>关于黑苹果X230 BIOS 设置 </strong></summary>
<br>
- 至少，必须进行这些BIOS设置才能安装和运行macOS而不会出现任何问题:

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

可以使用一种简单的方法来安装经过修改的BIOS[外部传送](https://github.com/n4ru/1vyrain/)（无需外部编程器）。
修改过BIOS 可以解网卡白名单 以及开启一些功能
    
以下是修改BIOS后可以配置的进一步优化设置。
| Main Menu | Sub 1 | Sub 2 | Sub 3 | Setting |
|-----------|-------|------ |------ |-------- |
| Advanced  | System Agent (SA) configuration | Graphics Configuration | DVMT Pre-Allocated | `128MB` |
</details>
