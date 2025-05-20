# LenovoKeyboardLayoutFix

[English README Here](https://github.com/long45343/LenovoKeyboardLayoutFix/blob/main/README_EN.md)

Solution for Lenovo Legion Y700 2025's keyboard when using stearming software

Low-tech solutions, code is very noob:).

# Principe

Edit /system/usr/keylayout/generic.kl to swap scroll_lock key and Action key to avoid trigger Action Key when using stearming software.

# Usage

（Juse adapt[Axixi2233's Moonlight](https://github.com/Axixi2233/moonlight-android)）

Install via Magisk/KSU/Apatch（only KSU tested，but it should work properly between these root solution), then open the Axixi2233"月光-阿西西"and import the buttonSwitch.json in[Release](https://github.com/long45343/LenovoKeyboardLayoutFix/releases), the option in setting called "导入自定义无障碍配置文件", enable the Accessibility permission then you can use Windows key fluently, And the scroll lock key is swaped.

# Modify

If you want to modify this module,here's the way.

This module swap the key 125(Windows key on Keyboard) and Key 70(Scroll lock key on keyboard), if you need to use scroll lock key,just swap key 125 with another key, but must gurantee that META_LEFT is vaild, or the keyboard will failure.

Moonlight should work fine without modify buttonSwitch.json after key swap.
