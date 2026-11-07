# newspaper · 报纸导航 (PaperNav)

杜绝加密空间旗下子站：**newspaper.mydjjm.cn**

## 内容

中外主流报纸与刊物导航，6 大类共 46 条官方站点链接：

- 党政大报（8）：人民日报、光明日报、经济日报、解放军报、学习时报、法治日报、工人日报、中国青年报
- 都市晚报（8）：北京晚报、新民晚报、羊城晚报、今晚报、扬子晚报、钱江晚报、楚天都市报、南方都市报
- 财经证券（8）：中证报、上证报、证券时报、证券日报、中国经营报、第一财经、21 经济、经济观察报
- 文摘周刊（8）：参考消息、环球时报、南方周末、瞭望、半月谈、中国新闻周刊、三联生活周刊、瞭望东方周刊
- 地方党报（6）：解放日报、南方日报、广州日报、北京日报、天津日报、新华日报
- 国际大报（8）：NYT、WSJ、FT、Guardian、Telegraph、朝日、读卖、The Economist

## 技术

- 纯静态单页，无后端、无数据库、无外部依赖
- 数据集中在 `index.html` 底部 `const SITES = [...]`，改一条即改一卡
- 分类标签与卡片网格由同一数据驱动自动渲染
- 深色主题，与 news-nav / media-nav / 主站同一套设计语言
- 左上角「← 返回主页」固定回 `https://mydjjm.cn/`

## 部署

- 仓库：`qinvision/newspaper`
- 发布：GitHub Pages，`main` 分支根目录
- 自定义域名：`newspaper.mydjjm.cn`（见 CNAME）
- DNS：阿里云万网 `newspaper` CNAME → `qinvision.github.io`
- HTTPS：Pages 设置里勾选 Enforce HTTPS

## 边界

- 本站不转载、不存储任何新闻内容，所有链接均跳转到各媒体官网
- 不收录聚合器、热榜工具、RSS 阅读器（那部分归 news-nav）
