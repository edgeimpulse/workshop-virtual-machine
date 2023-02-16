# Edge Impulse Workshop Virtual Machine

This virtual machine (VM) was constructed to alleviate toolchain installation issues across multiple operating systems during live workshops. It contains any necessary tools and development environments required, or it offers an easy path to install such tools in a standardized manner.

## Getting started

### Import VM

Install VirtualBox for your operating system: [www.virtualbox.org](https://www.virtualbox.org/)

Download the latest EI Workshop VM image: [EI Workshop VM v0.3](https://drive.google.com/file/d/1I1rS47PynmMVsL_fgTXP2UgQk_MMDaEc/view?usp=share_link)

Open VirtualBox. Select **File > Import Virtual Appliance**. Select the downloaded .ova file.

%%%screen: Import ova window

### Configure clipboard

If you would like to be able to copy and paste text between your host machine and VM, click on the imported VM on the left pane. Select **Settings**. Click **General** and go to the **Advanced** tab.

Change *Shared Clipboard* to **Bidirectional**.

%%%screen: bidirectional clipboard

Click **OK**.

### Configure USB passthrough

Click on the imported VM on the left pane. Select **Settings**. Select **USB** on the left pane of the pop-up window. Ensure that *Enable USB Contrller* is checked with *USB 2.0 (OHCI + EHCI) Controller* selected.

Plug in your development board to your computer.

Click the **Add new USB filter** button on the right side of the window. Select your development board. The board should appear in the *USB Device Filters* pane.

If your board has a bootloader mode, put the board into bootloader mode and repeat the above process. You should see two separate entries in the filters pane: one for your board in regular operation mode and another for your board in bootloader mode.

%%%screen: USB filters

Click **OK**.

### Start VM

Select the VM on the left pane and click *Start*!

## License

The virtual machine image is built using [Bodhi Linux](https://www.bodhilinux.com/), which mostly uses [GPL](https://www.gnu.org/licenses/gpl-3.0.en.html).

This (admittedly very short) guide is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).