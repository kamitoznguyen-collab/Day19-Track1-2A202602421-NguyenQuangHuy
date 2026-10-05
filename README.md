# Track 1 · Day 18 — Four Human–AI Micro-prototypes (A/B/C/D)

> Case A: **AI Tutor – Diagnostic Refresher**
>
> Tên repo giữ theo hướng dẫn của BTC.

## 1. Thông tin cá nhân và nhóm

| Mục | Nội dung |
|---|---|
| MHV | 2A202602421 |
| Họ tên | Nguyễn Quang Huy |
| Tên nhóm | Tung Tung Tung Sahur |
| Thành viên & option phụ trách | Lại Bá Quân (2A202602495) · A — [repo](https://github.com/vxtor012/Track1_Day18_02495_LaiBaQuan)<br>Đỗ Lê Việt Anh (2A202602491) · B — [repo](https://github.com/dlvanh/Track1_Day19_2A202602491_DoLeVietAnh)<br>Nguyễn Thị Minh Khánh (2A202602546) · C<br>**Nguyễn Quang Huy (2A202602421) · D** |
| Case | A. AI Tutor – Diagnostic Refresher |
| Tester mình facilitate | Phạm Minh Hiếu (2A202602919) · Tester 4 |

Cấu trúc repo:

```
├── README.md
├── three-option-design-sheet.md     # Chặng 1–5: evidence, A/B/C/D, Human–AI decisions, test plan (giữ tên file theo đề)
├── prototype-link.md                # link A/B/C/D + cách chạy
├── prototype/index.html             # micro-prototype A/B/C/D (một file HTML, canned AI output)
├── prototype-feedback-note.md       # phiên do mình facilitate
├── group-feedback-synthesis.md      # tổng hợp bốn feedback
└── ai-support-log.md
```

## 2. Hypothesis Problem

> **Khi** đang học trên VLearn trong một ngày học dày (đọc lại slide lý thuyết hoặc đang làm Lab) và gặp một khái niệm / bước không hiểu, **người học** gặp khó khăn trong việc **nhận được lời giải thích trúng đúng chỗ mình chưa hiểu**, **vì** họ không xác định được mình đang thiếu gì để hỏi cho rõ (thuật ngữ viết tắt, khái niệm cô đọng, không biết đặt prompt nên ném nguyên slide vào ChatGPT), **dẫn đến** phải rời bài học sang công cụ ngoài, nhận câu trả lời lan man, mất 30–60 phút cho một chỗ bí và có lúc không xong bài Lab trong giờ.

- **Evidence Day 17 (4 Practice Notes của nhóm):** chụp slide / copy text vào ChatGPT, *"nên mình nghĩ là do cả 2"* (Huy); slide viết tắt nên tự ôn không hiểu, mất 30–60 phút (Việt Anh); phát hiện mình bí khi làm sai quiz, tra không được thì hỏi người (Khánh); bí khi làm Lab, hỏi AI ngoài, thường mang bài Lab về nhà (Quân).
- **Chưa chứng minh:** chỗ bí do thiếu kiến thức nền (H1) hay cách trình bày / cách hỏi (H2) (4 note đều nghiêng H2 nhưng là lời tự đánh giá); trợ giúp ngay trong bài có thay được thói quen copy sang ChatGPT không; pattern có đúng ngoài 4 người luyện phỏng vấn không.

Chi tiết: [three-option-design-sheet.md](three-option-design-sheet.md).

## 3. Four Solution Options

Cùng một tình huống: đang ở trình đọc slide của VLearn, đọc một slide 2 lần vẫn không hiểu. Mục tiêu: hiểu đủ để trả lời đúng câu hỏi nhanh dưới slide. Prototype có ba chủ đề (**Context window**, **ReAct agent**, **Gradient Descent**), mỗi chủ đề có **tab Lý thuyết** (slide) và **tab Lab** (bước hướng dẫn) riêng; mỗi phiên test chọn một chủ đề + tab bắt đầu và giữ nguyên cho cả A/B/C/D. Mọi nội dung AI tạo ra đều có **trích dẫn slide** ("Nguồn: Slide 12 · …" / "Xem lại lý thuyết: Slide 12 · …"), bấm vào sẽ mở đúng đoạn trong tab Lý thuyết. Cả bốn option bắt đầu từ cùng nút **"Tôi vẫn chưa hiểu"** (làm nổi bật như nhau); A và C hiện ngay trên nội dung slide, B mở panel chat "Trợ giảng AI", D mở form "Nhờ người hỗ trợ", mô phỏng giao diện VLearn.

| | Cơ chế | Ai xác định chỗ hổng? | AI |
|---|---|---|---|
| **A: Hỏi có hướng dẫn** | User chọn phần chưa hiểu trên slide + kiểu giúp. Hệ thống soạn câu hỏi rõ ràng, user sửa rồi gửi. | User | Don't Act |
| **B: AI hỏi chẩn đoán** | AI hỏi 3 câu ngắn, đưa chẩn đoán kèm bằng chứng và độ chắc chắn. User xác nhận hoặc chọn phần khác. | AI, dựa trên câu trả lời của user | Ask |
| **C: AI chủ động gợi ý** | AI dựa vào tín hiệu hành vi, tự mở sẵn phần ôn. User chấp nhận, đổi, ẩn hoặc tắt. | AI, dựa trên tín hiệu thụ động | Act |
| **D: Nhờ người thật, AI soạn yêu cầu** | AI gom ngữ cảnh thành yêu cầu hỗ trợ; user chọn gửi mentor/TA hoặc nhóm Lab, bỏ bớt dòng không muốn chia sẻ; người thật trả lời. | Người thật (mentor/TA, bạn cùng nhóm) | Act khi soạn, Ask trước khi gửi, Don't Act khi giải thích |

Prototype: [prototype-link.md](prototype-link.md).

## 4. Đóng góp của tôi trong nhóm

> Nháp do AI soạn từ những việc đã làm trong phiên làm việc với AI (xem [ai-support-log.md](ai-support-log.md)). Đã tự đọc lại, sửa cho đúng và bổ sung phần làm cùng nhóm mà AI không biết.

- **Option phụ trách chính: D — Nhờ người thật, AI soạn yêu cầu.** Đề xuất hướng human escalation (đề yêu cầu pool phải có), dựa trên nút "Gửi yêu cầu" sẵn có của VLearn và Practice Note 3 ("tra không được thì hỏi người"). Thiết kế modal gom ngữ cảnh (chọn người nhận, tick / bỏ từng dòng ngữ cảnh), panel theo dõi trạng thái Đã gửi → Đã xem → Đang trả lời → Đã trả lời, và luồng "Vẫn chưa hiểu".
- **Shared context / prototype:** cung cấp bản ghi màn hình và ảnh chụp VLearn (trình đọc slide, chế độ Lab, panel Trợ giảng AI) để prototype giống hệ thống thật; mô tả hiện trạng VLearn (lý thuyết chỉ có slide, Lab theo bước, 70% tech / 30% non-tech). Định hướng các thay đổi lớn của prototype: thêm nội dung dạng khái niệm, tách tab Lý thuyết / Lab, trích dẫn số slide trong mọi câu trả lời của AI, làm nổi bật nút "Tôi vẫn chưa hiểu", bỏ chế độ tối mặc định. Prototype nộp là bản chung của nhóm (giống repo của Quân) để khớp với các phiên test.
- **Human–AI decisions:** mức Act / Ask / Don't Act cho D (Act khi soạn yêu cầu, Ask trước khi gửi, Don't Act ở phần giải thích); data & consent check cho D.
- **Pilot nội bộ:** tự dùng thử Option A và phát hiện người dùng bỏ qua dòng hướng dẫn "chạm vào đoạn" → sửa thành đoạn nháy vàng + nhãn "+ Chạm để chọn". Phát hiện mục bằng chứng ở B trông như chữ thường → thêm chip luôn hiện + nút mở rõ ràng.
- **Facilitate:** Tester 4 · Phạm Minh Hiếu (2A202602919), thứ tự D → A → B → C. Đã hoàn thành test, tổng hợp kết quả chi tiết trong prototype-feedback-note.md. Điểm nhấn: Tester cần gợi ý ở Option A do định bôi đen văn bản, nhưng sau đó hoàn thành tốt bài test.
- **Tổng hợp:** dựng bản group-feedback-synthesis chung, gom 4 Practice Notes Day 17 vào Design Sheet. Thảo luận cùng nhóm để xác định các pattern từ các phiên test đã có (hiện 2/4 phiên có dữ liệu) (đặc biệt là việc user ưu tiên in-context help như Option A và C) và thống nhất hướng Next Change.

