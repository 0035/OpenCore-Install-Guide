# Making the installer in Windows

* Supported version: 0.5.7

While you don't need a fresh install of macOS to use OpenCore, some users prefer having a fresh slate with their boot manager upgrades.

To start you'll need the following:
* 4GB USB Stick
* [GibMacOS](https://github.com/corpnewt/gibMacOS)

## Downloading macOS

To start, open gibMacOS.bat as Admin and select `Toggle Recovery-Only`:

![](/images/post-install/winblows-install-md/gib-default.png)

Now search through for your desired version of macOS, for this example we'll choose option 5 for macOS Catalina:

![](/images/post-install/winblows-install-md/gib-recovery.png)

This will download the RecoveryHDMetaDmg.pkg to `\gibmacos-master\macOS Downloads\publicrelease\xxx-xxxxx - 10.x.x macOS xxx`

![](/images/post-install/winblows-install-md/gib-done.png)

## Making the installer

Next open `makeinstall.bat` as Admin and select your drive with option O for OpenCore( ex: 1O).

![](/images/post-install/winblows-install-md/make-install.png)

Once your drive is formatted, it will then ask you for the `RecoveryHDMetaDMG.pkg` that we downloaded earlier. Top right of the file window will let you copy the file path:

![](/images/post-install/winblows-install-md/make-install-location.png)

![](/images/post-install/winblows-install-md/recovery-location.png)

makeinstall will finish up by installing OpenCore to your USB's EFI System Partition, you can find this partition labeled as `BOOT`:

![](/images/post-install/winblows-install-md/make-install-done.png)

![](/images/post-install/winblows-install-md/EFI-base.png)




### Now with all this done, return to [Creating the USB](/installer-guide/opencore-efi.md) to finish up your work