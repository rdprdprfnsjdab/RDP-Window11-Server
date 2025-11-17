# 🚀 Windows VPS Auto Pro Max

**Windows VPS Auto Pro Max** là một workflow GitHub Actions mạnh mẽ giúp bạn tự động triển khai một VPS Windows với Remote Desktop (RDP) và Tailscale Premium, kèm quản lý phiên, giám sát và dọn dẹp tự động. Workflow cho phép bạn chọn **thời gian sử dụng VPS từ 30 phút đến 6 giờ 10 phút**.

---

## 🛠 Tính năng chính

- **Tùy chọn thời gian sử dụng VPS**:  
  - 30 phút → 6 giờ (tùy chọn khi chạy workflow)
- **Cấu hình RDP Premium tự động**:  
  - Mở cổng 3389, bật dịch vụ TermService  
  - Tạo user `vanmanhgaming` với quyền Administrator & RDP  
  - Mật khẩu an toàn (bao gồm chữ hoa, chữ thường, số) hoặc dùng mật khẩu tùy chỉnh
- **Tailscale Premium**:  
  - Kết nối VPS vào mạng Tailscale riêng với Auth Key
  - Lấy IP Tailscale tự động
- **Giám sát hệ thống**:  
  - Kiểm tra trạng thái RDP và kết nối liên tục  
  - Tự động khởi động lại dịch vụ nếu cần
- **Tự động tắt VPS**:  
  - Theo thời gian đã chọn
- **Dọn dẹp hệ thống tự động**:  
  - Xóa file tạm, vô hiệu hóa user, đóng kết nối mạng, xóa rule firewall, khôi phục cài đặt RDP

---

## ⚡ Hướng dẫn sử dụng

1. Fork repository và bật **GitHub Actions**.
2. Chạy workflow `🚀 SEVER vanmanhgaming` bằng **`workflow_dispatch`**.
3. Chọn thời gian sử dụng VPS:
   - Ví dụ: `1_Giờ_30_Phút_(90m)`
4. Workflow sẽ thực hiện:
   - Cấu hình RDP, tạo user, cài Tailscale Premium
   - Giám sát VPS liên tục
   - Hiển thị thông tin kết nối:
     ```
     Địa chỉ: <TAILSCALE_IP>
     User: vanmanhgaming
     Password: <RDP_PASSWORD>
     Thời lượng: 1 giờ 30 phút
     ```
5. Mở **Remote Desktop Connection** trên máy của bạn và kết nối với VPS:
   - Host/IP: `<TAILSCALE_IP>`
   - User: `vanmanhgaming`
   - Password: `<RDP_PASSWORD>`

---

## 📝 Lưu ý

- Workflow này chỉ dành cho mục đích học tập và trải nghiệm cá nhân.
- Không để lộ Auth Key của Tailscale trên repository công khai.
- Thời gian VPS sẽ tự động tắt sau khi kết thúc phiên.

---

## © Bản quyền & Liên hệ

© 2025 vanmanhgaming. Mọi quyền được bảo lưu.  
Không được phép sao chép, phân phối hoặc sử dụng thương mại mà không có sự cho phép của tác giả.

🔗 Kết nối với tôi trên mạng xã hội:  
- Facebook: [https://www.facebook.com/Bong.Toi.11022010/](https://www.facebook.com/Bong.Toi.11022010/)  
- YouTube: [youtube.com/@vanmanhgaming](https://youtube.com/@vanmanhgaming)  
- Discord: [https://discord.com/users/1118923892732477691](https://discord.com/users/1118923892732477691)

Cảm ơn bạn đã sử dụng **Windows VPS Auto Pro Max**! 🚀
