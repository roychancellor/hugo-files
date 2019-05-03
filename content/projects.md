+++
title = "My projects"
date = "2019-05-03"
menu = "main"
+++


All of my personal projects can be found on [GitHub](https://github.com/nathanchance), here are a few key repositories that I am proud of:


# ClangBuiltLinux

ClangBuiltLinux is a collaborative organization between several engineers across different companies like Google, Linaro, and IBM to improve building the Linux kernel with the LLVM tools such as clang and lld. I have contributed warning fixes to [the mainline Linux kernel](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/log/?qt=author&q=Nathan+Chancellor), [improved the continuous integration setup](https://github.com/ClangBuiltLinux/continuous-integration/commits/master?author=nathanchance), and [developed a set of toolchain build scripts](https://github.com/ClangBuiltLinux/tc-build) for myself and others to use for consistent testing/configuration.


# Flash Kernel

I supported the [Pixel 2 (XL) [walleye/taimen]](https://github.com/nathanchance/wahoo), [Pixel (XL) [sailfish/marlin]](https://github.com/nathanchance/marlin), [OnePlus 6 (enchilada)](https://github.com/nathanchance/op6), [OnePlus 5/T (cheeseburger/dumpling)](https://github.com/nathanchance/op5), and [Nexus 6P (angler)](https://github.com/nathanchance/angler).

All of my kernels focused on stability/security by merging in the stable updates from [kernel.org](https://www.kernel.org), any relevant updates from Qualcomm, and building with newer compilers to fix warnings during compilation. Below are the highlights for each kernel.

* Pixel 2 (XL): First to merge in linux-stable and build with up to date versions of Clang. Added EAS 1.5 from kernel/common.

* Pixel (XL): First standalone custom kernel to be compiled properly with Clang, fixing the vast majority of warnings.

* OnePlus 6: I recieved this device as part of [OnePlus's developer program](https://www.xda-developers.com/oneplus-6-developer-application/). I was the first to merge in linux-stable and the updates from Code Aurora Forum, build with Clang, and port over the 32-bit vDSO for arm64 from the Pixel 2 kernels (initially created on a 4.4 base).


# Other interesting personal repos

* [My scripts](https://github.com/nathanchance/scripts) and [dotfiles](https://github.com/nathanchance/dotfiles): The scripts I use for my workflow and personal configuration files, focusing on increasing productivity by decreasing manual intervention needed to doing repetitive tasks.

* [android-kernel-clang](https://github.com/nathanchance/android-kernel-clang): Collected the core Clang patchset for Android kernels from the Pixel 2 and Chromium kernel repositories, supplementing them with fixes for warnings from out of tree code.

* [build-tools-gcc](https://github.com/nathanchance/build-tools-gcc): A script to build a GCC cross compiler for arm/arm64.


# Open source organizations I belong to

* [android-linux-stable](https://github.com/android-linux-stable): Several Android kernel trees with the latest stable tags from [kernel.org](https://www.kernel.org) merged into them, along with conflict resolution notes and a how-to process for other developers and information for users to understand the process. Testing includes merging into my own Flash Kernel repositories linked above and building with all of the relevant defconfigs/compilers. I report results back to the stable tree maintainers, receiving praise for my efforts on a couple occasions ([1](https://lore.kernel.org/lkml/20171117083016.GA20306@kroah.com/) and [2](https://lore.kernel.org/lkml/20180805140301.GA17056@kroah.com/)). Recently, I streamlined the maintenance of these repos into [a script](https://github.com/nathanchance/scripts/blob/master/server/als).

* [Substratum](https://github.com/substratum): An app to compile theming overlays for Sony's Overlay Manager Service (OMS). I am responsible for [our code review](https://substratum.review]) and [our documentation](https://github.com/substratum/documentation).

* [Dirty Unicorns](https://github.com/DirtyUnicorns): An aftermarket Android ROM. I am responsible for helping with testing and picking in features, along with fixing issues.


# Other open source contributions

* [kernel/common](https://android-review.googlesource.com/q/project:kernel/common+author:natechancellor%2540gmail.com): Google's common Android kernel.

* [sonyxperiadev/kernel](https://github.com/sonyxperiadev/kernel/pulls?q=author%3Anathanchance): The Linux kernel used for [Sony's Open Devices program](https://developer.sony.com/develop/open-devices/).

* [AnyKernel2](https://github.com/osm0sis/AnyKernel2/commits/master?author=nathanchance): A kernel flashing utility for TWRP, responsible for unpacking the boot image, applying any requested ramdisk changes, repacking the files, and flashing them to the boot image partition.
