# Checklist chuẩn bị công cụ — trước Buổi 01 (23/07/2026)

Chỉ đánh dấu PASS khi đã **kiểm tra thật**, không chỉ vì đã cài đặt hoặc đăng ký (theo mục 14 cẩm nang).

## 1. Nền tảng đã có sẵn trên máy (đã kiểm tra 23/07/2026)

- [x] Git 2.45.2 — identity: `Thien Ha Duy <thienhd@gmail.com>`
- [x] Node.js v24.13.0 + npm 11.6.2
- [x] Python 3.14.3
- [x] VS Code 1.95 (dự phòng, khóa học dùng Antigravity là chính)
- [x] Antigravity IDE đã cài (`%LOCALAPPDATA%\Programs\Antigravity`)

## 2. Tài khoản

- [ ] Tài khoản GitHub cá nhân (dùng để tạo repo public `k1-aiautomation-thienhd`)
- [ ] Google Account (cho Gemini API, Google AI Studio)
- [ ] Trình duyệt Chrome cài sẵn

## 3. GitHub CLI (khuyến nghị, giúp push/tạo repo nhanh hơn)

```bash
winget install --id GitHub.cli
gh auth login
```

- [ ] `gh` cài đặt thành công
- [ ] `gh auth login` đăng nhập thành công

## 4. Tạo repo cá nhân trên GitHub

- [ ] Tạo repo **public** tên `k1-aiautomation-thienhd`
- [ ] Push nội dung workspace này lên (xem hướng dẫn cuối file [README.md](README.md))
- [ ] Mở link repo bằng cửa sổ ẩn danh để xác nhận public, không cần đăng nhập

## 5. Clone repo học chung (khi giảng viên cung cấp link/quyền truy cập)

```bash
cd "C:\Users\thienhd\source\K1-AI-Automation"
git clone https://github.com/alobase-org/hocvien_k1_aiautomation.git
cd hocvien_k1_aiautomation
git switch main
git remote -v
```

- [ ] Đã clone thành công `hocvien_k1_aiautomation`
- [ ] `git remote -v` trỏ đúng `alobase-org/hocvien_k1_aiautomation`

## 6. Cline extension trong Antigravity

- [ ] Mở Antigravity → **Open Folder** → chọn `k1-aiautomation-thienhd`
- [ ] `Ctrl+Shift+X` → tìm **Cline** → Install
- [ ] Mở Cline Settings → chọn provider **OpenAI Compatible**
- [ ] Nhập Base URL + Z.AI API Key + model GLM (giảng viên chốt tại buổi học — điền vào [.env](.env) local, không hard-code)
- [ ] Test prompt: *"Đọc README của workspace và tóm tắt 3 việc cần làm. Chưa sửa file."* → Cline trả lời đúng và **chưa sửa file nào**

## 7. n8n — chọn 1 trong 3 phương án

- [ ] Đã chọn phương án: ☐ Cloud ☐ Hostinger VPS ☐ Docker local
- [ ] Mở được giao diện n8n
- [ ] Chạy thử được một workflow đơn giản

Ghi chú giá/khuyến mãi (kiểm tra lại trước khi thanh toán, giá có thể đổi):
- n8n Cloud: <https://n8n.partnerlinks.io/giangxai> — xem trial & giá tại <https://n8n.io/pricing/>
- Hostinger VPS: <https://hostinger.com/GIANGXAI10> — mã giảm giá `Giangxai` (-10%), xem giá VN tại <https://www.hostinger.com/vn/n8n-hosting>
- Docker local: cần cài Docker Desktop trước (`winget install Docker.DockerDesktop`), lưu ý máy tắt thì n8n dừng.

## 8. Gemini API (Google AI Studio)

- [ ] Mở <https://aistudio.google.com/api-keys>
- [ ] Tạo/chọn Google Cloud project
- [ ] Set up billing, nạp trước ~10 USD (~300.000đ, tỷ giá có thể đổi)
- [ ] Tạo API key, lưu vào `.env` local
- [ ] Test request thành công
- [ ] Xác nhận key **không** xuất hiện trong bất kỳ commit nào trên GitHub

Tham khảo chính thức: <https://ai.google.dev/gemini-api/docs/billing>

## 9. Kiểm tra bảo mật cuối cùng trước buổi học

- [ ] File `.env` đã nằm trong `.gitignore`
- [ ] Chưa từng `git add .env` hoặc bất kỳ file chứa key nào
- [ ] Đã hiểu quy trình xử lý nếu lỡ commit key (mục "Tự xử lý lỗi thường gặp" trong cẩm nang)
