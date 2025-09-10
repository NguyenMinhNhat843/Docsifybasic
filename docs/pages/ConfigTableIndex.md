# Trong file index.html chứa đoạn code config chung

```bash
 <script>
    window.$docsify = {
        loadSidebar: true,
        subMaxLevel: 3,
    };
</script>
```

#### <span style="color: red;">Danh sách các thuộc tính</span>

```bash
loadSideBar     Boolean         Hiện html tương ứng trong file _navbar.md

subMaxLevel     number          Mỗi thẻ H sẽ tương ứng với 1 đề mục trong sideBar,
                                number là số cấp tối đa được hiển thị

loadNavbar      Boolean         Hiển thị custom navbar

auto2top        Boolean         Scroll tới đầu trang khi chuyển routes

# Title <!-- Docsify-ignore -->:  Viết trong file .md để loại thẻ thẻ H này khỏi sideBar
# Getting Started <!-- {docsify-ignore-all} --> : Đặt ở đầu file .d để loại toàn bộ chỉ mục trong file này ra khỏi sideBar
```
