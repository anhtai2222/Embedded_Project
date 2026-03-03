# Dự án Embedded Project

Thư mục `embbededproject` chứa hệ thống giám sát nhúng với giao diện web
Next.js. README này cung cấp tổng quan về cấu trúc và cách khởi chạy ứng dụng.

---

## 🗂 Cấu trúc thư mục chính

```
embbededproject/
├── MonitorSystem_WebApp/   # ứng dụng web front-end (Next.js)
├── release/                # gói phát hành firmware hoặc tài liệu cho các phiên bản
│   ├── v1.0/
│   ├── v1.1/
│   └── v1.2/
├── latest.json             # thông tin phiên bản mới nhất
└── README.md               # tài liệu này
```

### 📌 MonitorSystem_WebApp

Giao diện web được xây dựng bằng Next.js (TypeScript) giúp hiển thị dữ
liệu từ hệ thống nhúng.  Bạn có thể xem README riêng trong thư mục này để
biết cách chạy và phát triển.

````bash
# mở thư mục và khởi chạy
cd MonitorSystem_WebApp
npm install     # hoặc yarn / pnpm
npm run dev     # chạy chế độ phát triển
````

Truy cập `http://localhost:3000` trên trình duyệt để xem.

## 🛠 Hướng dẫn chung

- Các phiên bản firmware và tài liệu liên quan được lưu trong `release/`.
- `latest.json` chứa metadata (số phiên bản, đường dẫn) để hệ thống nhúng
  có thể kiểm tra cập nhật tự động.
- Mã nguồn backend/firmware (nếu có) nằm ngoài workspace này hoặc sẽ
  được thêm vào bởi nhóm phát triển.

## 📄 Ghi chú

- Đây là một template cơ bản; khi triển khai thực tế bạn nên bổ sung
  mô-đun nhúng, API server và hướng dẫn cài đặt.
- Nếu cần cấu hình thêm cho Next.js, chỉnh trong `MonitorSystem_WebApp/`
  (xem `next.config.ts`).

---


