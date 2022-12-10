# 4ov-scripts

[4399 on vscode](https://github.com/dsy4567/4399-on-vscode) 的 HTML 代码片段仓库

# HTML 代码片段被用来做什么

它们会被 [4399 on vscode](https://github.com/dsy4567/4399-on-vscode) 注入
`webview` 里, 用来优化游戏体验, 以及为
[4399 on vscode](https://github.com/dsy4567/4399-on-vscode) 添加新功能

# 快速上手

```html
<!-- foobar.html -->
<!--

版权声明
===license===
XXX LICENSE

Copyright (c) <year> <your name>

balalalalalalalalalala...
===/license/===


清单声明
===manifest===
{
    "author": "https://githbu.com/xxx",
    "description": "balalalalalalalalalala...",
    "id": "xxx.foobar",
    "name": "foobar"
}
===/manifest/===

-->

<script>
    // 常量
    FULL_WEB_SERVER_URI; // 详见 https://code.visualstudio.com/api/advanced-topics/remote-extensions#option-1-use-asexternaluri

    // 打开链接(任选一个)
    fetch("/openUrl/https://www.4399.com/");
    fetch("/openUrl/https://www.4399.com/flash/114514.htm"); // 直接启动游戏
    open("https://www.4399.com/"); // 4399 on vscode 已经帮你重写了这个函数, 等效于 fetch("/openUrl/https://www.4399.com/")

    // 代理, 仅支持 GET 请求
    fetch("/proxy/https://www.4399.com/");

    console.log("Hello world!");
</script>
<style>
    .myDiv{
        color: #66ccff;
    }
</style>
```
# 发布

1. fork 这个仓库
2. 在仓库根目录下创建一个文件夹, 名字随便
3. 在这个文件夹里创建 `LICENSE`, `README.md`, `<dir-name>.html` 以及其他必要的文件
4. 修改 `download.html`
5. 发个 PR, 等待合并

# 安装

将 `.html` 文件保存到 `<主目录>/.4ov-data/html-scripts/` 文件夹下
