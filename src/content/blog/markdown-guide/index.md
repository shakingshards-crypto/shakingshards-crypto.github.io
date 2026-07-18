---
title: Markdown Syntax Guide
description: Examples of all Markdown syntax supported by this theme, including headings, lists, tables, code blocks, blockquotes, images, etc.
date: 2026-06-10
tags: [Markdown, Tutorial]
category: Tutorial
cover: https://images.unsplash.com/photo-1517694712202-14dd9538aa97?w=1200
---

## Headings

# H1 Heading
## H2 Heading
### H3 Heading
#### H4 Heading

## Text Formatting

**Bold**, *Italic*, ~~Strikethrough~~, `Inline Code`, [Hyperlink](https://astro.build).

## Lists

### Unordered List

- First item
- Second item
  - Nested item
  - Another nested item
- Third item

### Ordered List

1. Step one
2. Step two
3. Step three

### Task List

- [x] Completed task
- [ ] Todo item
- [ ] Another todo item

## Blockquotes

> This is a blockquote.
>
> It can span multiple lines and paragraphs.
>
> > Nested blockquote

## Tables

| Name | Age | City |
|------|------|------|
| John | 25 | New York |
| Emma | 30 | London |
| Mike | 28 | Tokyo |

## Code Blocks

### TypeScript

```typescript
interface User {
  name: string;
  age: number;
  email: string;
}

const getUser = (id: number): Promise<User> => {
  return fetch(`/api/users/${id}`).then(res => res.json());
};
```

### Python

```python
def fibonacci(n: int) -> list[int]:
    a, b = 0, 1
    result = []
    for _ in range(n):
        result.append(a)
        a, b = b, a + b
    return result
```

### CSS

```css
.card {
  border-radius: 12px;
  padding: 24px;
  background: var(--color-card);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
}
```

### Shell

```bash
#!/bin/bash
for file in *.md; do
  echo "Processing $file"
  sed -i 's/foo/bar/g' "$file"
done
```

Code blocks support language tags, copy-to-clipboard, and line numbers. The copy button is located in the top-right corner.

## Horizontal Rule

---

## Images

![Scenery](https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=800)

## Footnotes

Here is a simple footnote[^1].

[^1]: This is the footnote content.

## HTML Embedding

<div class="bg-blue-50 dark:bg-blue-900/20 border border-blue-200 dark:border-blue-800 rounded-xl p-4 text-sm">
  Tip: This theme supports embedding HTML tags within Markdown.
</div>
