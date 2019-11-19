---
views:
    redovisa:
        region: sidebar-left
        template: anax/v2/block/default
        data:
            meta:
                type: single
                route: block/om-redovisa

    mumin:
        region: sidebar-right
        template: anax/v2/block/default
        data:
            meta:
                type: single
                route: block/om-mumin
---
Heading1
=========================
Lek med markdown


type|.md syntax|HTML tag
:---:|:------:|:------:
Heading1|   `#`, `===`  |`<h1></h1>`
Heading2|   `##`, `---` |`<h2></h2>`
Heading3|`###`|`<h3></h3>`
Heading4|`####`|`<h4></h4>`
Heading5|`#####`|`<h5></h5>`
Heading6|`######`|`<h6></h6>`
Italics|`* *`, `_ _`
Unordered list|`*`, `+`, `-`|`<ul><li></li></ul>`
Ordered list|`1.`|`<ol><li></li></ol>`
Horizontal rule|`---`, `***`, `___`|`<hr>`
Inline code|` ` ` `|`<code></code>`
Block code| ` ``` ``` `| ?
Blockquotes|`>`|`<blockquote></blockquote>`
