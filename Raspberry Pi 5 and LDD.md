## Kernel Build for RPi5

Download the RPi Kernel version 6.10.y from git repository

```bash
git clone --depth=1 --branch rpi-6.1.y https://github.com/raspberrypi/linux.git
cd linux
```

 Set up build config
```bash
export ARCH=arm64
export CROSS_COMPILE=aarch64-linux-gnu-
make bcm2712_defconfig
```

Menuconfig

```bash
make menuconfig
```

Build kernel + DTBs

```bash
make -j`nproc` Image modules dtbs
```

To clean kernel build and configs

```bash
make mrproper
```
## Rootfs Image

Install Raspberry Pi OS Lite (64-bit) using raspberry pi imager software tool.

## Replace the kernel + DTBs + overlays

```bash
cp arch/arm64/boot/Image /media/<user>/<boot>/kernel8.img
cp arch/arm64/boot/dts/broadcom/bcm2712-rpi-s-b.dtb /media/<user>/<boot>/
cp -r arch/arm64/boot/overlays/* /media/<user>/<boot>/overlays/
make INSTALL_MOD_PATH=/media/<user>/<rootfs>/module_install
```

Ensure `config.txt` has

```ini
kernel=kernel8.img
enable_uart=1
dtoverlay=vc4-kms-v3d
```

## Verify

Once logged in you see boot screen and login shell if everything goes well.

To read the boot log from kernel

```bash
journalctl -b
journalctl -b | grep printk
```

## Execution

[[vscodessh]]
[[terminalssh]]

## First Module

[[hello.c]]
