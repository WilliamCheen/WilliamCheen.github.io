---
layout: post
title: "使 Xcode8.x 支持基于 iOS7 系统的真机调试"
date: 2017-06-02 13:37:45 +0800
comments: true
categories: 
---

#### Xcode8.x 支持 iOS7 的真机调试

* 将 Xcode 7 里的 /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/DeviceSupport 文件拷贝到 Xcode 8.x 的相同文件夹下
* 修改 /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS.sdk/SDKSettings.plist 文件里的 DefaultProperties\DEPLOYMENT_TARGET_SUGGESTED_VALUES，以此（从大到小的）增加相应的版本（7.0、7.1）
* 重启 Xcode
