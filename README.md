自用Windows跳转插件</br></br>
## Feature:
## Why:</br>
1.Koodo Reader本地词典功能仅支持mdx，会丢掉图片和音频</br>
2.Koodo查词窗口样式太丑，没有css渲染</br>
3.我想保留Koodo查词历史中的句子和章节，以便后续做单词卡用。而这个功能是GoldenDict-ng提供不了的</br>
（所以单词的具体内容会丢失，导出查词历史后有价值的内容只有单词、章节、句子、书名、作者）</br></br>
所以让AI帮我写了一个跳转插件</br></br>
Koodo Reader本身会拦截非[HTTP](https://)，goldendict://直接用插件调用会被拦截。</br>
于是链路是：插件写一个 .url 快捷方式 → 让 Koodo 用系统方式“打开”它 → Windows 按 URL 里的 goldendict:// 分发给 GoldenDict</br></br>
## 操作方式：</br>
1.下载json文件，用记事本打开，复制全部内容</br>
2.打开Koodo设置→插件→添加自定义插件→粘贴→确认
