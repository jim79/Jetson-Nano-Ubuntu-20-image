# Jetson Nano with Ubuntu 20.04 OS image

## This page contains the backup images from the original git repo.
Bare-bones Ubuntu 20.04 OS with JetPack 4.6.1, without TensorFlow and PyTorch

## A Jetson Nano - Ubuntu 20.04 image with OpenCV, TensorFlow and Pytorch
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>
### Update 9-17-2023. 
- Refresh Ubuntu 20.04.
- Add WiFi support (https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/issues/28).
- Reduce xz archive.
### Update 9-6-2023. 
- Added a new spilt image.
### Update 7-15-2023. 
- Refresh Ubuntu 20.04.
- Update OpenCV (**4.8.0**)
- Update PyTorch (**1.13.0**)
- Update TorchVision (**0.14.0**)
- New: TensorRT (**8.0.1.6**)
### Update 7-13-2023. 
- Added an installation wheel for TensorRT 8.0.1.6+cuda10.2. The version is synchronous with the C++ version found on the image. Newer versions of TensorRT require CUDA 11 or later, which is not supported on a Jetson Nano. (thanks to [Teemu Heikkilä](https://github.com/theikkila))
### Tip 3-10-2023. 
- Connected to the net for the first time? Wait for the Software Updater and let it refresh your operating system.
### Update 7-30-2022. 
- Added bare overclocked Ubuntu 20.04 image.
### Update 7-26-2022. 
- Refresh Ubuntu 20.04
- Update OpenCV (**4.6.0**)
- Update PyTorch (**1.12.0**)
- Update TorchVision (**0.13.0**)
- New xz archive (size reduction of 26%)
- New download site (Gdrive has a limited number of downloads per day).
### Update 1-30-2022. 
- Add **Jtop** (thanks to [SkrilaxCZ](https://github.com/rbonghi/jetson_stats/issues/173))

------------

## Installation.

- Get a 32 GB (minimal) SD card to hold the image. 
- Download the image `JetsonNanoUb20_3b.img.xz` (**8.7 GByte!**) from our [Sync](https://ln5.sync.com/dl/403a73c60/bqppm39m-mh4qippt-u5mhyyfi-nnma8c4t). 
- Flash the image on the SD card with the [Imager](https://www.raspberrypi.org/software/) or [balenaEtcher](https://www.balena.io/etcher/).
- According to [issue #17](https://github.com/Qengineering/Jetson-Nano-image/issues/17#) only flash the xz directly, not an unzipped img image.
- Insert the SD card in your Jetson Nano and enjoy.
- Password: ***jetson***
- JetsonNanoUb20_3b.img.xz md5sum: D738F1FE20088A1BDBD10E2358B512F7

### GDrive.
In some parts of the world, getting a good solid connection to Sync is difficult. That is why we've also provided a copy on [Google Drive](https://drive.google.com/file/d/1L2H_sQC_kSILrcJteWg7htKxJirtDsZ9/view?usp=sharing). However, Google Drive limits the number of daily downloads, which is much lower than our average daily download volume. Please be considerate and use Google Drive only if necessary.

#### Tip:<br>
The SD card is overflowing with software; more than 21 GByte! With a 32 GB card, you don't have enough space to work decently.<br>
Therefore, flash the image on an SD card of 64 or more and use GParted (`$ sudo apt-get install gparted`) to enlarge the partition.

------------

### Split image.

Due to the large image (9.3 GB), the download may take quite some time. It makes downloading vulnerable.<br/>
That's why we split the file into smaller chunks. These are more manageable than one huge download.<br/>
If you prefer this partial download over one large one, download the following 14 files (700 MB each) and place them in one folder.</br>
- [JetsonNanoUb20_3b.img.xz.001](https://ln5.sync.com/dl/26ab88540/2mgt4wai-ej6kx28m-hu2jymnk-7zfe65d8)
- [JetsonNanoUb20_3b.img.xz.002](https://ln5.sync.com/dl/768c93180/cq7zriji-dnhe3thr-upgnyyfr-zerrba9x)
- [JetsonNanoUb20_3b.img.xz.003](https://ln5.sync.com/dl/5d3da43d0/wy34gd75-689eh3hq-asg8w89n-ti5c3ky5)
- [JetsonNanoUb20_3b.img.xz.004](https://ln5.sync.com/dl/0ef819060/qsxkb62n-ufx8wfsw-tujifiw4-38zt2xzh)
- [JetsonNanoUb20_3b.img.xz.005](https://ln5.sync.com/dl/d753ac7f0/fhdhynne-86mgaeq5-6q2bs3qs-z3tkyzt4)
- [JetsonNanoUb20_3b.img.xz.006](https://ln5.sync.com/dl/1b5b19800/z46pgc2q-quvpm5hy-yj2n4x4x-u34mwdgm)
- [JetsonNanoUb20_3b.img.xz.007](https://ln5.sync.com/dl/f76c905b0/he8psg2g-293hjh5u-kgpyjmr7-fui227qu)
- [JetsonNanoUb20_3b.img.xz.008](https://ln5.sync.com/dl/97cada030/5ixwp92p-zwgj6hkj-t6hfe3fv-pbcxyd28)
- [JetsonNanoUb20_3b.img.xz.009](https://ln5.sync.com/dl/f3f531a70/mgqinzz2-9ys5rtbg-z7t89un7-8i7zm65d)
- [JetsonNanoUb20_3b.img.xz.010](https://ln5.sync.com/dl/db8b60ec0/a4hakcrw-78g9i65r-h675jq7t-xuhv5ft4)
- [JetsonNanoUb20_3b.img.xz.011](https://ln5.sync.com/dl/6861a0cd0/9xyekbt6-ipsrep5w-9rcuwk8g-hggp2kx3)
- [JetsonNanoUb20_3b.img.xz.012](https://ln5.sync.com/dl/3e521c4a0/c5meen53-gnkupyzv-ixp57fmc-tu4n6bej)
- [JetsonNanoUb20_3b.img.xz.013](https://ln5.sync.com/dl/72f4dae70/av2f5bnt-z4mynsua-tu8us97q-gntzgrks)

Once you have all the files run
```
7z x JetsonNanoUb20_3b.img.xz.001
```
7Z will start extracting the first file (`*.001`) and automatically the next files in order.</br>
You will end up with `JetsonNanoUb20_3b.img.xz`, the original image which you now can flash on an SD card with [Imager](https://www.raspberrypi.org/software/) or [balenaEtcher](https://www.balena.io/etcher/).<br/><br/>
If you get the error `'7z' is not recognized as an internal or external command, operable program or batch file.` please give the full path to 7z. For instance,
```
"C:\Program Files\7-Zip\7z.exe" x JetsonNanoUb20_3b.img.xz.001
```

------------

### Bare image.

For those who want a bare-bones Ubuntu 20.04 OS with JetPack 4.6.1, without TensorFlow and PyTorch, you can download the [image here](https://ln5.sync.com/dl/7261d3770/jebr2z9k-kwj4wwvd-3wxjtqsx-36zbu3cx) (5.6 GB).<br/>
The Nano is overclocked at 1900 MHz. See https://qengineering.eu/overclocking-the-jetson-nano.html for more information.<br/>
By the way, the image with TensorFlow and PyTorch is not overclocked and runs at the regular 1479 MHz.<br/>
- JetsonNanoUb20_bare.img.xz md5sum: DB4FC5A1B09876B37FF57F42540B3250 
![output image]( https://qengineering.eu/images/OverNanoUb20.webp )<br/>

------------

### ROS

If you plan to use this image with ROS, please look at [JetsonNano-ROS2](https://github.com/AIResearchLab/JetsonNano-ROS2).<br>
As you can see, [Kalana Ratnayake](https://github.com/KalanaRatnayake), a PhD student in the Robotics and Artificial Intelligence Lab, part of the Faculty of Science and Technology at the University of Canberra has done a great job. Thanks. 👍

------------

### Archive.

The previous (7-26-2022) Ubuntu 20.04 image, with OpenCV **4.6.0**, TensorFlow **2.4.1** and PyTorch **1.12.0** can be [downloaded here](https://ln5.sync.com/dl/741c98fe0/x8kxkhgs-cgmzk7rf-n4m7pyw8-h64tzbv5) - **7.9 GByte**.<br>
Or the split image:<br>
- [JetsonUb20_2.7z.001](https://ln5.sync.com/dl/44d2f0f10/9h9skipf-i7jaixkh-mpbznnev-vk58qfaa)
- [JetsonUb20_2.7z.002](https://ln5.sync.com/dl/d506a8680/rfs5jync-rgnkvk9u-igwjc2y5-pxkppy4c)
- [JetsonUb20_2.7z.003](https://ln5.sync.com/dl/21e5b83e0/e87zbu2t-mx8vvhh4-z7kww4g3-hfe68b46)
- [JetsonUb20_2.7z.004](https://ln5.sync.com/dl/401753da0/qipc4az9-7amw452w-asiazc5u-t8t4yy99)
- [JetsonUb20_2.7z.005](https://ln5.sync.com/dl/866cb6b90/zrpbzhyk-p392casn-qqmp2g6c-qwxiz7nq)
- [JetsonUb20_2.7z.006](https://ln5.sync.com/dl/84b315060/w6mb6jyi-pnhrxs2i-e3mqn747-8yqzpc4n)
- [JetsonUb20_2.7z.007](https://ln5.sync.com/dl/7a82d6820/xn6y9jva-xqeqfqkq-hbu5kkr2-dssdjhhq)
- [JetsonUb20_2.7z.008](https://ln5.sync.com/dl/01c6d8a60/6nrvzuv9-4s8ik4wh-3hqn6b8k-4cj4hkz4)

The first (9-22-2021) Ubuntu 20.04 image, with OpenCV **4.5.3**, TensorFlow **2.4.1** and PyTorch **1.9.0** can be [downloaded here](https://drive.google.com/file/d/13IsHEH8RnpFwJob1ZeJynVj40BKt5qBL/view?usp=sharing) - **10.3 GByte**. 

------------

## Warnings.

* **Do not install Chromium** as it will interfere with the Snap installation. Use the preinstalled Morzilla Firefox.
* **Corrupted lavapipe** You may encounter a warning during booting that the lavapipe is broken.<br/>
The solve the issue remove the /usr/share/vulkan/icd.d folder `$ sudo rm -rf /usr/share/vulkan/icd.d`<br/>
See issue [#173](https://github.com/rbonghi/jetson_stats/issues/173).


------------

## Upgrading.

You may encounter issues when upgrading (`$ sudo apt-get upgrade`) this Ubuntu 20.04 version. It has to do with a conflicting `/etc/systemd/sleep.conf` file, which blocks the upgrade.
Follow the instructions on our [website](https://qengineering.eu/install-ubuntu-20.04-on-jetson-nano.html#upgrade) to resolve this issue.

------------

## Tips.

Use a tool like [GParted](https://gparted.org/) `sudo apt-get install gparted` to expand the image to larger SD cards. We recommend a minimum of 64 GB. Deep learning simply requires a lot of space.<br/><br/>
Many CUDA related software needs gcc version 8.<br/> We have installed gcc and g++ version 8 alongside the preinstalled version 9.<br/>
You can select your choice with `$ sudo update-alternatives --config gcc` and `$ sudo update-alternatives --config g++`.<br/><br/>
![output image]( https://qengineering.eu/images/SelectorUb20.webp )<br/>

------------

## SSD 

You can use an external SSD USB drive holding your Ubuntu 20.04 OS and other software.
Please follow the steps given at [issue 32](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/issues/32).

------------

## Pre-installed software.

Clicking on the links below will direct you to our installation guide.<br>

- [OpenCV](https://qengineering.eu/install-opencv-on-jetson-nano.html) 4.8.0
- [TensorFlow](https://qengineering.eu/install-tensorflow-2.4.0-on-jetson-nano.html) 2.4.1
- [Pytorch](https://qengineering.eu/install-pytorch-on-jetson-nano.html) 1.13.0
- [TorchVision](https://qengineering.eu/install-pytorch-on-jetson-nano.html) 0.14.0
- [TensorRT](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/issues/11) 8.0.1.6
- [TeamViewer aarch64](https://www.teamviewer.com/en/download/linux/) 15.24.5
- [Jtop](https://github.com/rbonghi/jetson_stats) 4.2.1

Tensorflow 2.5 and above, just like PyTorch 2.0, requires CUDA 11. CUDA version 11 cannot be installed on a Jetson Nano due to incompatibility between the GPU and low-level software.

![image](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/466e8a7e-b610-41c9-bfdb-5291465f24e4)<br>
![image](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/f7931af3-d4c2-4ca0-bf00-d09e2c18e313)<br>
![image](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/6df69080-f84f-465a-a20f-199d4b2a98b2)<br>

------------

## VNC.
Ubuntu 20.04 supports VNC. Please follow the next steps to enable it.<br>
BTW, images are taken from the Jetson Orin, but they are identical on the Jetson Ubuntu 20<br>
![VNC_1](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/e94843dd-3222-4893-8848-e169461101da)<br>
![VNC_2](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/52d4fcfa-0492-4b1e-bef7-a0f3f6929038)<br>
![VNC_3](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/b9f89e79-bf53-4690-ad7d-6e53895546f9)<br>
![VNC_4](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/cf2abd1d-1b26-44fa-92b3-34d363fd7948)<br>
The last step is lowering the encryption level.
```
$ gsettings set org.gnome.Vino require-encryption false
```
On your client please uncheck the _Authenticate_ boxes.<br>
![image](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/9a646010-d53e-4e65-8681-f9785e6ffa85)

------------

## Headless.
If you want a headless installation of Ubuntu 20.04, please follow the next commands.
```
sudo chown root:root / /lib
sudo apt purge ubuntu-desktop -y && sudo apt autoremove -y && sudo apt autoclean
sudo apt-get remove nautilus nautilus-* gnome-power-manager gnome-screensaver gnome-termina* gnome-pane* 
sudo apt-get remove gnome-applet* gnome-bluetooth gnome-desktop* gnome-sessio* gnome-user* gnome-shell-common
sudo apt-get remove zeitgeist-core libzeitgeist* gnome-control-center gnome-screenshot && sudo apt-get autoremove
sudo apt-get remove --purge libreoffice*
sudo apt-get remove libreoffice-core
sudo apt-get remove snapd lightdm cups chromium*
```
You end up with a headless OS consuming ~ 420 MB.<br>
Below is a screen dump of Putty connected to the Jetson Nano running jtop.<br>
![330769059-52674244-cf3c-4ea1-a903-a1ed19719ce0](https://github.com/Qengineering/Jetson-Nano-Ubuntu-20-image/assets/44409029/cbdf1acc-19d5-4b7b-bf10-7ba8556afcbb)


------------

## OpenCV + TensorFlow or TensorRT.

Importing both TensorFlow (or TensorRT) and OpenCV in Python can throw the error: _cannot allocate memory in static TLS block_.<br/>
This behaviour only occurs on an aarch64 system and is caused by the OpenMP memory requirements not being met.<br/>
For more information, see GitHub ticket [#14884](https://github.com/opencv/opencv/issues/14884).<br/>

![output image](https://qengineering.eu/images/SwapImportOpenCVJetson.webp)

There are a few solutions. The easiest is to import OpenCV at the beginning, as shown above.<br/>
The other is disabling OpenMP by setting the -DBUILD_OPENMP and -DWITH_OPENMP flags OFF.<br/>
Where possible, OpenCV will now use the default pthread or the TBB engine for parallelization.<br/>
We don't recommend it. Not all OpenCV algorithms automatically switch to pthread.<br/>
Our advice is to import OpenCV into Python first before anything else.<br/><br/>

Please visit https://qengineering.eu/install-ubuntu-20.04-on-jetson-nano.html for more information.<br/>

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 
