---
title: hello
abbrlink: 13522
date: 2024-11-08 21:30:53
comment: true
cover: https://api.luoh-an.me/PicLibrary/AnimeImage?t=wallpaper&r=image
tags:
---

# 1.前言

本文是对于[luohAPI](https://api.luoh-an.me/)的文档介绍，便于更方便的使用

---

# 2.介绍

## 2.1 InfoHub

### 2.1.1 HistoryToday

{% fold 'title' open %}
**接口地址**  <span id="HistoryToday" onclick="CopyApiLink()"><code class="API">`https://api.luoh-an.me/InfoHub/HistoryToday/`</code></span>
**请求方法** `GET` <br>
**请求参数说明**

<div class="APITable">

| 名称 | 必填 | 类型 | 说明 |
| - | - | - | - |
| date | 否 | string | `{month}{day}` <br> 例如 `1010` 及表示 `十月十日`的历史 <br> `0101` 即表示 `一月一日` 的历史 <br> 不填写时默认为今日日期 |

</div>

<br>

**返回示例**

```json
{
    "year": "1731",
    "title": "英国化学家和物理学家 卡文迪许 出生",
    "festival": "辛亥革命纪念日",
    "type": "诞生",
    "desc": "卡文迪许是英国化学家和物理学家。他出生贵族，继承了叔伯和父亲的遗产后成为英国巨富之一。但他生活简朴，全心投身于科学研究，在物理化学领域获得了杰出成就，硝酸就是他发现的。",
    "cover": true,
    "recommed": true,
    "pic_caledar": "http://baike.bdimg.com/cms/rc/r/image/2014-08-31/c83fa196d6f0d95fbd1292d0ecd11e22_80_80.jpg",
    "pic_share": "http://baike.bdimg.com/cms/rc/r/image/2014-08-31/a04b2298b06e097a216d053b888c10fe_360_212.jpg",
    "pic_idex": "http://baike.bdimg.com/cms/rc/r/image/2014-08-31/23c0660eb476f5e8ac614f9dea4a048c_134_100.jpg",
    "baike": "http://baike.baidu.com/subview/19638/14698117.htm"
}
```

<br>

**返回参数说明**
<div class="APITable">

| 名称 | 类型 | 说明 |
| - | - | - |
| year | string | 年份 |
| title | string | 该历史精简概括 |
| festival | string | 节日 |
| type | string | 历史类型 |
| desc | string | 详细介绍 |
| cover | boolean | 是否有图片 |
| recommed | boolean | 是否推荐 |
| baike | string | 百科链接 |

</div>

*其余不做解释*

<br>

**请求示例** 
<br> <span id="HistoryToday" onclick="CopyApiLink()"><code class="API">`https://api.luoh-an.me/InfoHub/HistoryToday/`</code></span>

 {% endfold %}