# 鱼群背景约会邀请网站（电脑 + 手机版优化版）

## 本版重点

- 电脑端：两条视频交替叠化循环，优先使用 1080P。
- 手机版和微信端：使用独立的 720P 单视频自动循环，避免两条视频同时抢占播放权限。
- 手机视频直接写入 HTML 的 `src`，并启用：
  - `autoplay`
  - `muted`
  - `playsinline`
  - `webkit-playsinline`
  - 微信 X5 内核相关属性
- 手机版末尾增加轻微淡入淡出遮罩，减弱循环跳变。
- 手机版布局改为约会界面在上、完整鱼群画面在下。
- 年月日和项目选择、门票图片生成等功能保持不变。

## 上传 GitHub

请把本文件夹里的所有文件一起上传到仓库根目录：

```text
index.html
fish-loop-1080p.mp4
fish-loop-720p.mp4
fish-poster-hq.jpg
.nojekyll
.gitignore
README.md
```

不要漏掉视频文件。

## 开启 GitHub Pages

1. 仓库 `Settings`
2. `Pages`
3. `Source`：Deploy from a branch
4. Branch：main
5. Folder：/ (root)
6. Save

生成 HTTPS 链接后，可以直接发到微信打开。
