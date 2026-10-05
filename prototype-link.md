# Prototype Link — A/B/C/D

> Prototype trong repo này là **bản chung của nhóm** (giống [repo của Lại Bá Quân](https://github.com/vxtor012/Track1_Day18_02495_LaiBaQuan/tree/main/prototype)), đúng bản đã dùng trong các phiên test.

**Link chạy online:** https://kamitoznguyen-collab.github.io/Day19-Track1-2A202602421-NguyenQuangHuy/prototype/ (GitHub Pages của repo này; bật ở Settings → Pages, branch `main`, thư mục `/ (root)`).

Prototype mô phỏng trình đọc bài của VLearn. Có ba chủ đề, mỗi chủ đề có **tab Lý thuyết** và **tab Lab** riêng (tester tự chuyển được). Mỗi phiên test chọn **một** chủ đề + tab bắt đầu và dùng cho cả A/B/C/D.

Đường dẫn: `https://kamitoznguyen-collab.github.io/Day19-Track1-2A202602421-NguyenQuangHuy/prototype/#/<chủ đề>/<tab bắt đầu>/<phương án>`, với chủ đề = `context` | `react` | `gd`, tab = `theory` | `lab`, phương án = `A` | `B` | `C` | `D`.

| Trang | Ví dụ |
|---|---|
| Màn chọn (chủ đề + tab + phương án) | `https://kamitoznguyen-collab.github.io/Day19-Track1-2A202602421-NguyenQuangHuy/prototype/` |
| Context window, bắt đầu ở Lý thuyết, Option A | `https://kamitoznguyen-collab.github.io/Day19-Track1-2A202602421-NguyenQuangHuy/prototype/#/context/theory/A` |
| ReAct agent, bắt đầu ở Lab, Option C | `https://kamitoznguyen-collab.github.io/Day19-Track1-2A202602421-NguyenQuangHuy/prototype/#/react/lab/C` |
| Gradient Descent, bắt đầu ở Lab, Option D | `https://kamitoznguyen-collab.github.io/Day19-Track1-2A202602421-NguyenQuangHuy/prototype/#/gd/lab/D` |
| Facilitator log (chỉ facilitator xem) | `https://kamitoznguyen-collab.github.io/Day19-Track1-2A202602421-NguyenQuangHuy/prototype/#/log` |

Cơ chế từng option (không đưa cho tester):

- **A:** user tự chỉ chỗ chưa hiểu và chọn kiểu giúp; AI chỉ trả lời câu được hỏi.
- **B:** AI hỏi 3 câu chẩn đoán, đưa chẩn đoán kèm bằng chứng và độ chắc chắn; user xác nhận hoặc đổi.
- **C:** AI tự bật phần ôn sau ~12 giây hoặc khi trả lời sai câu hỏi nhanh; user chấp nhận, đổi, đóng hoặc tắt.
- **D:** AI soạn yêu cầu hỗ trợ từ ngữ cảnh; user chọn mentor/TA hoặc nhóm Lab rồi gửi; người thật trả lời (Wizard-of-Oz: câu trả lời soạn sẵn hiện sau ~15 giây).

## Chạy local

Mở thẳng file `prototype/index.html` bằng trình duyệt, hoặc chạy server tĩnh:

```bash
python -m http.server 8765 --directory prototype
```

Sau đó mở http://localhost:8765.

## Deploy GitHub Pages

1. Push repo lên GitHub.
2. Vào **Settings → Pages → Build and deployment**, chọn **Deploy from a branch**, branch `main`, thư mục `/ (root)`.
3. Link sẽ có dạng `https://<username>.github.io/<repo>/prototype/`.

## Ghi chú

- Toàn bộ output của AI là **canned** (soạn sẵn), không gọi model hay API.
- Reset: nút **↺ Làm lại** trên thanh trên cùng xoá trạng thái của option đó. Đóng panel Trợ giảng AI thì về lại slide.
- Log lưu trong `localStorage` của trình duyệt đang test. Xoá log trước mỗi tester.
- Font tải từ Google Fonts; nếu không có mạng, trình duyệt dùng font hệ thống.
