# AO3 独伊读者用过滤器

这是一个 AO3 Site Skin，用于屏蔽部分 CP 和标签。

由于在AO3阅读tag中的文章时经常被某些CP创到，所以做了这个皮肤，适合独伊读者使用。

## 功能

屏蔽以下 CP：

- 伊独
- 伊双子
- 芋兄弟
- 爱丽舍

## 使用方法

1. 复制 `ao3-blocklist.css` 中的代码  
2. 打开 AO3 → Dashboard → Skins  
3. 新建 Site Skin  
4. 粘贴代码并保存

## 原理

利用 CSS `:has()` 选择器隐藏包含特定 tag 的作品。

### 说明

第一段用于屏蔽所有匿名作者的作品，如果不需要可以删除。
第二段用于屏蔽指定标签，可以根据需要自行添加或修改 tag。

## 如何添加新的 tag
.blurb:has(a[href$="/tags/TAG_NAME/works"])
- 空格 `" "` → `%20`
- 斜杠 `"/"` → `*s*`
- 例：
- Germany/North Italy (Hetalia)
- 对应tag URL为：
- Germany*s*North%20Italy%20(Hetalia)
