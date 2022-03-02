# 语法规则

## Overview

- 只能有一个 root 元素；

- 序言 prolog

  - `<?xml version="1.0" encoding="UTF-8"?>`
  - 可选。如果有，必须在最前面；
  - 不是 XML document 的一部分；
  - `encoding`：默认为 `UTF-8`；

- 所有元素都必须有一个结束标签：

  ```xml
  <p>This is a paragraph.</p>
  <br />
  ```

- 标签(tag) 大小写敏感；

- 元素(element) 必须正确嵌套；

- 属性的值 (attribute value) 必须使用双引号括起来；

- 实体引用（entity reference）

  - 有些字符在 XML 有特殊意义。使用前需要替换成 entity reference
  - `&lt;`： `<`，less than
  - `&gt;`：`>`，greater than
  - `&amp;`：`&`，ampersand
  - `&apos;`：`'`，apostrophe
  - `&quot;`：`"`，quotation mark

- 注释

  ```xml
  # 正确
  <!-- This is a comment -->
  
  # 错误 -- 不允许在内容中间使用
  <!-- This is an invalid -- comment -->
  ```

- 换行

  - Windows：CR+LF

    Unix and Mac OSX：LF

    XML：LF.

## References

- [XML Syntax Rules](https://www.w3schools.com/xml/xml_syntax.asp)
