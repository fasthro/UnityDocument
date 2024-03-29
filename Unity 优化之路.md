# Unity 优化之路

---

## **图片压缩格式**

**Android**
使用 ETC 和 ETC2 格式 (不支持 ASTC 格式的 Android 机型太多)

**IOS** 
使用 ASTC 格式

---

## **Bundle压缩**

使用 LZ4 压缩格式，不管从解压速度还是内存占用来说都非常小

---

## **运行时设置分辨率**

高渲染的场景中可以动态调整降低分辨率，是用户在没有感知的情况下提高帧频。

---

## **Camera RT缩放分辨率可提高帧频**

Unity 2017 之后，在提高帧频的同时会在效果显示上会响应降低。

---

## **Android 打包方式**

IL2CPP 打包

---

## **支持 GPU Instance**

在动作处理这块，可以动态合批

---

## **动画系统可以指定区域进行缩放**

---

## **Android Blit 设置（提高帧率）**

描述了如何在屏幕上显示内容的方法。

如果3D 和光照渲染方面不是特别多可以选择 Never 关闭此选项，否则可以设置自动

![avatar](Images/Unity-优化/BlitType.jpg)

---

## **Camera 设置（提高帧率）**

可以选择关闭 Allow HDR 和抗锯齿 Allow MSAA 这两个选项提高渲染效率

![avatar](Images/Unity-优化/Camera-HDR.jpg)

---

## **Lighting 设置（提高帧率）**

如果没有使用实时光，可以关闭 Lighting 设置中 Realtime Lighting 和 Mixed Lighting 选项

![avatar](Images/Unity-优化/Lighting-Setting.jpg)


