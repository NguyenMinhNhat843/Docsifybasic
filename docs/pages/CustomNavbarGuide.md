# Custom Navbar

## Cách dùng

> Thay vì bật sideBar thì cũng có thể tự code 1 navBar trên đầu

```html
<!-- index.html -->

<body>
  <nav>
    <a href="#/">EN</a>
    <a href="#/zh-cn/">简体中文</a>
  </nav>
  <div id="app"></div>
</body>
```

> Thẻ nav phải nằm trên thẻ div.app - đây là nơi render html chính

Hoặc cũng có thể tách 1 file \_navbar.md ra riêng

```bash
# Bật loadNavbar: true trong config index.html
<script>
  window.$docsify = {
    loadNavbar: true
  }
</script>

# Tạo file _navbar.md cùng cấp với README.md
# Code file _navbar.md giống với khi code _sidebar.md

```

> Nếu vừa code cả thẻ nav trong file index.html, vừa bật loadNavbar và code navBar riêng thì \_navbar.md sẽ ghi đè thẻ nav
> loadNavbar và loadsSidebar không ghi đè lẫn nhau

## Nested Navbar

> Có thể code navbar với submenu như code dưới

```bash
# file _navbar.md

* Nhóm 1
    * [item 1](#)
    * [item2](#)
* Nhóm 2
    * item 1
    * item 2
```
