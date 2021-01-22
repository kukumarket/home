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

