## 有关 Strapi Markdown 编辑器的提示 —— 来自 IT Team

> 为什么选用 Markdown 的好处建议自行 Google，在此不再赘述  
> *P.S. 本文也是基于 Markdown 写出来的，原文本见[这里](https://raw.githubusercontent.com/61FINTECH/tips-about-strapi-markdown-editor-from-it-team/master/README.md)*

### § 熟悉 Markdown 基础语法
实际上日常能用上的 Markdown 语法只占其很小一部分，无非就是：
* 标题：例如 `h3` 就是 `### 三号标题`（注意井号后面的空格）
* 加粗：`**粗体文字**`
* 外链：`[文字](链接)`
* 贴图：`![图片说明](图片链接)`（但 Strapi 支持直接粘贴图片，所以基本可以省了）
* 列表：有序直接写 `1. 2. 3.`，无序用 `*` 或者 `-` 就好

更多常用语法请参考以下教程：
* [认识与入门 Markdown](https://sspai.com/post/25137)
* [献给写作者的 Markdown 新手指南](https://www.jianshu.com/p/q81RER)
* *更多请自行 Google，教程多到贴不完*

### § 本地编辑软件
如果你要长篇大论，觉得 Strapi 的编辑器不够好用，想在本地编辑完后再粘贴回去，没问题。  
为此我专门调研并亲自试用了近十款主流的 Markdown 编辑器，选出如下两款：
* [Haroopress](http://pad.haroopress.com)：跟 Strapi 的编辑器一样，左侧编辑右侧预览
* [Typora](https://typora.io/)：完全单屏，编辑预览二合为一

> 请注意，图片还是得在 Strapi 中复制粘贴上传，本地编辑主要是为了行文、构文更加流畅直观  
>（实际上 Strapi 的编辑器已是数十款 CMS 中综合水平最好的了，亲测）

### § 工具推荐
* [Ditto](https://ditto-cp.sourceforge.io)：历史剪贴板（编辑必备神器）
* [f.lux](https://justgetflux.com)：护眼神器

> 更多请自行 Google，或参考这个[知乎帖](https://www.zhihu.com/question/22919326)

### § 已知 bug
* 鼠标点击工具栏中的快捷操作后，预览面板中没有任何变化
    - **原因**：编辑器是基于监听键盘按键事件来同步预览面板的
    - **解决方案**：随便按一下回车之类的即可触发刷新预览面板内容
    - **根本解决方案**：熟记 Markdown 的基本语法，不使用工具栏

* 选中文字后点击工具栏中的“链接”操作，文字竟然放在了 link 的位置
    - **原因**：这的确与常规的操作不一致，但没办法
    - **解决方案**：不使用工具栏的“链接”操作
    - **根本解决方案**：熟记 Markdown 的基本语法，不使用工具栏
