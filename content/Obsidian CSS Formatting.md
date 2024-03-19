---
created: 2024-01-29
tags:
  - notetaking
  - coding
aliases:
---
This note is *both* a reference and example for how things are formatted. 

> [!NOTE] Note to Non-Aaron-types
> The reference code below only styles my actual [[Obsidian]], not what you're seeing if you're seeing this online. Again these are for **me**.
# H1 - Page Titles
Almost **never** used *outside* of page titles.

## H2 - Looks like this!
With text below, usually!

> This is a quote.
> *- some dude*

A list:
- Mary
- Had
	- A
- _little_
- lamb
1. Or
2. Two
### H3 - Another useful heading.
All the time[^1]. You like to use H3 here in Obsidian. Here's a table.

| Item | Changed? |
| ---- | ---- |
| Block |  |
| Blockquote | ✅ |
| Callout | ✅ |
| Code |  |
| Embed |  |
| File |  |
| Footnote |  |
| Headings | ✅ |
| Horizontal Rule |  |
| Inline Title |  |
| Link |  |
| List |  |
| Properties |  |
| Table |  |
| Tag |  |
[^1]: for reasons.

#### H4 - Now you're getting to the dregs
Very rarely is there a good use for H4.

Inline `preformatted` aka "code" in the [[Notion]] vernacular. [External Notion Link](https://notion.so)

## The Actual Code
From `.obsidian > snippets > aaron-style.css`:
```css
body{
	--callout-border-width: 1px;
	--callout-radius: 0.5em;
	--h2-color: steelblue;
	--h3-color: rgb(152, 182, 222);
	--h4-color: rgb(159, 145, 247);

	--h1-size: 2.25em;
	--h2-size: 2em;
	--h3-size: 1.75em;
	--h4-size: 1.5em;

	--bold-color: khaki;
	--bold-weight: bolder;
	--italic-color: peachpuff;

	--blockquote-background-color: rgb(30, 30, 57);
	--blockquote-border-thickness: 3px;
  
	--file-line-width: 950px;
}

.callout-content > p{
	margin-top: 8px;
	margin-bottom: 0px;
}
  

.cm-inline-code{
	color: lightsalmon !important;
}
```

****
### Source
- self
- https://docs.obsidian.md/Reference/CSS+variables/CSS+variables

### Related
- [[HTML CSS JavaScript]]
- [[Obsidian Niceties]]