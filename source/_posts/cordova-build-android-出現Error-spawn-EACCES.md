---
title: 'cordova build android 出現Error: spawn EACCES'
date: 2019-06-25 10:38:08
categories:
- 筆記
tags:
- cordova
- android
---
## 問題發生原因
因為platform/android中的gradlew沒有執行權限

## 解決方式
開啟consol並切換目錄至專案下的 /platform/android的資料夾
執行以下之指令，目的為取得該執行黨的執行權限
```bash
$ chmod +x ./platform/android/gradlew
```
