# anime-avatars

50 张动漫头像（256×256 原图 + 96×96 移动端缩略图），可直接用于移动端头像选择器。

## 来源

- 图片选自 [learner-lu/anime-face-dataset](https://github.com/learner-lu/anime-face-dataset)（v0.0.1，共 27,588 张）
- 原始图片来源于 konachan.net 与 wallhaven.cc，经数据集作者人工三遍筛选（单人正脸、256×256、色域正常）
- 本仓库为从中均匀抽样挑选的 50 张，仅作个人/应用内头像使用；商用或上架前请确认来源站授权条款

## 结构

```
anime-avatars/
├── avatars/       50 张原图 256×256 JPEG（~1.3MB）
├── thumbs/        50 张缩略图 96×96 JPEG（~185KB，移动端选择器网格用）
├── index.json     清单：id / file / thumb / size / source
└── preview.html   本地预览（浏览器打开）
```

## 移动端接入

```json
[
  { "id": 1, "file": "avatars/avatar_001.jpg", "thumb": "thumbs/avatar_001.jpg", "size": 32063, "source": "anime256/102917-156.jpg" }
]
```

- 选择器网格加载 `thumbs/`（单张约 3.7KB，50 张共 ~185KB）
- 选中后展示/上传用 `avatars/` 原图（256×256，圆形裁切也清晰）

## 许可

本仓库内图片版权归原作者（konachan.net / wallhaven.cc 投稿者）所有，请勿用于违反来源站条款的场景。
