---
layout: post
title: 配置插件来设置默认图片粘贴位置
categories: 软件配置
description: second commit
keywords: 配置插件，默认图片粘贴位置
mermaid: false
sequence: false
flow: false
mathjax: false
mindmap: false
mindmap2: false
---


# 配置插件来设置默认图片粘贴位置
在VS Code中编辑Markdown文章时，你可以通过配置插件或使用一些快捷键来设置默认图片粘贴位置。以下是两种方法：
# Markdown Image

## Markdown 图片扩展

此插件旨在改善插入和引用本地图片的体验。它允许类似于 Typora 的体验，您只需复制本地图片，然后粘贴到 MD 文档中，插件将在插入文档之前自动格式化图片名称和路径。

安装插件后，进入配置界面。两个主要的配置区域是：

### 基础图片名格式
如果您不想深入研究这些变量，可以直接在输入框中粘贴以下 CX 的配置：

```plaintext
${mdname}/IMG_${YY}${MM}${DD}-${HH}${mm}${ss}${mss}
```

### 图片文件夹
上述变量将使用此插件插入的本地图片复制到与 MD 文档相同文件夹中的 `.assets_IMG` 文件夹。它将创建一个以当前 MD 文档命名的文件夹来存储图片，图片文件名将以当前时间命名，如 `IMG_20211216-093507812`（用于排序）。

这类似于 Typora 选项中的 "将图片复制到 /${filename}.assets 文件夹"，但为了更好地管理，它在图片上添加了一个额外的层次，避免在有许多文档时引起混淆。

### 类似于 Typora 的图片引用

配置完成后，您可以在 MD 文档内使用快捷键 `Shift+Alt+V`，直接以相对路径的方式粘贴剪贴板中复制好的图片。

或者在 MD 文档编辑区右键选择 "粘贴图片" 即可。

## 额外配置（不建议）

您可以配置另一个选项 `Local: Reference Path`，以实现绝对路径引用，但并不推荐。

### 方法一：使用插件

1. 安装 "Markdown All in One" 插件。

   在VS Code的扩展市场中搜索并安装 "Markdown All in One" 插件。

2. 打开 VS Code 设置。

   可以通过快捷键 `Ctrl + ,`（Windows/Linux）或 `Cmd + ,`（Mac）打开设置。

3. 在设置中搜索 "Markdown: Paste Image"。

4. 设置默认的图片粘贴位置。

   在 "Markdown: Paste Image" 配置项中，设置默认的粘贴位置，可以是相对路径或绝对路径。例如：

   ```json
   "markdownPasteImage.relativePath": "./images"
   ```

   这将设置粘贴的图片相对于Markdown文件的路径为 "./images"。





### 方法二：使用快捷键

1. 打开 VS Code 设置。

   快捷键 `Ctrl + ,`（Windows/Linux）或 `Cmd + ,`（Mac）。

2. 在设置中搜索 "Files: Default Language".

3. 在 "Files: Default Language" 设置项中，点击 "Edit in settings.json"。

4. 添加 Markdown 的默认配置。

   在 `settings.json` 文件中，添加以下配置：

   ```json
   "[markdown]": {
       "files.defaultLanguage": "markdown",
       "editor.defaultFormatter": "yzhang.markdown-all-in-one",
       "markdownPasteImage.relativePath": "./images"
   }
   ```

   这里的 `"markdownPasteImage.relativePath"` 配置与方法一中的设置类似，可以根据需要进行调整。

保存设置后，每次粘贴图片时，它们将会被默认保存到指定的位置。

选择适合你的方式进行设置，使得编辑Markdown文件时更加方便。