<h3 align="center">朗译 ( Lang Translator )</h3>

<p align="center">让你沉浸在阅读中的划词翻译利器</p>
<p align="center"><a href="https://chrome.google.com/webstore/detail/%E7%A9%86%E8%AF%91/mcfdomppancgaladcgflcgahbgcgbagb"><img src="https://raw.githubusercontent.com/LangInteger/lang-translator/master/app/images/icon-128.png" border="0" /></a></p>

<p align="center">传承经典（穆译），启迪未来</p>

### Building from source

Install nvm for node version control:

- for Windows, install [nvm-windows
](https://github.com/coreybutler/nvm-windows)
- for OS X & Linux, install [nvm](https://github.com/nvm-sh/nvm)

```shell
nvm install 10.0.0
nvm use 10.0.0
npm install -g gulp@3.9.0
npm install --save-dev gulp@3.9.0
gulp build
```

### RoadMap

- [x] 添加单词发音 2022-03-24
- [ ] 支持阅读 PDF 文件时候取词
- [ ] 升级 chrome extension manifest v2 为 v3
- [ ] 添加可变颜色背景

### Appendix

#### A ReadMe of 穆译

```
### 穆译的信条

> 不要让划词翻译干扰阅读状态

所以页面划词翻译的结果不会显示在词语附近遮挡住你的阅读材料，而是显示在页面的右上角，余光扫一眼便立即回到阅读，稍后它便会自己关闭。

### 如何使用穆译

- 如果要查询页面中的某个单词，双击选中，单词的释义会显示在页面右上角，然后自动在几秒后消失（你可以在设置页面调整时间长短）。
- 要前往扩展设置页面，可以点击扩展图标打开翻译窗口，然后点击窗口中的齿轮图标。
- 在翻译窗口中也可以进行翻译，输入要翻译的内容，翻译结果会自动呈现。在翻译窗口的输入框中按下 `ESC`，会清除当前的输入内容，
  方便查询新的单词。如果输入框没有内容，`ESC` 会关闭翻译窗口。
- 如果想在某个网站上禁用划词翻译，可以在翻译窗口中取消勾选「在 xxx 启用划词翻译」，
  如果想在全部页面禁用划词翻译，请在设置页面中的取消勾选「默认」条目。
- 如果你想对页面中的某个链接中的单词划词翻译，可以使用快捷键 `Ctrl + Shift + L` 进入链接划词模式，
  此时所有的链接的跳转会失效，你可以对其进行划词翻译，划词后，会自动退出链接划词模式。
  这个快捷键你可以在 Chrome 的快捷键设置里面更改（可以在扩展设置页面点击「更改快捷键」按钮前往设置）。
- 扩展的翻译窗口打开时会自动显示上一次翻译（包括页面划词）的内容，即便你关闭了页面划词翻译，
  仍然可以在页面中选中文本内容后，点击扩展图标打开翻译窗口查看选中内容的翻译结果。
  页面划词翻译只会显示单个英语单词的翻译结果，所以如果你想查看页面上某个句子（包括中文）的翻译结果，
  这个特性会是一个很好的补充。

----

穆译使用[有道翻译](http://translate.youdao.com/)提供词典和翻译服务。

穆译是一个开源应用，如果你想审查代码或者参与开发，请访问

https://github.com/greatghoul/smooth-translator
```
