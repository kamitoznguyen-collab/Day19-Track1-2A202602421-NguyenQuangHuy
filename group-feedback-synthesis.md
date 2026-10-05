# Group Feedback Synthesis — Tung Tung Tung Sahur · Case A

> File làm việc chung của nhóm, giữ cùng cấu trúc với bản trong repo [Lại Bá Quân](https://github.com/vxtor012/Track1_Day18_02495_LaiBaQuan/blob/main/group-feedback-synthesis.md) và [Đỗ Lê Việt Anh](https://github.com/dlvanh/Track1_Day19_2A202602491_DoLeVietAnh/blob/main/group-feedback-synthesis.md).
> Ô nào chưa có phiên test thật thì để trống. Không dùng 4 feedback để tuyên bố validated.

---

## 1. Ma trận 4 phiên test

| Nội dung | Phiên 1 (Học viên Khóa 3)<br>*Facilitator: Lại Bá Quân (A)* | Phiên 2 (Thiều Quang Vinh)<br>*Facilitator: Đỗ Lê Việt Anh (B)* | Phiên 3 (Lan - VLearn)<br>*Facilitator: Nguyễn Thị Minh Khánh (C)* | Phiên 4 (Phạm Minh Hiếu)<br>*Facilitator: Nguyễn Quang Huy (D)* | Pattern / khác biệt |
|---|---|---|---|---|---|
| **First action** | | Làm câu hỏi nhanh (quiz) trước; làm sai mới chọn phần chưa hiểu để AI giải thích lại | | Bắt đầu ở D: bấm "Tôi vẫn chưa hiểu" ở giây 35, khựng lại nhìn form trước khi gửi. Sang A: định bôi đen như Word, cần gợi ý mới chọn đoạn | Đều hướng về việc giải quyết vấn đề in-context ngay trên slide |
| **Breakdown chính** | | Đã chọn 1 đoạn và được AI giải thích xong thì không chọn tiếp được các phần còn lại | | Ban đầu định bôi đen (highlight) như dùng Word thay vì click vào nguyên khối (block) | UI affordance chưa đủ rõ ràng về cách chọn đoạn văn bản |
| **Cách lấy lại control** | | Bấm "Không đúng chỗ" | | Ở D: bấm X tắt popup để đọc lại slide rồi mở lại; ở A không có thao tác bỏ chọn (theo log) | Cần nút hủy/chọn lại dễ thấy hơn |
| **Option được chọn** | | **C** (nhận xét: trực quan nhất trong 4 phương án) | | **A** (vì bấm vào đâu giải thích chỗ đó luôn, không nhảy chỗ khác) | Dữ liệu từ 2 phiên cho thấy xu hướng ưu tiên C và A |
| **Trade-off** | | Thích nhất là chọn được đúng chỗ mình chưa hiểu để AI giải thích; không thấy đánh đổi | | Hơi mất công nếu chỉ không hiểu 1 từ nhưng phải chọn cả khối dài | Đôi lúc bất tiện khi đơn vị tương tác không như kỳ vọng |

*Cột Phiên 2 chép nguyên văn từ repo của Việt Anh; cột Phiên 4 từ [prototype-feedback-note.md](prototype-feedback-note.md). Cột Phiên 1 và 3 chờ dữ liệu từ Quân và Khánh.*

**Tín hiệu sớm từ 2 phiên:**
- First action trùng với Practice Note 3 của Day 17 (phát hiện mình bí **khi làm sai quiz**) → ủng hộ việc đặt câu hỏi nhanh / checkpoint và cho trigger "sai câu hỏi nhanh" ở C.
- Việc thao tác click khối block còn lạ lẫm với người quen bôi đen (Phiên 4) → cần cải thiện visual.

---

## 2. Ưu / nhược điểm từng phương án theo thiết kế (heuristic review, trước khi có dữ liệu test)

> Đây là đánh giá của nhóm dựa trên thiết kế và evidence Day 17, **không phải dữ liệu tester**. Dùng làm "kỳ vọng" để so với kết quả test; chỗ nào test cho ra khác thì ghi vào "Evidence chống lại kỳ vọng".

| | **A** · Chỉ vào chỗ kẹt | **B** · Chẩn đoán 3 câu | **C** · AI gợi ý chủ động | **D** · Nhờ người thật |
|---|---|---|---|---|
| **Ai xác định chỗ bí** | Học viên | AI, từ câu trả lời | AI, từ hành vi | Người thật |
| **Tốc độ tới lời giải** | ●●●●○ | ●●●○○ | ●●●●● | ●○○○○ (chờ ~10 phút) |
| **Học viên kiểm soát** | ●●●●● | ●●●○○ | ●●○○○ | ●●●●○ |
| **Trúng chỗ bí khi học viên *không biết* mình thiếu gì** | ●○○○○ | ●●●●○ | ●●●○○ | ●●●●● |
| **Công sức học viên bỏ ra** | Trung bình | Trung bình (3 câu) | Thấp | Thấp, nhưng phải chờ |
| **✅ Ưu** | Hỏi đúng đoạn; minh bạch, AI không đoán bừa; có nguồn slide | Có bằng chứng (✓ / ? / ✗) và độ chắc chắn; hợp người "không biết hỏi gì" (Note 1) | Không cần nghĩ; bắt đúng lúc sai quiz (Note 3) | Người thật hiểu ngữ cảnh; không phải kể lại từ đầu; hợp với thói quen "tra không được thì hỏi người" (Note 3) |
| **Nhược điểm** | Đòi học viên tự biết chỗ bí, đúng cái barrier của Hypothesis Problem; dễ bỏ qua hướng dẫn chọn đoạn (pilot nội bộ) | Tốn ~1 phút, dễ thấy như bị kiểm tra; Note 3: chờ lâu là chuyển sang ChatGPT | Có thể đoán sai; tự bật dễ gây phiền; dùng dữ liệu hành vi | Phải chờ; phụ thuộc người online; ngại hỏi; chia sẻ dữ liệu học |
| **Hợp với ai** | Người biết mình kẹt ở đâu | Người mơ hồ, không biết thiếu gì | Người đang vội, không muốn hỏi | Người đã thử AI mà vẫn bí |
| **Câu hỏi cần test trả lời** | Tester có tự chọn được đoạn không? | 3 câu là "được giúp" hay "bị hỏi bài"? | Tự nhắc là hữu ích hay phiền? | Con số "~10 phút" có làm bỏ cuộc không? |


---

## 3. Group Next Change *(chốt sau khi có đủ 4 phiên)*

**Một Next Change đề xuất (chưa chốt):** Lựa chọn Option A làm hướng thiết kế chính, cải tiến giao diện chọn văn bản để giống với việc bôi đen highlight hơn, và kết hợp nhẹ với trigger sai quiz từ Option C.

**Evidence nào dẫn tới quyết định này:** Tester Phiên 2 và Phiên 4 đều có chung sở thích là thao tác in-context trực tiếp trên slide. Tester Phiên 4 làm rất tốt với Option A và đánh giá cao vì không bị che lấp nội dung học. Tester Phiên 2 thấy C là hợp lý khi sai quiz. Các option như B và D tốn thời gian, rườm rà.

**Still Unproven sau bốn feedback:** Việc chọn đoạn văn bản có giúp AI giải thích tốt các case debug code Lab phức tạp hay không vẫn chưa được kiểm chứng đầy đủ.

Với Hypothesis Problem này, chúng tôi đã thử bốn cách giải. Tester đã ưu tiên mạnh mẽ việc tương tác in-context và hạn chế nhảy tab hay chờ đợi, vì vậy iteration tiếp theo chúng tôi sẽ tập trung hoàn thiện tính năng bôi khối văn bản (Option A) và bổ sung trigger thông minh khi trả lời sai (Option C).
