# 上传页面图片 / 视频到 CDN

> 页面和文档里的大图片、视频**不建议直接塞进代码仓库**：先把文件上传到 CDN，
> 拿到返回的 URL，再在 Markdown 里引用。这样仓库保持轻量，页面加载也更快。

!!! note "本页内容待补充"
    本页目前是文档骨架，用于保证导航结构完整；上传界面的逐步操作与截图正在整理中。

## 为什么走 CDN

| 引用方式 | 仓库体积 | 页面加载 | 适用场景 |
|---|---|---|---|
| 直接提交到仓库 | 持续膨胀，clone 变慢 | 依赖 Pages 带宽 | 图标等极小文件 |
| 上传到 CDN 后引用 URL | 几乎不变 | 就近分发，更快 | 截图、演示视频、大图 |

## 引用方式

上传拿到 URL 后，按标准 Markdown 语法引用即可：

```markdown
![image](https://serve.nutshellai.cn/publish/auto/tutorial/13_xiaomo_control_hub_01.jpg)
```

视频同理，用 HTML 的 `<video>` 标签或对应平台嵌入代码引用 CDN 地址。

## 相关阅读

- [万能捷径：小莫助理](tutorial/13_xiaomo_control_hub.md) —— 该页的截图即为 CDN 引用的实际效果
- [项目文件打包下载](tutorial/18_package_download_project.md)
