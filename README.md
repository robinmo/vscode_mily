# 米粒鼓励师

在 VS Code 中连续写代码30分钟（时间可配置），会有米粒提醒你该休息啦~

本项目有个小彩蛋，等你们使用时就会发现啦！嘻嘻～～

## 使用

除了每过一小时会自动弹出提醒页面，也可以按 `F1`, 然后输入 `mily: 打开提醒页面`来打开提醒页面

![usage](images/usage.png)

## 配置

* `mily.reminderViewIntervalInMinutes`: 展示提醒页面的时间间隔（分钟）。(默认值为**60**)
* `mily.title`: 提示文字。 (默认值为**亲爱的，亲爱的，代码写久了，该休息啦~**)
* `mily.type`: default (默认图)；url (图片地址)。(默认值为**default**)
* `mily.customImages`: 配置图片数组（需要搭配mily.type为url） (默认值为**默认图片**)

```
如下例子，使用自定义图片：
"mily.type": "url",
"mily.customImages": [
    "http://test.jpg"
]
```
## 如何使用本地图片作为展示图片

* vscode不允许读取外部文件路径，所以只能自己去替换插件内的图片。替换步骤如下：
  
  1、找到vscode插件安装的地方 (如mac 在~/.vscode/extensions/milyyy.mily-{version})
  
  2、替换images/mily内图片
