# LenovoKeyboardLayoutFix

[English README Here](https://github.com/long45343/LenovoKeyboardLayoutFix/blob/main/README_EN.md)

适用于Y700 2025的串流键盘解决方案

低技术力的解决方案，还请大佬轻喷。

# 原理

通过修改/system/usr/keylayout/generic.kl使得滚轮锁定键和Action键交换，从而避免在串流时按到左边Windows键触发。

# 使用方法

（仅适配了[阿西西的Moonlight](https://github.com/Axixi2233/moonlight-android)）

Magisk/KSU/Apatch（仅测试了KSU，但应该都可以用）安装模块后打开月光-阿西西的无障碍权限后导入本项目[Release](https://github.com/long45343/LenovoKeyboardLayoutFix/release)内的buttonSwitch.json后即可实现串流效果，但无法使用滚轮锁定键

# 修改

如果想对模块进行自定义可参照以下方法

本模块对调了Generic.kl内的key 125（对应键盘的Windows键）与key 70（对应键盘的滚轮锁定键）所对应的按键，如果需要使用滚落锁定键，可将key 125对应的META_LEFT与其他按键的定义对调，但一定要使META_LEFT可用，否则连接键盘会没有反应

对调完成后应该无需修改buttonSwitch.json也可正常工作。
