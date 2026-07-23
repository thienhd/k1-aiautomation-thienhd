# k1-aiautomation-thienhd

Repo cá nhân của **Thiện Hà Duy** cho khóa **K1 AI Automation & Vibe Coder** (Alobase).
Dùng để lưu bài thực hành, tùy biến (Learn → Customize → Submit) và nộp bài cho giảng viên chấm.

- Hướng dẫn học/setup đầy đủ: [CLAUDE.md](CLAUDE.md)
- Cẩm nang gốc từ giảng viên (Markdown): [docs/CAM_NANG_HOC_VIEN.md](docs/CAM_NANG_HOC_VIEN.md)
- Lịch học: [LICH_HOC.md](LICH_HOC.md)
- Checklist chuẩn bị công cụ: [SETUP_CHECKLIST.md](SETUP_CHECKLIST.md)
- Theo dõi tiến độ nộp bài: [TIEN_DO.md](TIEN_DO.md)

## Cấu trúc

```
k1-aiautomation-thienhd/
├── CLAUDE.md                  # hướng dẫn ngữ cảnh khóa học cho Claude Code
├── README.md                  # file này
├── LICH_HOC.md                 # lịch 8 buổi
├── SETUP_CHECKLIST.md          # checklist cài đặt công cụ
├── TIEN_DO.md                  # theo dõi tiến độ nộp bài / điều kiện Mentor & Capstone
├── docs/
│   └── CAM_NANG_HOC_VIEN.md    # cẩm nang gốc tải về từ Google Doc
├── _template-buoi/             # khung mẫu, copy thành buoi-NN khi bắt đầu buổi mới
│   ├── lop-1-lab-mau/
│   └── lop-2-custom/
├── buoi-01/
│   ├── lop-1-lab-mau/
│   ├── lop-2-custom/
│   └── README.md
├── buoi-02/ ... buoi-08/
```

## Đưa repo này lên GitHub (làm 1 lần)

```bash
cd "C:\Users\thienhd\source\K1-AI-Automation\k1-aiautomation-thienhd"
git init
git add .
git commit -m "chore: khoi tao workspace khoa K1 AI Automation"
gh repo create k1-aiautomation-thienhd --public --source=. --remote=origin --push
```

Nếu chưa cài `gh`, tạo repo public thủ công trên github.com rồi:

```bash
git remote add origin https://github.com/<username>/k1-aiautomation-thienhd.git
git branch -M main
git push -u origin main
```

## Nộp bài mỗi buổi

```bash
git add buoi-03
git commit -m "feat(buoi-03): nop bai"
git push origin main
```

Sau đó mở link repo/thư mục bằng cửa sổ ẩn danh để xác nhận public, rồi điền vào form nộp bài của giảng viên.
