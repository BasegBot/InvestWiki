---
layout: "home"
---

# toffee wiki

Official WIP wiki!!

## Pages

[Example alternative language](/wiki/ja/)

Eventually there will be other things!!!

## Markdown Support

some random examples!

### Syntax Highlighting

```jsx
export default function RenderMarkdown({ children }: RenderMarkdownProps) {
  return (
    <ReactMarkdown
      remarkPlugins={[remarkGfm]}
      rehypePlugins={[rehypeHighlight, rehypeSlug]}
    >
      {children}
    </ReactMarkdown>
  );
}
```

### Images

![image alt](img/4x.webp "Image title text!")

### GFM

#### Autolink literals

www.example.com, <https://example.com>, and contact@example.com.

#### Footnote

A note[^1]

[^1]: Big note.

#### Strikethrough

~one~ or ~~two~~ tildes.

#### Table

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

#### Tasklist

- [ ] to do
- [x] done
