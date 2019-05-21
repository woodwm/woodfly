+++
categories = []
date = "2017-12-24T03:09:22+00:00"
slug = ""
tags = []
title = "Macbook 待机耗电量大"

+++
（ macOS High Sierra ）

* 蓝牙偏好设置 /高级 /去掉勾选「允许蓝牙设备唤醒这台电脑」
* 系统偏好设置 /节能 /电源适配器下， 去掉勾选「唤醒以供 Wi-Fi 网络访问」
* 系统偏好设置 /节能 /电池下，先勾选「电池供电时启用 Power Nap 」，再去掉勾选该选项，此举为了解决 macOS  存在的可能性的 Bug，看似未勾选，实际上是勾选的可能性存在的 Bug。这个 Bug 会导致在用电池睡眠的时候依然在定期唤醒访问 Wi-Fi。
*  sudo pmset -b tcpkeepalive 0 设置在电池供电的情况下，关闭网络访问。