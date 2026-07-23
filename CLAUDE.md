# CLAUDE.md — k1-aiautomation-thienhd

Đây là **repo cá nhân** của anh Thiện cho khóa **K1 AI Automation & Vibe Coder** (Alobase).
Repo này dùng để lưu bài thực hành, tùy biến và nộp bài — **không** phải nơi chứa tài liệu gốc của khóa học.

## Bối cảnh khóa học

- **Khóa:** AI Automation & Vibe Coder K1 (Alobase)
- **Giảng viên:** Đặng Hải Lộc, Giang Vt, Minh Cường
- **Admin/hỗ trợ:** Zalo 0974 155 356 (Ms. Lê Trang)
- **Lịch học:** bắt đầu Thứ 5, 23/07/2026, đều đặn Thứ 3 & Thứ 5 hàng tuần, tổng **8 buổi**. Xem chi tiết tại [LICH_HOC.md](LICH_HOC.md).
- **Cẩm nang gốc (đã tải về):** [docs/CAM_NANG_HOC_VIEN.md](docs/CAM_NANG_HOC_VIEN.md) — nguồn: [Google Doc](https://docs.google.com/document/d/1H5EUbfmNuRa9K_4K5_GdDlAQ3zVpvQ5GmD9_AOZbQlE/edit)

## Mô hình 2 repo — LUÔN nhớ điều này

| Repo | Vai trò | Vị trí đề xuất |
| --- | --- | --- |
| `hocvien_k1_aiautomation` | Repo học chung của Alobase, **chỉ đọc**. Chứa Student Kit (slide, lab.md, prompts, templates, schema) theo từng buổi. | `C:\Users\thienhd\source\K1-AI-Automation\hocvien_k1_aiautomation` (clone khi có link chính thức) |
| `k1-aiautomation-thienhd` | Repo cá nhân **(chính là repo này)**, nơi duy nhất để ghi, commit, push bài làm. | thư mục hiện tại |

**Quy tắc bất di bất dịch:**
- KHÔNG BAO GIỜ thực hành hoặc commit trực tiếp vào repo học chung.
- Chỉ copy đúng phần cần thiết (lab.md, prompt, template) từ repo học chung sang đúng thư mục `buoi-NN/lop-1-lab-mau/` của repo này.
- Không copy toàn bộ solution/checkpoint trừ khi giảng viên cho phép.

## Cấu trúc mỗi buổi (3 lớp: Learn → Customize → Submit)

```
buoi-NN/
├── README.md            # mục tiêu buổi, cách chạy, kết quả
├── lop-1-lab-mau/        # chạy đúng lab mẫu, đối chiếu schema/PASS
└── lop-2-custom/         # tùy biến bằng bài toán thực tế của anh Thiện
```

- **Lớp 1** — làm đúng theo `lab.md` của Student Kit, không sáng tạo thêm, chỉ để hiểu quy trình.
- **Lớp 2** — giữ nguyên data contract & bước kiểm chứng, nhưng đổi dữ liệu/bối cảnh/yêu cầu thành bài toán thực tế (vd: dữ liệu công việc tại HOYA, nếu không có gì nhạy cảm).
- **Lớp 3** — publish: `git add buoi-NN && git commit -m "feat(buoi-NN): ..." && git push origin main`, sau đó điền link vào form nộp bài của giảng viên.

Dùng [`_template-buoi/`](_template-buoi) làm khung mẫu khi bắt đầu một buổi mới — copy thư mục này thành `buoi-NN` rồi điền nội dung.

## Bộ công cụ đã cài trên máy này

| Công cụ | Vai trò trong khóa | Trạng thái |
| --- | --- | --- |
| Git 2.45 | Lưu lịch sử sản phẩm, push bài | ✅ Đã cài, identity: Thien Ha Duy |
| Antigravity IDE | Workspace chính để code | ✅ Đã cài |
| Cline (extension) | Coding Agent chạy trong Antigravity | ⬜ Cần cài trong Antigravity (`Ctrl+Shift+X` → tìm "Cline") |
| GLM qua Z.AI (OpenAI Compatible) | Model đứng sau Cline | ⬜ Cần API key từ giảng viên |
| n8n | Workflow automation | ⬜ Chưa chọn phương án (Cloud / VPS / Docker local) |
| Gemini API (Google AI Studio) | Model cho các lab AI | ⬜ Cần bật Paid Tier + nạp ~10 USD |
| GitHub CLI (`gh`) | Push/tạo repo nhanh hơn | ❌ Chưa cài — cân nhắc `winget install --id GitHub.cli` |
| Docker | Chạy n8n local | ❌ Chưa cài — chỉ cần nếu chọn phương án Docker local |

Chi tiết setup từng bước: xem [SETUP_CHECKLIST.md](SETUP_CHECKLIST.md).

## Quy tắc bảo mật — TUYỆT ĐỐI không vi phạm

- **Không bao giờ** commit API key, token, `.env`, hoặc credential lên GitHub (repo này sẽ để **public**).
- Lưu mọi key trong file `.env` local (đã có trong `.gitignore`) hoặc Secret Manager của IDE.
- Trước mỗi lần `git add`, luôn chạy `git status` và `git diff --stat` để kiểm tra không dính file nhạy cảm.
- Nếu lỡ commit key: thu hồi (revoke) key ngay lập tức, tạo key mới, báo giảng viên/TA để làm sạch lịch sử Git.
- Khi dùng Cline/Coding Agent: luôn xem diff và phạm vi file trước khi Accept — không tự động approve toàn bộ thay đổi.

## Lộ trình & điều kiện hoàn thành

- Hoàn thành tối thiểu **50% bài tập** → đủ điều kiện vào chương trình **Mentor**.
- Trong giai đoạn Mentor, hoàn thiện dự án thành **Capstone**.
- Hoàn thành Capstone → đủ điều kiện nhận **chứng nhận**.
- Theo dõi tiến độ tại [TIEN_DO.md](TIEN_DO.md).

## Khi Claude Code hỗ trợ trong repo này

- Đây là repo học tập cá nhân, không phải sản phẩm công ty HOYA — nhưng vẫn áp dụng quy tắc chung: viết code/comment tiếng Anh nếu là script thực thi (theo global CLAUDE.md), tài liệu/README có thể tiếng Việt như khóa học yêu cầu.
- Khi tạo bài nộp buổi mới, luôn tạo cả `lop-1-lab-mau/` và `lop-2-custom/`, không ghi đè lẫn nhau.
- Trước khi push, luôn nhắc kiểm tra checklist ở mục 18 của [docs/CAM_NANG_HOC_VIEN.md](docs/CAM_NANG_HOC_VIEN.md#18-checklist-trước-khi-gửi-bài).
- Không tự ý `git push` khi chưa được anh Thiện xác nhận nội dung buổi học đã hoàn chỉnh.
