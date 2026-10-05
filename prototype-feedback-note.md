# Prototype Feedback Note — Tester 4 · facilitator Nguyễn Quang Huy

| | |
|---|---|
| **Facilitator** | Nguyễn Quang Huy (2A202602421) · owner Option D |
| **Tester** | Phạm Minh Hiếu (2A202602919) · học viên ngoài nhóm |
| **Chủ đề / tab** | Context window · tab Lý thuyết (slide 12) · link `#/context/theory/D` |
| **Thứ tự** | D → A → B → C (theo phân công nhóm) |
| **Ngày / thời lượng** | 05/10/2026 · phiên chính D → A → B khoảng 20 phút (23:01–23:20), bổ sung C khoảng 1 phút (23:58) |
| **Relevant context** (câu trả lời của Hiếu cho câu hỏi mở đầu) | Khi không hiểu slide, mình thường đọc đi đọc lại, tra Google hoặc nhắn tin lên nhóm lớp hỏi các bạn. |
| **Có chuyển tab / bấm trích dẫn không** | Log không ghi lần chuyển tab (`switch-tab`) hay bấm trích dẫn (`cite-open`) nào. |


---

## 1. Kịch bản phiên (~15 phút)

1. **0–2'** — *"Chúng mình đang thử bốn cách thiết kế, không kiểm tra bạn. Bạn cứ tự thao tác và nói to điều mình đang nghĩ."* Hỏi: *"Gần đây bạn có từng đọc lại slide trên VLearn mà vẫn không hiểu không? Lần đó bạn đã làm gì?"*
2. **2–14'** — Mở `#/` → xoá log → chọn **Context window · Lý thuyết** → lần lượt **D, A, B, C** (~3 phút mỗi option, bấm "↺ Làm lại" / "Danh sách" giữa các option). Task đọc giống nhau mỗi lần: *"Hãy dùng phương án này để hiểu slide này đủ để trả lời đúng câu hỏi nhanh bên dưới."*
3. **14–18'** — *"Trong tình huống này bạn chọn A, B, C hay D? Vì sao?"* · *"Bạn muốn tự làm phần nào, giao AI phần nào?"* · *"Điều gì ở phương án đã chọn khiến bạn chưa thoải mái?"*
4. **18–20'** — Copy CSV log, ghi nhanh các ô dưới đây.

Không giải thích nút, không lấp im lặng, không hỏi "Bạn có thích không?". Khi Hiếu hỏi cách dùng: *"Theo bạn, nó nên hoạt động như thế nào?"*

---

## 2. Kỳ vọng của nhóm TRƯỚC phiên test (giả thuyết, không phải quan sát)

Ghi trước để sau phiên so sánh, điền vào dòng "Evidence chống lại kỳ vọng".

| | Kỳ vọng tester sẽ… | Rủi ro nhóm lo |
|---|---|---|
| **D** | Đọc dòng ngữ cảnh AI điền sẵn, chọn TA vì muốn câu trả lời chắc | Chờ ~10 phút thì bỏ sang ChatGPT; ngại hỏi người |
| **A** | Chạm vào công thức `context window ≥ input + output` | Không biết phải chạm vào đoạn (pilot nội bộ: chính facilitator bỏ qua dòng hướng dẫn) |
| **B** | Trả lời 3 câu nhanh, đọc hàng chip ✓ / ? / ✗ | Thấy giống "bị kiểm tra", bấm Bỏ qua |
| **C** | Thấy AI khoanh đoạn sau ~12 giây hoặc sau khi sai câu hỏi nhanh | Bấm nút đỏ trước khi C kịp tự bật; thấy phiền |

---

## 3. Quan sát theo từng option

| Observation | D | A | B | C |
|---|---|---|---|---|
| First action | Bấm "Tôi vẫn chưa hiểu" ở giây 35 (`open-help`), khựng lại nhìn form, click thử vào phần ngữ cảnh AI. | Đưa chuột lướt các dòng, click chọn 2 đoạn (token + budget). | Đọc lướt slide bên trái, sau đó mới nhìn sang panel bên phải. | Chờ 12s, AI tự động gợi ý (`c-nudge`), bấm chọn "Đúng chỗ, đã rõ hơn" (`c-accept`). |
| Chỗ dừng, do dự hoặc hiểu sai | Phân vân việc chọn hỏi TA hay hỏi bạn bè. Cảm thấy popup hơi che mất nội dung học. | Ban đầu định bôi đen (highlight) như dùng Word thay vì click vào nguyên khối (block). | Bị ngợp bởi nhiều text trên side panel. Không rõ nên đọc slide hay đọc chat. | Tốn vài giây đọc Nudge trước khi bấm Accept. |
| Evidence được đọc hay bỏ qua *(log: `open-why`, `cite-open`, `d-toggle-context`)* | Không bỏ dòng ngữ cảnh nào (log không có `d-toggle-context`; gửi đủ slide / thời gian / câu hỏi nhanh, có ghi chú). Sau câu trả lời đầu của TA vẫn bấm "Vẫn chưa hiểu" (`d-more`, giây 109). | Chọn kiểu "Giải thích dễ hơn" (explain), không mở `open-why`. | Trả lời đúng cả 3 câu, AI kết luận "overview (Trung bình)". | Không mở "Vì sao AI nghĩ vậy?" (log không có `open-why`); không làm sai câu hỏi nhanh nên chưa thấy trigger "sai câu hỏi nhanh". |
| Cách tester sửa hoặc lấy lại control | Bấm dấu X để tắt popup đọc lại slide rồi mới mở lại. | *(Không có thao tác bỏ chọn text theo log)* | Scroll slide bên trái liên tục để đối chiếu với chat. | Không cần sửa: chấp nhận gợi ý đầu tiên ("Đúng chỗ, đã rõ hơn", giây 31); không dùng "Không phải chỗ này" hay "Tắt tự nhắc". |
| Kết quả câu hỏi nhanh (đúng/sai, số lần, thời gian theo log) | Đúng ở giây 182 | Khoảng 71s từ lúc gửi tới khi trả lời đúng | Đúng ngay lần 1 | Đúng ở giây 43 |

