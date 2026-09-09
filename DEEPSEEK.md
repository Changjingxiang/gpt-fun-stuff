# Deepseek鲸鱼娘

一只运行时埋头吃白饭的 Codex 桌面宠物。蓝发、鲸尾、女仆裙，抱着饭碗陪你工作。

![运行时吃白饭](eating.gif)

## 下载与安装

从仓库的 Releases 下载 `Deepseek-whale-girl-v1.0.0.zip`，解压后把 `deepseek-rice-whale` 文件夹复制到：

- Windows：`%USERPROFILE%\.codex\pets\`
- macOS / Linux：`~/.codex/pets/`

在 Codex 宠物选择器中选择 **Deepseek鲸鱼娘**。若列表未刷新，重新打开 Codex。

也可以直接下载本目录中的 `deepseek-rice-whale` 文件夹。

## 动作

|状态|表现|帧数|
|---|---|---|
|待机|抱空碗、眨眼等饭|6|
|向右移动|抱碗小步走|8|
|向左移动|抱碗小步走|8|
|挥手|拿着碗打招呼|4|
|跳跃|抱碗开心跳起|5|
|出错|检查空碗，失落垂耳|8|
|等待确认|递碗请求添饭|6|
|任务运行|夹白饭、送入口、鼓腮咀嚼|6|
|审查 / 思考|停筷思考、歪头|6|

## 预览

下载并用浏览器打开 [preview.html](preview.html)，可切换全部状态、暂停动画、切换背景。

![全部动作](spritesheet-preview.png)

## 制作记录

使用 GPT 与内置图像生成工具，依据用户提供的角色参考创作；经绿幕处理、逐帧提取和对齐，合成为透明无损 WebP。生成提示词见 [prompts.json](prompts.json)。

规格：1536×1872，8列×9行，每格192×208，共57个有效帧。尺寸、透明通道、空白格、帧边界和绿底残留检查已通过，详见 [validation.json](validation.json)。尚未完成 Codex 原生宠物窗口的事件触发测试。

休眠、拖动和点击护食未作为独立事件实现；当前采用的标准9行格式没有对应行。跳跃的具体触发由 Codex 决定。

这是 DeepSeek 鲸鱼娘的非官方同人创作，与 DeepSeek、OpenAI 无官方关联。
