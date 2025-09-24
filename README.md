NOTE: This repository is no longer being updated and has been succeeded by [StikDebug](https://github.com/StephenDev0/StikDebug)

This project was made as a proof of concept for on device JIT enabling for iOS 17+. It used my fork of [pymobiledevice3](https://github.com/joshrad-dev/pymobiledevice3) and my version of [JitStreamer](https://github.com/joshrad-dev/JitStreamer) running in a barebones Alpine Linux VM. It included Python, pip, tailscale, usbmuxd, and helper scripts.

## Documentation
Download the VM from releases. To run the server, login with root/password and run `./JitStreamer.sh`

When running the shortcut and using the "Enable JIT" function in SideStore, constantly bring UTM SE into the foreground to maintain the connection and prevent it from being killed in the background. UTM SE has issues with connecting when running from the background.

The VM also includes a script `sh update.sh` which should update to their latest versions if needed.

If the scripts show up blank for whatever reason, you can redownload them using curl:

`curl -O https://raw.githubusercontent.com/jawshoeadan/AlpineJitVM/refs/heads/main/JitStreamer.sh`

`curl -O https://raw.githubusercontent.com/jawshoeadan/AlpineJitVM/refs/heads/main/update.sh`

If you appreciate what I do, [consider donating.](https://buymeacoffee.com/joshrad-dev)
