使用 snapd 安装 Flutter

最简单的方式是使用 snapd 在 Linux 上安装 Flutter。更多详情请查看：安装 snapd。

如果你已经有 snapd 了，那么你可以通过 Snap 商店来安装 Flutter，或者通过以下命令安装：

$ sudo snap install flutter --classic

备忘

安装 snap 后，可以使用如下命令展示 Flutter SDK 路径：

  $ flutter sdk-path

vi ~/.bash_profile
在文件末尾添加：使能Flutter桌面，添加flutter路径，添加国内镜像源（方便更新flutter SDK）

export ENABLE_FLUTTER_DESKTOP=true
export PATH=~/work/flutter/bin:$PATH
export PUB_HOSTED_URL=https://pub.flutter-io.cn
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn




    On Ubuntu, if you installed from snap, you should set these two parameters:

    flutter config --android-sdk="$HOME/Android/Sdk"
    flutter config --android-studio-dir="/snap/android-studio/current/android-studio/"

[模拟器]
    对于 Debian/Ubuntu 系统，使用 APT-GET 命令 或 APT 命令 来安装 anbox。

    $ sudo apt install anbox

[adb调试工具]
默认情况下，Anbox 并没有带有 Google Play Store。因此，我们需要手动下载每个应用程序（APK），并使用 Android 调试桥（ADB）安装它。

ADB 工具在大多数的发行版的软件仓库是轻易可获得的，我们可以容易地安装它。
对于 Debian/Ubuntu 系统，使用 APT-GET 命令 或 APT 命令 来安装 ADB。

    $ sudo apt install android-tools-adb


