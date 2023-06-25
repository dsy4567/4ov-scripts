# [4ov-scripts](https://github.com/dsy4567/4ov-scripts)

[4399 on vscode](https://github.com/dsy4567/4399-on-vscode) 的 HTML 代码片段仓库

## HTML 代码片段被用来做什么

它们会被 [4399 on vscode](https://github.com/dsy4567/4399-on-vscode) 注入
`webview` 里, 用来优化游戏体验, 以及为
[4399 on vscode](https://github.com/dsy4567/4399-on-vscode) 添加新功能

## 安装

访问 <https://dsy4567.github.io/4ov-scripts/download.html>，将 `.html` 文件保存到 `<主目录>/.4ov-data/html-scripts/` 文件夹下，然后打开 VSCode 设置页，在搜索框中输入 `@id:4399-on-vscode.scripts` 并修改设置

> 在 Windows 系统下, 你可以通过按 <kbd>Windows 徽标键</kbd> + <kbd>R</kbd>, 然后输入 `%USERPROFILE%` 来打开主目录

## 快速上手

> 注: 非贡献者无需阅读以下内容

```html
<!-- foobar.html -->

<!--

XXX LICENSE

Copyright (c) <year> <your name>

balalalalalalalalalala...

-->

<!--

<head>...

-->

<script>
    // 常量
    FULL_WEB_SERVER_URI; // 详见 https://code.visualstudio.com/api/advanced-topics/remote-extensions#option-1-use-asexternaluri

    fetch("/openUrl/https://www.4399.com/"); // 打开链接
    fetch("/openUrl/https://www.4399.com/flash/114514.htm"); // 直接启动游戏
    open("https://www.4399.com/"); // 4399 on vscode 已经帮你重写了这个函数, 等效于 fetch("/openUrl/https://www.4399.com/")

    // 代理, 仅支持 GET 请求
    fetch("/proxy/https://www.4399.com/");
</script>
<style>
    .myDiv{
        color: #66ccff;
    }
</style>

<!--

...</head>

-->

```
## 发布

1. fork 这个仓库
2. 在仓库根目录下创建一个文件夹, 名字随便（尽量不要包含空格或特殊字符）
3. 在这个文件夹里创建 `LICENSE`, `README.md`, `<dir-name>.html` 以及其他必要的文件
4. 修改 `download.html`
5. 发个 PR, 等待合并

