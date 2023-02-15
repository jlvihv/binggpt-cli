# BingGPT

BingGPT 命令行客户端，使用 rust 编写。

这个项目是 [EdgeGPT](https://github.com/acheong08/EdgeGPT) 的 rust 语言实现，所有困难的事情都是原项目作者 `acheong08` 完成的，我仅仅是用 rust 写了一遍，所有的功劳都归功于他，感谢大佬的辛勤付出！

## 要求

你必须有一个可以访问 BingGPT 的微软账户。

## 配置 (必须的)

- 为 [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) 或 [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/) 安装 `cookie-editor` 扩展
- 去 [bing.com](https://www.bing.com) 登录你的微软账户
- 打开扩展
- 单击右下角的“Export”（这会将您的 cookie 保存到剪贴板）
- 将您的 cookie 新建或写入到 `~/.config/bing-cookies.json` 文件中

## 使用方法

> 首先你需要执行上面的配置步骤。

如果你有 rust 开发环境，首先你需要克隆代码，进入本项目目录，然后运行 `cargo run` 。

如果你想编译成二进制文件，可以运行 `cargo build --release`，编译完成后，你可以在 `target/release` 目录下找到编译好的二进制文件。

启动程序后，当看到`You:`时，表示你可以开始与 BingGPT 对话了，按两次回车键，即可发送消息。

在对话中，你可以使用如下指令：

- `:q` `:quit` `:exit` 退出程序
- `:more` 进入多行模式，你可以放心的输入更多文本，或者从剪贴板中粘贴文本
- `:end` 退出多行模式

## 工作正在进行中