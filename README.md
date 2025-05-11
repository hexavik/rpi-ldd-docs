# Raspberry Pi 5 & Linux Device Driver Learning Vault

Welcome to my personal knowledge base for experimenting **Linux Device Drivers and kernel module development** and tinkering with the **Raspberry Pi 5**, maintained using [Obsidian](https://obsidian.md/).

> [!NOTE]
>
> This vault includes real-world logs, setups, issues, and solutions - writing dyring hands-on experiments with the Raspberry Pi 5 running a custom Linux kernel.

---

## 🧠 What's Inside

- 💻 **Kernel Compilation Logs**
- 🧰 **Device Tree Overlays & Config**
- 📁 **Driver Code Structure**
- ⚙️ **Module Build & Insert Logs**
- 🐛 **Debugging Sessions**
- 🧪 **Experiments with GPIO, SPI, I2C, etc.**
- 📚 **Helpful Resources, Commands & Tips**

---

## 🛠 Requirements

To use this Obsidian vault:

- Isntall [Obsidian](https://obsidian.md/) on your system (Mac, Linux, Windows).
- Clone this repo locally.
- In Obsidian, open the folder as a vault (`Open folder as vault`).

```bash
git clone https://github.com/hexavik/rpi5-linux-drivers-vault.git
cd rpi5-linux-drivers-vault
```

## 🧭 Folder Structure (might be changed)

```text
📁 RPi5-Linux-Drivers-Vault/
├── 📝 00_Overview.md
├── 🧪 Experiments/
│   ├── gpio_blink_test.md
│   └── spi_driver_log.md
├── ⚙️ Kernel/
│   ├── kernel_build_steps.md
│   └── rpi_kernel_config_notes.md
├── 🐞 Debug/
│   ├── insmod_crash.md
│   └── dmesg_troubleshooting.md
└── 📚 References/
    └── linux_driver_books.md
```

## 🧩 Optional: Use Obsidian Git Plugin

For automatic sync within Obsidian:

1. Install the "Obsidian Git" plugin from Community Plugins.
2. Configure the plugin with your GitHub repo.
3. Enable auto-push/pull if desired.

## 🧵 Contributing

This is a personal learning vault, but feel free to fork it if you’re also exploring embedded Linux on the Pi. If you have ideas or corrections, open an issue or pull request.

*Built with ❤️ by [hexavik](https://hexavik.github.io/)*