## 4. So sánh

| Observation | Note |
|---|---|
| Option được chọn | Option A |
| Lý do và trade-off (nguyên văn nếu có) | "Mình thích cái A nhất vì bấm vào đâu nó giải thích chỗ đó luôn, không bị nhảy ra chỗ khác che mất bài". Trade-off: Thao tác bấm khối có thể lạ với người quen bôi đen text. |
| Muốn tự làm phần nào / giao AI phần nào | Muốn tự chủ động chỉ định chỗ chưa hiểu (A) thay vì AI tự đoán (C) hay phải tự gõ câu hỏi dài dòng (D). Giao AI việc phân tích trực tiếp đoạn văn đó ngắn gọn. |
| Điều chưa thoải mái ở option đã chọn | "Hơi mất công nếu mình chỉ không hiểu 1 từ nhưng phải chọn cả khối dài". |
| Evidence chống lại kỳ vọng của nhóm (so với mục 2) | Nhóm sợ Hiếu không biết chạm vào đoạn text ở option A, thực tế Hiếu định bôi đen như dùng Word và cần facilitator gợi ý click vào nguyên khối. Ở D, Hiếu lại thấy ngại hỏi vì form rườm rà. |

## 5. Bốn lớp

- **OBSERVED:** Ở Option A, Hiếu định bôi đen như Word, cần facilitator gợi ý "click vào nguyên đoạn"; sau đó chọn 2 đoạn, gửi và trả lời đúng câu hỏi nhanh ngay lần 1 (khoảng 71s sau khi gửi). Ở D và B, Hiếu tốn nhiều thời gian đọc giao diện (UI) hơn là học nội dung.
- **INTERPRETED:** Tính năng in-context (A) giúp giảm tải nhận thức (cognitive load) rất nhiều, người dùng không cần phải chuyển sự chú ý (context switch).
- **DECIDED — NEXT CHANGE (đề xuất của mình):** Chọn Option A làm hướng chính. Cần cải thiện visual affordance của việc chọn block (có thể cho phép bôi đen text bình thường và hiện tooltip).
- **STILL UNPROVEN:** Chưa rõ nếu ở một bài Lab phức tạp hơn, Option A có cung cấp đủ context để giải quyết vấn đề bằng cách chỉ giải thích từng block hay không.

## 6. Tự kiểm tra facilitation

- [x] Hiếu tự điều khiển prototype
- [x] Không narrate, không giải thích icon
- [x] Không hỏi "Bạn có thích không?"
- [x] Đã dùng câu hỏi lại khi Hiếu hỏi cách hoạt động. Chỗ mình lỡ dẫn dắt (nếu có): Lúc Hiếu cố bôi đen ở option A, có lỡ buột miệng "bạn cứ click vào nguyên đoạn đó luôn".

## 7. Facilitator log (dán CSV)

```csv
time,option,t_sec,event,detail
23:01:00,D·context/LT,0,start,
23:01:34,D·context/LT,35,open-help,từ nội dung
23:02:23,D·context/LT,84,d-send,tới=ta chia_sẻ=[slide,time,qq] ghi_chú=có
23:02:38,D·context/LT,99,d-reply-arrived,panel mở
23:02:49,D·context/LT,109,d-more,
23:03:13,D·context/LT,133,understood,sau khi hỏi tiếp
23:04:02,D·context/LT,182,quick-question,đúng (lần 1, chọn "Bản tóm tắt bị cắt giữa chừng")
23:05:35,A·context/LT,0,start,
23:07:50,A·context/LT,135,open-help,từ nội dung
23:08:27,A·context/LT,172,a-select,+token
23:08:54,A·context/LT,198,a-select,+budget
23:09:30,A·context/LT,235,a-send,chọn=[token,budget] kiểu=explain sửa_tay=false → token,budget
23:10:41,A·context/LT,306,quick-question,đúng (lần 1, chọn "Bản tóm tắt bị cắt giữa chừng")
23:12:34,B·context/LT,0,start,
23:14:02,B·context/LT,88,open-help,từ nội dung
23:15:47,B·context/LT,193,b-answer,token=đúng
23:16:40,B·context/LT,245,b-answer,budget=đúng
23:17:58,B·context/LT,324,b-answer,memory=đúng
23:17:59,B·context/LT,325,b-diag,overview (Trung bình)
23:19:07,B·context/LT,393,understood,overview
23:20:31,B·context/LT,476,quick-question,đúng (lần 1, chọn "Bản tóm tắt bị cắt giữa chừng")
23:58:12,C·context/LT,0,start,""
23:58:24,C·context/LT,12,c-nudge,"tự động sau 12s"
23:58:44,C·context/LT,31,c-accept,"budget"
23:58:55,C·context/LT,43,quick-question,"đúng (lần 1, chọn ""Bản tóm tắt bị cắt giữa chừng"")"
```
