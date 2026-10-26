# 微信读书助手

为支持 Skills 的 AI 助手提供微信读书能力：搜索书籍、查看书架、分析阅读偏好、筛选短书，以及查看笔记、划线和书评。

本仓库仅包含一个 skill：**weread-skills**（版本 **1.0.5**）。

## 安装

```bash
npx skills add shunforever4/skills-introduction-to-github -g
```

## 配置

1. 前往 [微信读书 Skills](https://weread.qq.com/r/weread-skills) 获取个人 API Key。
2. 在运行 AI 助手的环境中，将密钥配置为 `WEREAD_API_KEY`。在云环境中，使用环境设置的 Secrets 安全填写。
3. 确保环境允许通过 HTTPS 访问 `i.weread.qq.com`。

密钥绑定你的微信读书身份。请勿将真实密钥写入仓库、提交记录或公开聊天；无需安装应用依赖，也无需启动本地服务。

## 使用示例

安装并配置后，直接向 AI 助手提出请求：

- 帮我扫描书架，推荐几本篇幅短、读起来快的书。
- 浏览我读完的书，分析我的阅读偏好。
- 看看我这个月读了多久。
- 导出我在某本书里的划线。
- 搜索书籍，并查看目录或书评。

## 技能文件

| 文件 | 用途 |
| --- | --- |
| [SKILL.md](skills/weread-skills/SKILL.md) | 技能入口、接口规范与鉴权说明 |
| [shelf.md](skills/weread-skills/shelf.md) | 书架管理 |
| [book.md](skills/weread-skills/book.md) | 书籍详情、目录与阅读进度 |
| [readdata.md](skills/weread-skills/readdata.md) | 阅读统计与偏好分析 |
| [notes.md](skills/weread-skills/notes.md) | 笔记和划线 |
| [search.md](skills/weread-skills/search.md) | 搜索书籍 |
| [review.md](skills/weread-skills/review.md) | 书籍点评 |
| [discover.md](skills/weread-skills/discover.md) | 推荐与发现 |
| [profile.md](skills/weread-skills/profile.md) | 用户阅读概况与统计组合工作流 |

## 来源与许可

技能文件原样保留自 [Tencent/WeChatReading](https://github.com/Tencent/WeChatReading)，对应上游提交 `d98e66ee60a8c7bcd35da549d0643c4470439643`，Copyright © 2026 Tencent。

技能及上游许可证采用 [Apache-2.0](LICENSE)。本仓库新增中文项目说明与安装入口，保留上游技能文件的名称，以兼容现有安装与调用方式。
