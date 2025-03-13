Note: Work in progress, this patch doesn't actually work

Known issue: Enabling CFG80211 and MAC80211 will crash WiFi functuionality

# Modified Melt Kernel for Kali Nethunter

NEVER use it for illegal use, I am not responsible for any loss caused by users who violate this aggrement

本仓库仅供学习使用，切勿用于非法用途，下载使用该补丁视为同意该点，本人不为任何非法行为导致的损失负责

**根据《中华人民共和国刑法》第二百八十五条，非法侵入计算机信息系统将受法律制裁，最高可处三年有期徒刑**

This is not my own effort and work, I am just the person who find it then carry it. Highly experimental, use it at your own risk

## Usage

Clone melt source from [Pzqqt's repo](https://github.com/Pzqqt/android_kernel_xiaomi_marble/releases/tag/Melt-marble-v3.6)

Apply patch from this repo:

```Linux Shell
git apply <path to the diff file>
```

Follow guide from [Melt's issue](https://github.com/Pzqqt/android_kernel_xiaomi_marble/issues/1) but before you start make, run ```make ARCH=arm64 LLVM=1 LLVM_IAS=1 O=out menuconfig``` to config Kernel Feature according your need, take a look at [Configuring Kernel - Kali Docs](https://www.kali.org/docs/nethunter/nethunter-kernel-2-config-1/)

Flash it then follow [install Nethunter - Kali Docs](https://www.kali.org/docs/nethunter/installing-nethunter/)

## Note

Sytem V IPC is not supported and never enable it if you don't know what it mean

## CREDIT

[Melt Kernel by Pzqqt](https://github.com/Pzqqt/android_kernel_xiaomi_marble)

[Kali Nethunter Gitlab](https://gitlab.com/kalilinux/nethunter)

[shandongtlb's Nethunter Port](https://github.com/shandongtlb/MI9-Nethunter-Project)
