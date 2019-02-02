+++
categories = []
date = "2019-02-01T16:00:00+00:00"
draft = true
slug = ""
tags = []
title = "Using macOS"

+++
1. restart `mDNSResponder`

Restart `mDNSResponder` may help to solve the network problem after long time running

```
sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.mDNSResponder.plist
sudo launchctl load -w /System/Library/LaunchDaemons/com.apple.mDNSResponder.plist
```