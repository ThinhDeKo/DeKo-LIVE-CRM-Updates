# DeKo LIVE CRM — Auto Update

Repository công khai này dùng để phát hành bộ cài Windows qua GitHub Releases, không lưu dữ liệu khách hàng hay mã nguồn riêng.

## Phát hành phiên bản đầu tiên v46.5.2
1. Trên Windows, giải nén source v46.5.2 và chạy `Tao_File_Cai_Dat_1_EXE.bat` (cần Python 3.12 và Inno Setup 6).
2. Vào tab **Releases** → **Draft a new release**.
3. Tạo tag `v46.5.2`, upload `DeKo_LIVE_CRM_Setup_v46_5_2.exe` từ thư mục `installer_output`, ghi chú thay đổi rồi **Publish release**.
4. Phiên bản v46.5.2 tự kiểm tra URL: https://api.github.com/repos/ThinhDeKo/DeKo-LIVE-CRM-Updates/releases/latest
5. Khi có bản mới, tăng phiên bản trong source và phát hành tag mới (ví dụ `v46.5.3`).

**Bảo mật:** Bật GitHub 2FA. Không commit token, mật khẩu, dữ liệu CRM hay mã nguồn không muốn công khai. App kiểm tra HTTPS và SHA256 digest của tài sản GitHub; chữ ký số vẫn được khuyến nghị. Khi chưa có Release, API latest trả 404 — đây là trạng thái bình thường.