## 5. Prototype Feedback

- **Observation từ phiên mình facilitate:** Tester ưu tiên tương tác in-context (Option A) vì giảm thiểu context switch, không bị phân tâm khỏi nội dung slide. Option D (modal gửi trợ giảng) gây rườm rà và tốn thời gian. (chi tiết: [prototype-feedback-note.md](prototype-feedback-note.md))
- **Bốn-feedback synthesis:** 2/4 phiên có dữ liệu: 1 tester thích Option A (bôi khối nội dung để giải thích ngay tại chỗ) và 1 tester thích Option C (AI chủ động gợi ý). Cả hai đều cung cấp tính năng hỗ trợ in-context mạnh mẽ. (chi tiết: [group-feedback-synthesis.md](group-feedback-synthesis.md))
- **Next Change:** Đề xuất cá nhân (chờ nhóm chốt): Chọn hướng phát triển Option A (Hỏi có hướng dẫn bằng cách chọn đoạn văn bản), đồng thời có thể kết hợp nhẹ với gợi ý từ Option C để tăng tính chủ động. Cải thiện visual affordance khi người dùng chọn khối text.
- **Still Unproven:** Chưa rõ nếu bài Lab cực kỳ phức tạp (phải debug cả đoạn code dài) thì tính năng chọn từng block text (Option A) có đủ đáp ứng ngữ cảnh cho AI để đưa ra hướng dẫn chính xác hay không.

## 6. AI Support Log

Xem [ai-support-log.md](ai-support-log.md). Tóm tắt: AI (Claude) hỗ trợ soạn nháp design sheet, build prototype HTML với canned output và tạo template. AI không tạo observation, quote hay feedback nào. Đã tự viết phần phản ánh cá nhân và các chỉnh sửa thủ công.
