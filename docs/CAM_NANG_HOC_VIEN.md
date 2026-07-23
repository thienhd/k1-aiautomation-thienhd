# CẨM NANG HỌC VIÊN — HOW TO LEARN & SUBMIT

> **Khóa K1 AI Automation — Cách học, thực hành, lưu bài và nộp bài**
>
> Nguồn: [Google Doc gốc của giảng viên](https://docs.google.com/document/d/1H5EUbfmNuRa9K_4K5_GdDlAQ3zVpvQ5GmD9_AOZbQlE/edit)
> Tải về & chuyển sang Markdown ngày 2026-07-23.

> **Mục tiêu của tài liệu:** giúp bạn tự chuẩn bị công cụ, sử dụng đúng repo học chung, lưu toàn bộ sản phẩm trong repo cá nhân và gửi link bài làm để giảng viên chấm.

## Cách sử dụng cẩm nang

- Đọc lần lượt từ đầu đến cuối trước buổi thực hành đầu tiên.
- Thực hiện ngay những mục có nhãn "Bạn cần làm" và tự kiểm tra "Kết quả cần đạt".
- Giữ tài liệu này làm checklist cho mỗi buổi học.
- Nếu giá dịch vụ, tên model hoặc giao diện khác hình minh họa, hỏi giảng viên trước khi thanh toán hoặc cấu hình.

---

## 1. Cách học và cách nộp bài

**Bạn cần hiểu:** Khóa học không dừng ở việc xem demo. Mỗi buổi, bạn lấy tài liệu chuẩn, làm lab, tùy biến thành bài toán của mình, lưu sản phẩm và gửi link để nhận phản hồi.

**Bạn cần làm:**
- Chuẩn bị một tài khoản GitHub cá nhân.
- Xác định rõ repo học chung chỉ là nguồn tài liệu.
- Dành một repo riêng để lưu bài của toàn khóa.

**Kết quả cần đạt:** Bạn phân biệt được nơi lấy bài và nơi lưu/nộp bài.

## 2. Mỗi bài học có ba lớp

**Bạn cần hiểu:** Ba lớp là **Learn → Customize → Submit**. Làm đúng mẫu giúp hiểu quy trình; tùy biến chứng minh năng lực; gửi bài giúp nhận phản hồi.

**Bạn cần làm:**
- Lớp 1: chạy đúng lab mẫu.
- Lớp 2: thay dữ liệu, bối cảnh hoặc yêu cầu bằng bài toán của bạn.
- Lớp 3: publish kết quả và gửi link qua form.

**Kết quả cần đạt:** Bài nộp có cả kết quả lab mẫu và phiên bản tùy biến, không chỉ đổi tên file.

## 3. Workflow Mindset

**Bạn cần hiểu:** Một workflow tốt có chuỗi đầu vào–đầu ra rõ ràng: output của bước trước trở thành input của bước sau. Hãy hiểu quy trình trước khi chọn công cụ.

**Bạn cần làm:**
- Chọn use case cụ thể.
- Mô tả quy trình hiện tại (As-is).
- Thiết kế quy trình mong muốn (To-be), bổ sung fallback, log, edge case và bước con người duyệt.
- Sau khi logic ổn định mới triển khai bằng n8n, AI Agent hoặc ứng dụng.

**Kết quả cần đạt:** Bạn mô tả được workflow bằng các bước, input, output và điều kiện kiểm soát.

**Lưu ý:** Không tự động hóa một quy trình chưa được hiểu và kiểm chứng.

## 4. Lớp 1: Làm theo lab mẫu

**Bạn cần hiểu:** Repo học chung cung cấp Student Kit gồm lab, prompt, template và schema. Bạn chỉ lấy phần cần thiết sang repo cá nhân để thực hành.

**Bạn cần làm:**
- Mở `lab.md` và đọc mục tiêu.
- Lấy input từ `templates` và prompt từ `prompts`.
- Chạy bài trong thư mục buổi học thuộc repo cá nhân.
- Đối chiếu output với schema hoặc tiêu chí PASS.

**Kết quả cần đạt:** Output tồn tại, mở được và đúng cấu trúc yêu cầu.

**Lưu ý:** Không thực hành trực tiếp trong repo học chung.

## 5. Lớp 2: Tùy biến bài toán

**Bạn cần hiểu:** Tùy biến nghĩa là đổi dữ liệu, bối cảnh hoặc yêu cầu thực tế nhưng vẫn giữ data contract và bước kiểm chứng.

**Bạn cần làm:**
- Giữ nguyên thư mục kết quả lab mẫu để đối chiếu.
- Tạo thư mục `lop-2-custom`.
- Ghi rõ dữ liệu đã thay, prompt đã chỉnh và output mới.
- Kiểm tra lại output theo cùng chuẩn chất lượng.

**Kết quả cần đạt:** Người khác đọc repo có thể nhận ra phần nào là mẫu và phần nào là sản phẩm của bạn.

**Lưu ý:** Không ghi đè kết quả Lớp 1.

## 6. Lớp 3: Chuẩn bị bài để được chấm

**Bạn cần hiểu:** Mỗi học viên tạo một repo GitHub public riêng cho toàn khóa. Mỗi buổi có một thư mục `buoi-NN`. Link bài được gửi qua form khảo sát/nộp bài.

**Bạn cần làm:**
- Tạo repo theo gợi ý `k1-aiautomation-<username>`.
- Tạo thư mục riêng cho từng buổi.
- Push bài lên GitHub.
- Điền GitHub username và link repo hoặc link trực tiếp đến thư mục buổi học vào form.

**Kết quả cần đạt:** Giảng viên mở được bài mà không cần quyền truy cập đặc biệt.

**Lưu ý:**
- Không nộp bài vào repo học chung.
- Không đưa API key, `.env`, credential hoặc dữ liệu nhạy cảm lên GitHub.
- Form chính thức sẽ được giảng viên cung cấp.

## 7. Clone repo học chung lần đầu

**Bạn cần hiểu:** Clone chỉ cần thực hiện một lần trên mỗi máy. Những lần sau dùng `pull` để cập nhật Student Kit.

**Bạn cần làm:**
- Mở Terminal tại thư mục bạn dùng để học.
- Chạy lần lượt các lệnh bên dưới.
- Kiểm tra remote trỏ đúng `alobase-org/hocvien_k1_aiautomation`.

```bash
git clone https://github.com/alobase-org/hocvien_k1_aiautomation.git
cd hocvien_k1_aiautomation
git switch main
git remote -v
```

**Kết quả cần đạt:** Bạn có thư mục `hocvien_k1_aiautomation` trên máy và đang ở branch `main`.

## 8. Cấu trúc Student Kit

**Bạn cần hiểu:** Mỗi thư mục tương ứng một buổi học; bên trong có slide, README, lab, prompt, template và schema.

**Bạn cần làm:**
- Đọc README trước.
- Thực hiện theo `lab.md`.
- Chỉ dùng checkpoint/solution khi giảng viên cho phép.

**Kết quả cần đạt:** Bạn biết chính xác file nào là hướng dẫn, input, prompt và chuẩn đầu ra.

**Lưu ý:** Repo này ở trạng thái chỉ đọc đối với bài cá nhân.

## 9. Cập nhật bài mới an toàn

**Bạn cần hiểu:** Repo học chung nên luôn sạch để có thể cập nhật bằng fast-forward mà không xung đột với bài cá nhân.

**Bạn cần làm:**
- Chạy `git status` trước.
- Chuyển mọi file bài cá nhân sang repo riêng nếu lỡ tạo nhầm.
- Chạy `git pull --ff-only origin main`.

```bash
git status
git switch main
git pull --ff-only origin main
```

**Kết quả cần đạt:** Terminal báo cập nhật thành công và repo không có thay đổi cá nhân.

## 10. Tách hai repo trên máy

**Bạn cần hiểu:** Bạn cần hai thư mục nằm cạnh nhau: repo học chung để đọc và repo cá nhân để viết, commit, push.

**Bạn cần làm:**
- Giữ `hocvien_k1_aiautomation` làm nguồn tham khảo.
- Mở `k1-aiautomation-<username>` làm workspace thực hành.
- Copy đúng tài liệu cần dùng, không copy toàn bộ solution.

**Kết quả cần đạt:** Mọi file do bạn tạo hoặc chỉnh sửa đều nằm trong repo cá nhân.

## 11. Publish bài và gửi form

**Bạn cần hiểu:** Sau khi hoàn thành, chỉ commit đúng thư mục của buổi, push lên GitHub rồi kiểm tra link trước khi gửi form.

**Bạn cần làm:**
- Kiểm tra `git status`.
- Add đúng thư mục buổi học.
- Commit bằng thông điệp dễ hiểu.
- Push lên `main`.
- Mở link trong cửa sổ ẩn danh để xác nhận repo public.
- Điền form khảo sát/nộp bài.

```bash
cd k1-aiautomation-<username>
git status
git add buoi-03
git commit -m "feat(buoi-03): nop bai"
git push origin main
```

**Kết quả cần đạt:** Link gửi cho giảng viên mở trực tiếp đúng bài của buổi học.

## 12. Lộ trình bài tập và chứng nhận

**Bạn cần hiểu:** Hoàn thành tối thiểu **50% bài tập** là điều kiện bước vào chương trình **Mentor**. Trong giai đoạn Mentor, bạn hoàn thiện dự án thành **Capstone**; hoàn thành Capstone mới đủ điều kiện nhận chứng nhận.

**Bạn cần làm:**
- Theo dõi số bài đã nộp.
- Cập nhật bài theo feedback.
- Lưu các phiên bản quan trọng trong Git để thấy tiến bộ.

**Kết quả cần đạt:** Bạn hiểu 50% bài tập mở quyền tham gia Mentor, không thay thế Capstone.

## 13. Bộ công cụ học tập

**Bạn cần hiểu:** Git/GitHub lưu lịch sử sản phẩm; **Antigravity** mở workspace; **Cline** là Coding Agent; **GLM** là model hỗ trợ Cline.

**Bạn cần làm:**
- Cài Git và đăng nhập GitHub.
- Cài Antigravity.
- Cài extension Cline.
- Chuẩn bị API key theo hướng dẫn của giảng viên.

**Kết quả cần đạt:** Bạn hiểu vai trò của từng công cụ và không nhầm Coding Agent với nơi lưu bài.

**Lưu ý:** Luôn xem diff và phạm vi file trước khi chấp nhận thay đổi do agent tạo.

## 14. Checklist chuẩn bị công cụ

**Bạn cần hiểu:** Chỉ đánh dấu PASS khi đã kiểm tra thật, không chỉ vì đã cài đặt hoặc đăng ký.

**Bạn cần làm:**
- Mở được repo trên máy.
- Chạy thử một prompt.
- Chạy thử một workflow n8n.
- Kiểm tra kết nối dịch vụ cần dùng.
- Chuẩn bị Google Account, GitHub và trình duyệt Chrome.

**Kết quả cần đạt:** Bạn sẵn sàng bước vào lab mà không mất thời gian cài đặt cơ bản.

**Lưu ý:** Không chiếu, gửi hoặc commit API key/token.

## 15. Thiết lập Antigravity, Cline và GLM

**Bạn cần hiểu:** Cline cần được mở trong đúng repo cá nhân và cấu hình provider/model theo thông tin giảng viên cung cấp tại thời điểm học.

**Bạn cần làm:**
- Mở Antigravity → Open Folder → chọn repo cá nhân.
- Nhấn `Ctrl+Shift+X`, tìm **Cline** và cài đặt.
- Mở Cline Settings, chọn **OpenAI Compatible**.
- Nhập Base URL, Z.AI API Key và model GLM được giảng viên chốt.
- Gửi prompt kiểm tra: *"Đọc README của workspace và tóm tắt 3 việc cần làm. Chưa sửa file."*

**Kết quả cần đạt:** Cline đọc đúng workspace, trả lời đúng yêu cầu và chưa sửa file.

**Lưu ý:**
- Lưu key trong Secret hoặc `.env`; không dán key vào chat hay commit lên GitHub.
- Không tự đoán model ID nếu gặp lỗi Model not found.

## 16. Chọn cách sử dụng n8n

**Bạn cần hiểu:** Có ba phương án: **n8n Cloud** để bắt đầu nhanh; **VPS** để chạy 24/7; **Docker local** để học và kiểm soát dữ liệu trên máy.

**Bạn cần làm:**
- [Cloud](https://n8n.partnerlinks.io/giangxai): kiểm tra trial và giá hiện hành trước khi đăng ký.
- [Hostinger VPS](https://hostinger.com/GIANGXAI10): kiểm tra giá khuyến mãi, chu kỳ trả trước và giá gia hạn. Nhập mã giảm giá "Giangxai" để được giảm 10%.
- Docker local: cài Docker, chạy n8n trên máy và chuẩn bị tunnel/domain nếu cần webhook Internet.
- Chọn phương án phù hợp mục tiêu và ngân sách.

**Kết quả cần đạt:** Bạn mở được giao diện n8n và chạy thử một workflow.

**Lưu ý:**
- Máy tắt thì n8n local dừng.
- Giá và chính sách trial có thể thay đổi; xem trang chính thức trước khi thanh toán.

## 17. Kích hoạt Gemini API

**Bạn cần hiểu:** Đối với luồng học của khóa, hãy chuẩn bị khả năng kích hoạt **Paid Tier** và nạp trước khoảng **10 USD** (giao diện/tỷ giá Việt Nam có thể xấp xỉ 300.000đ).

**Bạn cần làm:**
- Mở [aistudio.google.com/api-keys](https://aistudio.google.com/api-keys).
- Tạo hoặc chọn Google Cloud project.
- Chọn Set up billing và thêm phương thức thanh toán.
- Nếu hệ thống yêu cầu Prepay, nạp số dư tối thiểu hiển thị trên giao diện.
- Tạo API key, lưu trong Secret hoặc `.env` và test request.

**Kết quả cần đạt:** Gemini API key hoạt động và không xuất hiện trong GitHub.

**Lưu ý:**
- Google AI Pro/Google One không đồng nghĩa Gemini API được miễn phí hoặc tự động dùng Postpay.
- Billing phụ thuộc tài khoản và có thể thay đổi; đọc thông tin hiển thị trước khi xác nhận thanh toán.

## 18. Checklist trước khi gửi bài

**Bạn cần hiểu:** Một bài nộp tốt phải mở được, dễ hiểu, đúng vị trí và không làm lộ bí mật.

**Bạn cần làm:**
- Output mở được.
- README mô tả ngắn gọn mục tiêu, cách chạy và kết quả.
- Bài nằm đúng repo cá nhân và đúng thư mục buổi.
- Không có API key, token, `.env` hoặc dữ liệu nhạy cảm.
- Repo public và mở được trong cửa sổ ẩn danh.
- Form chứa đúng GitHub username và link bài.

**Kết quả cần đạt:** Giảng viên có thể truy cập, chạy/đọc và phản hồi bài mà không phải hỏi lại link hoặc quyền truy cập.

---

## Mẫu cấu trúc repo cá nhân

```
k1-aiautomation-<username>/
├── README.md
├── buoi-01/
│   ├── lop-1-lab-mau/
│   ├── lop-2-custom/
│   └── README.md
├── buoi-02/
└── buoi-03/
```

## Tự xử lý một số lỗi thường gặp

| Tình huống | Cách xử lý |
| --- | --- |
| Không thấy bài mới | Kiểm tra đúng repo/branch `main` rồi chạy `git pull --ff-only origin main`. |
| Sửa nhầm repo học chung | Copy file sang repo cá nhân trước; chỉ hoàn nguyên khi đã chắc chắn bài được lưu. |
| Cline không xuất hiện | Reload Antigravity/IDE và kiểm tra extension đã Enable. |
| Invalid API Key | Kiểm tra key, Base URL, provider OpenAI Compatible và model ID. |
| n8n local không nhận webhook | Kiểm tra container, port `5678` và dùng tunnel/domain nếu dịch vụ ngoài gọi vào máy. |
| Repo không mở được | Chuyển repo sang Public và kiểm tra lại bằng cửa sổ ẩn danh. |
| Lỡ commit API key | Thu hồi key ngay, tạo key mới và nhờ giảng viên/TA hỗ trợ làm sạch lịch sử Git. |

## Nguồn chính thức để kiểm tra

- n8n Cloud — Trial và pricing: <https://n8n.io/pricing/>
- Hostinger — n8n VPS và giá Việt Nam: <https://www.hostinger.com/vn/n8n-hosting>
- Google — Gemini API billing: <https://ai.google.dev/gemini-api/docs/billing>

> Giá, trial, model ID, hạn mức và chính sách billing có thể thay đổi. Hãy kiểm tra nguồn chính thức và hướng dẫn cập nhật của giảng viên trước khi thanh toán.
