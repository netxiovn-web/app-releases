# 📦 Netxio App Releases Hub

Kho lưu trữ phân phối và cập nhật tự động (Auto-Updater Distribution Hub) cho các phần mềm phát triển bởi **Netxio Web**.

---

## 🎯 Danh sách ứng dụng hỗ trợ cập nhật

| Tên Ứng Dụng | File Cấu Hình Version | Tag Release |
| :--- | :--- | :--- |
| **Facebook Fanpage BM Manager** | [`fb_version.json`](./fb_version.json) | `fb-v*` |

---

## ⚙️ Cơ chế hoạt động

1. Khi mở ứng dụng trên máy khách, app sẽ tự động gửi yêu cầu đọc file cấu hình tương ứng (ví dụ `fb_version.json`) từ nhánh `main`.
2. Nếu phát hiện số phiên bản mới hơn phiên bản hiện tại, app sẽ hiển thị hộp thoại thông báo cập nhật kèm danh sách các tính năng mới (`changelog`).
3. Khi người dùng bấm "Cập nhật ngay", app sẽ tự động tải file `update.zip` từ mục **Releases** của repo này, sao lưu an toàn `config.json` và giải nén cài đặt bản mới nhất.
