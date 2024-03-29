---
created: 2023-07-08
aliases: 
tags:
  - coding
  - notetaking
---
**Some lesser-supported Markdown syntaxes**

While nearly **all** [[Markdown]] clients support the basic markdown syntax, there are some “official” extended syntaxes that are not as widely supported. These are, unfortunately, also things that applications have come up with their own non-standard ways to implement, including [[Notion Markdown]] and [[Obsidian]]-flavored markdown.

Things commonly added:

- Tables
    
    ```
    | Header | Second Header, much longer | Third Header |
    | :---        |    :----:   |          ---: |
    | Left-aligned text | Centered text! | Right-aligned text.  |
    | A3  | B3 | C3 |
    ```
    
- Fenced Code Blocks
    
    ```
    ```javascript
    let i = 0;
    ```
    ```
    
- Footnotes
    
    ```
    My footnoted word[^1].
    
    [^1]: Footnote for that.
    ```
    
- Highlights
    
    ```
    The ==highlighted phrase== is in double equals signs.
    ```
    
- Superscript/Subscript
    
    ```
    3^2 = 9
    H~2~O = water
    ```
    
- Em and En-dashes
    
    ```
    -- en dash
    --- em dash
    ```
    
- Strikethrough
    
    ```
    This is ~~lame~~ cool.
    ```

Extended Markdown Specs/support:

- Github-flavored Markdown
    - A strict superset of CommonMark
- Kramdown
- Showdown
- MultiMarkdown

****
### Source

[Extended Syntax | Markdown Guide](https://www.markdownguide.org/extended-syntax/#definition-lists)

[Comparison of features in various Markdown flavors](https://gist.github.com/vimtaai/99f8c89e7d3d02a362117284684baa0f)

### Related
- [[Markdown]] 
- [[Mermaid]] 
- [[Markdown Processers]]