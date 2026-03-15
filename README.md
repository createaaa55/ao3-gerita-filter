# AO3 独伊读者用过滤器

这是一个 AO3 Site Skin，用于屏蔽部分 CP 和标签。适合独伊读者使用。

## 功能

屏蔽以下 CP：

- 伊  独
- 伊  双  子
- 芋  兄  弟
- 爱  丽  舍

## 使用方法

1. 打开 `ao3-gerita-filter.css`
2. 用任意文本编辑器打开该文件（例如 Windows 的“记事本”）
3. 复制文件中的全部代码
4. 登录 AO3
5. 进入 Dashboard → Skins
6. 创建新的 Site Skin
7. 粘贴代码并保存
8. 如果不会打开文件，也可以直接在 GitHub 页面中打开该文件并复制里面的代码
9. 需要和其他皮肤一起使用可以直接粘贴到代码结尾（应该）

## 说明

第一段用于屏蔽所有匿名作者的作品，如果不需要可以删除。

第二段用于屏蔽指定标签。本方法只能屏蔽与代码中完全相同的标签。由于作者本人已 mute 了部分作者，可能未覆盖所有情况，如有需要可以自行添加或修改 tag。

## 如何添加新的 tag
.blurb:has(a[href$="/tags/TAG_NAME/works"])
- 空格 `" "` → `%20`
- 斜杠 `"/"` → `*s*`
- 例：
- `Germany/North Italy (Hetalia)`
- 对应TAG_NAME为：
- `Germany*s*North%20Italy%20(Hetalia)`
  
- 包含汉字的tag请转化为UTF-8编码
-  例：
- `独伊`
- 对应TAG_NAME为：
- `%E7%8B%AC%E4%BC%8A`
