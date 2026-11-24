自用Windows跳转插件</br></br>
## Feature:<br/>
[Koodo Reader](https://github.com/koodo-reader/koodo-reader)里选中单词，按“词典”按钮，自动弹出[GoldenDict-ng](https://github.com/xiaoyifang/goldendict-ng)单词的popout小窗
## Why:</br>
1.Koodo Reader本地词典功能仅支持mdx，会丢掉图片和音频（不过不知道把mdx和mdd放在它的dictionary文件夹下可不可以）</br>
2.Koodo查词窗口样式太丑，没有css渲染</br>
3.我想保留Koodo查词历史中的句子和章节，以便后续做单词卡用。而这个功能是GoldenDict-ng提供不了的</br></br>
所以让AI帮我写了一个跳转插件，结合二者的功能</br></br>
Koodo Reader本身会拦截非HTTP，goldendict://直接用插件调用查询会被拦截。</br>
于是链路是：插件写一个 .url 快捷方式 → 让 Koodo 用系统方式“打开”它 → Windows 按 URL 里的 goldendict:// 分发给 GoldenDict</br></br>
<img width="536" height="80" alt="image" src="https://github.com/user-attachments/assets/0ecea786-7fca-4716-a1d2-05fe812bb5ef" />

## 操作方式：</br>
1.下载json文件，用记事本打开，复制全部内容</br>
2.打开Koodo设置→插件→添加自定义插件→粘贴→确认</br></br>
## 注意事项：
1.需要Koodo桌面版
2.其他操作系统很可能不能用，可以把代码丢给AI改</br>
3.单词的具体内容会缺失，导出查词历史后有价值的内容只有单词、章节、句子、书名、作者
