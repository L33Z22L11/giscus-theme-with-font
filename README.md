# Giscus Theme / Giscus 主题

This repository provides custom CSS for the Giscus comment system's `data-theme` field.

该存储库提供了用于 Giscus 评论系统的 `data-theme` 字段的自定义 CSS。

## Font Themes / 字体主题

For more detailed instructions, please refer to the [ADVANCED-USAGE.md](https://github.com/giscus/giscus/blob/main/ADVANCED-USAGE.md#data-theme) file in the [giscus](https://github.com/giscus/giscus) repository.

有关更详细的说明，请参阅 [giscus](https://github.com/giscus/giscus) 存储库中的 [ADVANCED-USAGE.md](https://github.com/giscus/giscus/blob/main/ADVANCED-USAGE.md#data-theme) 文件。

To use a custom font theme, configure the `data-theme` field in Giscus with one of the following links:

要使用自定义字体主题，请在 Giscus 中的 `data-theme` 字段中配置以下链接之一：

### LXGW-wenkai / 霞鹜文楷

Use the following CSS file for the LXGW-wenkai font theme:

使用以下 CSS 文件作为 LXGW-wenkai 字体主题：

https://cdn.jsdelivr.net/gh/L33Z22L11/giscus-theme/lxgw-wenkai.css

### HarmonyOS Sans / 鸿蒙字体

Use the following CSS file for the HarmonyOS Sans font theme:

使用以下 CSS 文件作为 HarmonyOS Sans 字体主题：

https://cdn.jsdelivr.net/gh/L33Z22L11/giscus-theme/harmonyos-sans.css

> [!TIP]
> You can also replace the domain with `fastly.jsdelivr.net`, `gcore.jsdelivr.net`, or other alternatives.
>
> 您还可以将域名替换为 `fastly.jsdelivr.net`、`gcore.jsdelivr.net` 或其他可用的选项。

## Usage / 使用方法

If your Hexo theme (e.g. [Stellar](https://github.com/xaoxuu/hexo-theme-stellar)) supports Giscus, you can configure Giscus with a font theme using a configuration similar to the following:

如果您的 Hexo 主题（如 [Stellar](https://github.com/xaoxuu/hexo-theme-stellar)）支持 Giscus，则可以使用类似以下配置的方式配置 Giscus 的字体主题：

```yaml
comments:
  service: giscus
  giscus:
    data-repo: #
    data-category: #
    data-theme: https://cdn.jsdelivr.net/gh/L33Z22L11/giscus-theme/lxgw-wenkai.css
```

Otherwise, add the following JavaScript code to your web page:

否则，将以下 JavaScript 代码添加到您的网页中：

```html
<script src="https://giscus.app/client.js"
        data-repo="[在此输入仓库]"
        data-category="[在此输入分类名]"
        data-theme="https://cdn.jsdelivr.net/gh/L33Z22L11/giscus-theme/lxgw-wenkai.css" 
        data-lang="zh-CN"
        crossorigin="anonymous"
        async>
</script>
```

Please note that you need to replace the placeholders `[在此输入仓库]` and `[在此输入分类名]` with the appropriate values for your repository and category.

请注意，您需要将 `[在此输入仓库]` 和 `[在此输入分类名]` 的占位符替换为您的存储库和分类的正确值。

This will enable Giscus with the specified font theme on your website.

这将在您的网站上启用使用指定字体主题的 Giscus。
