# Bắt đầu nhanh

#### Lệnh cài đặt global

npm i docsify-cli -g

#### Lệnh khởi tạo

docsify init ./docs

> Trong đó "./docs" là tên folder muốn khỏi tạo

#### Các File chính

- index.html: Là file đầu tiên web đọc khi chạy

[Xem các config cho file html ở đây](#)

```bash
#!/bin/bash
<body>
    <div id="app"></div>
    <script>
        window.$docsify = {
        // Config ở đây
        };
    </script>
    <!-- Docsify v4 -->
    <script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
    <script src="//cdn.jsdelivr.net/npm/docsify-emoji"></script>
</body>
```

- README.md: Trang home, route là "localhost:3000/#"

> Là nơi load UI đầu tiên, khi chạy web sẽ chuyển markdown ở file này trước thành html và bỏ vào index.html

# Setup nhiều route

#### Cấu trúc

```bash
docs
    routes
        route1.md
        route2.md
        ...
    index.html
    README.md # đây là trang chủ
```

#### Các route trên sẽ tương ứng với path:

```bash
- README.md:   localhost:300/#/
- route1.md:   localhost:3000/#/routes/route1
- route2.md:   localhost:3000/#/routes/route2
```
