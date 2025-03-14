# yt-dlp
yt-dlp它是一个功能强大的命令行工具，用于从 YouTube 和其他数百个支持的网站（如Bilibili、Twitter、TikTok等）下载视频或音频。它是经典工具 youtube-dl 的分支项目，但因其更快的更新频率、更丰富的功能以及更好的性能（例如多线程下载）而广受欢迎。

### yt-dlp下载音乐视频可视化菜单一键脚本:

```
bash<(curl -sL https://github.com/3981877/yt-dlp/releases/download/1.0/yt-dlp.sh)
```

---

主要功能特点：

1. 多平台支持

支持 Windows、macOS 和 Linux 系统，通过命令行操作。

2. 格式选择与转换

- 可下载特定分辨率或格式的视频（如 MP4、WebM）。

- 支持提取音频（转为 MP3、AAC 等格式）。

- 自动合并视频和音频流（需安装 ffmpeg）。

3. 批量下载

- 下载整个播放列表或频道内容。

- 自定义下载范围（例如前 10 个视频）。

4. 高级功能

- 绕过地理限制（通过代理）。

- 下载字幕、缩略图或视频描述。

- 支持 Cookie 文件，用于访问会员内容。

---

基础使用示例：

1. 安装
```
   pip install yt-dlp
   ```
3. 下载视频
```
   yt-dlp "视频URL"
   ```
4. 选择格式

- 查看可用格式：
  
```
     yt-dlp -F "视频URL"
  ```
- 下载指定格式（如编号 137+140）：
- 
```
     yt-dlp -f 137+140 "视频URL"
```
4. 提取音频
```
   yt-dlp -x --audio-format mp3 "视频URL"
```
---

注意事项：

1. 法律与道德

下载受版权保护的内容可能违反平台条款或当地法律。请确保你有权下载目标内容，并尊重创作者权益。

2. 依赖项

部分功能（如格式转换）需要安装 ffmpeg。可通过以下命令安装：

Ubuntu/Debian

```
   sudo apt install ffmpeg
   ```
macOS (Homebrew)
```
   brew install ffmpeg
```
3. 更新

定期更新以支持最新网站更改：

```
   yt-dlp --update
```
---
