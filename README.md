# aadb [![Linux Build Status](https://travis-ci.org/appetizerio/aadb.svg?branch=master)](https://travis-ci.org/appetizerio/aadb) [![Build status](https://ci.appveyor.com/api/projects/status/nkf33d5bk9lofyjd/branch/master?svg=true)](https://ci.appveyor.com/project/mingyuan-xia/aadb/branch/master)

![aadb architecture](https://github.com/appetizerio/aadb/blob/master/aadb.png|alt=aadb])

aadb (Appetizer Android Debug Bridge) is a Python Library that provides 101 Ways to Control an Android. It provides the following features across three major platforms (Linux, Windows and macOS):
* A superset of adb commands: shell, install, uninstall, reboot, etc; various convenience commands such as inputing text (enabled with a custom `adbclient`)
* Real-time multi-touchscreen control: tap, long click, drag, complicated gesture, multi-finger gesture (enabled by [openstf/minitouch](https://github.com/openstf/minitouch))
* Real-time screen capture: single screenshot and continuous high-FPS recording (enabled by [openstf/minicap](https://github.com/openstf/minicap))
* `[incubating]` On-screen view manipulation: view hierarchy and UI automation (enabled by [uiautomator](https://developer.android.com/training/testing/ui-testing/uiautomator-testing.html))

aadb requires `adb` from the Android SDK. You can download the full SDK or obtain a standalone `adb` executable. aadb only needs the adb server part of the `adb` executable and is compatible with the adb server from Google's [python-adb](https://github.com/google/python-adb) and Facebook's [fb-adb](https://github.com/facebook/fb-adb). aadb implements a custom adb client that is more stable and flexible than using the adb client part of the `adb` executable directly with `subprocess`. For a more technical understanding of the `adb` executable, client/server, protocol and derived versions, please check out our wiki.

```
License: Apache License Version 2
```
