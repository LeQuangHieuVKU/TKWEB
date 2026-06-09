## TVFlix - Movie Web App (Netflix-style UI)

TVFlix là một dự án web front-end thuần **HTML/CSS/JavaScript** mô phỏng giao diện xem phim kiểu Netflix.  
Ứng dụng lấy dữ liệu phim theo thời gian thực từ **TMDB API** và hiển thị theo nhiều màn hình khác nhau.

## Mục tiêu dự án

- Xây dựng giao diện xem phim hiện đại, responsive.
- Thực hành thao tác với API ngoài (TMDB).
- Rèn luyện tổ chức mã JavaScript theo module.

## Tính năng chính

- Trang chủ hiển thị:
  - Banner phim nổi bật (slider tự động/chuyển tay).
  - Danh sách phim: Upcoming, Trending tuần, Top Rated.
- Sidebar lọc phim:
  - Theo **thể loại** (genre).
  - Theo **ngôn ngữ** (English, Hindi, Bengali, Vietnamese).
- Trang danh sách phim (`movie-list.html`):
  - Hiển thị toàn bộ phim theo bộ lọc đã chọn.
  - Nút **Load More** để tải thêm dữ liệu.
- Trang chi tiết phim (`detail.html`):
  - Thông tin phim: poster, điểm đánh giá, thời lượng, năm phát hành, phân loại tuổi.
  - Diễn viên, đạo diễn.
  - Trailer/teaser YouTube.
  - Gợi ý phim tương tự.
- Tìm kiếm phim realtime bằng ô search ở header.

## Cấu trúc dự án

```text
TKWEB/
├── index.html                # Trang chủ
├── movie-list.html           # Trang danh sách phim theo bộ lọc
├── detail.html               # Trang chi tiết phim
├── assets/
│   ├── css/style.css         # Toàn bộ style giao diện
│   ├── js/
│   │   ├── api.js            # Cấu hình API key, helper fetch
│   │   ├── index.js          # Logic trang chủ
│   │   ├── movie-list.js     # Logic trang danh sách + load more
│   │   ├── detail.js         # Logic trang chi tiết
│   │   ├── search.js         # Logic tìm kiếm
│   │   ├── sidebar.js        # Logic sidebar và bộ lọc
│   │   ├── movie-card.js     # Component thẻ phim
│   │   └── global.js         # Hàm dùng chung + toggle UI
│   └── images/               # Hình ảnh icon/logo
└── README.md
```

## Công nghệ sử dụng

- HTML5
- CSS3
- JavaScript (ES Modules)
- TMDB API

## Cách chạy dự án

Vì là dự án front-end tĩnh, bạn có thể chạy nhanh bằng 1 trong 2 cách:

1. Mở trực tiếp file `index.html` bằng trình duyệt.
2. Hoặc dùng local server (khuyến nghị), ví dụ với VS Code + Live Server.
