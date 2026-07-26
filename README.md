# zyz-opener

左宥之「开场白管理」远程页面。角色卡里只放本地壳 `shell.html`，UI / 索引改这里即可，不用反复重导卡。

## 远程地址

- jsDelivr：`https://cdn.jsdelivr.net/gh/fchris1219-del/zyz-opener@main/opener.html`
- GitHub Pages：`https://fchris1219-del.github.io/zyz-opener/opener.html`

## 用法

1. 打开角色卡正则「【开场白】左宥之开场白管理…」
2. 把替换内容整段换成仓库里的 [`shell.html`](./shell.html)（格式同同层微博远程壳：`document.write` 整页注入）
3. 之后改索引 / 样式只改 `opener.html` 并 push

## 文件

| 文件 | 说明 |
|------|------|
| `opener.html` | 远程完整开场白管理页（票根 / 观影规则 / 电影开场） |
| `shell.html` | 酒馆正则本地壳：重试拉取 + `document.write` 注入 |

本地壳优先 jsDelivr，失败则打 GitHub Pages；带重试、超时与时间戳防缓存。
