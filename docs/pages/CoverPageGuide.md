# CoverPage

## Cách dùng

Set `coverPage: true` trong index.html

```bash
<script>
  window.$docsify = {
    coverpage: true, // Ở đây
    loadNavbar: true,
    loadSidebar: true,
    subMaxLevel: 3,
  };
</script>
```

Tạo ra 1 `coverPage`

```markdown
<!-- _coverpage.md -->

![logo](_media/icon.svg)

# docsify <small>3.5</small>

> A magical documentation site generator.

- Simple and lightweight
- No statically built html files
- Multiple themes

[GitHub](https://github.com/docsifyjs/docsify/)
[Get Started](#docsify)
```
