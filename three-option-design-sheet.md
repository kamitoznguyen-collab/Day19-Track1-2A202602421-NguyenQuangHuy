# Four-Option Design Sheet — Case A: AI Tutor (Diagnostic Refresher)

> Nhóm: **Tung Tung Tung Sahur** · Case A: AI Tutor – Diagnostic Refresher
>
> | Option | Owner | Repo |
> |---|---|---|
> | A — Chỉ vào chỗ kẹt | Lại Bá Quân (2A202602495) | [Track1_Day18_02495_LaiBaQuan](https://github.com/vxtor012/Track1_Day18_02495_LaiBaQuan) |
> | B — Chẩn đoán 3 câu | Đỗ Lê Việt Anh (2A202602491) | [Track1_Day19_2A202602491_DoLeVietAnh](https://github.com/dlvanh/Track1_Day19_2A202602491_DoLeVietAnh) |
> | C — AI gợi ý chủ động | Nguyễn Thị Minh Khánh (2A202602546) | Chưa có link (Khánh chưa đẩy repo) |
> | **D — Nhờ người thật, AI soạn yêu cầu** | **Nguyễn Quang Huy (2A202602421)** | repo này |
>


---

## Chặng 1 — Tổng hợp evidence

### 1. Evidence huddle (4 Practice Notes Day 17)

| Practice Note | User đã thực sự làm/nói gì? | Điều nhóm đang diễn giải |
|---|---|---|
| **1 — Huy** phỏng vấn học viên VLearn (nam, khoá 3) | Học 2 buổi sáng–chiều, chỉ kịp xem qua slide. Khi không hiểu thì copy nội dung, cắt hình minh hoạ hoặc chụp cả slide vào ChatGPT. *"Thực ra cái này cũng tùy, có lúc nó trả lời đúng ý mình có lúc không… có thể là do con chat trả lời hơi lan man, cũng có thể là do prompt của mình làm cho con AI clear, nên mình nghĩ là do cả 2."* Tần suất: "khá thường xuyên". | Không biết mình thiếu gì nên không hỏi trúng; AI trả lời lan man một phần do prompt mơ hồ. |
| **2 — Việt Anh** phỏng vấn học viên khoá 3 (Lab Coach) | Tra Google, rồi ChatGPT / Gemini, YouTube để học lại khái niệm. *"Nghe giảng các thầy cô thì hiểu nhưng mà có một số các lý thuyết thì nhìn slide đương nhiên nhìn lại mà nó viết tắt thì chắc chắn không hiểu"* (00:45). Mất 30 phút – 1 tiếng cho một khái niệm, thấy nản. | Bí khi **tự ôn lại slide**: thuật ngữ viết tắt, khái niệm cô đọng. Nghiêng về H2 (cách trình bày). |
| **3 — Minh Khánh** phỏng vấn học viên VLearn (Lan) | Nhận ra mình chưa hiểu **khi làm Quiz và bị sai**; quay lại tìm nội dung học lại; tìm ngoài "lúc có, lúc không"; không giải quyết được thì hỏi bạn bè / giảng viên, không bỏ qua. 1–2 lần/tuần. | **Trả lời sai quiz là thời điểm phát hiện mình bí**; khi tự tra không được thì tìm đến người thật. *(Phần hỏi ý kiến về tính năng trong note là câu hỏi giả định, không dùng làm evidence.)* |
| **4 — Quân** phỏng vấn học viên tự học Cloud | Bỏ video vì lướt quá nhanh, chuyển thẳng sang làm Lab, vừa làm vừa hỏi AI ngoài *"cái đấy nó có tác dụng gì, cái đấy nó dùng như thế nào"*. *"Bình thường là không hoàn thành được trong 4 tiếng của một bài lab đấy nhưng mà mình cũng hay phải mang về nhà để làm."* Text checkpoint dài dòng, chữ nhỏ. | Bí **khi đang làm Lab**, cần biết khái niệm dùng để làm gì trong bài; nghiêng mạnh về H2. |

**Thảo luận nhanh**

- **Lặp lại:** 4/4 người được hỏi đều tự tìm cách gỡ ngoài bài học (ChatGPT / Gemini / Google / YouTube / hỏi người khác). 3/4 dùng AI ngoài.
- **Mâu thuẫn / bất ngờ:** Không ai nói bí vì *quên kiến thức nền cũ* (H1); cả 4 đều nghiêng về **cách trình bày / cách hỏi** (H2). Note 1 tự nhận lỗi một phần ở prompt của mình. Note 4 bí ở **Lab**, không phải ở slide.
- **Vẫn là suy đoán:** H1 hay H2 là nguyên nhân chính (mới là lời tự đánh giá). Mức thời gian 30–60 phút và "không xong trong 4 tiếng" mới có từ 1 người mỗi ý.

### 2. Hypothesis Problem

> **Khi** đang học trên VLearn trong một ngày học dày (đọc lại slide lý thuyết hoặc đang làm Lab) và gặp một khái niệm / bước không hiểu, **người học** gặp khó khăn trong việc **nhận được lời giải thích trúng đúng chỗ mình chưa hiểu**, **vì** họ không xác định được mình đang thiếu gì để hỏi cho rõ (thuật ngữ viết tắt, khái niệm cô đọng, không biết đặt prompt nên ném nguyên slide vào ChatGPT), **dẫn đến** phải rời bài học sang công cụ ngoài, nhận câu trả lời lan man, mất 30–60 phút cho một chỗ bí và có lúc không xong bài Lab trong giờ.

**Evidence ban đầu hỗ trợ giả thuyết:** Note 1 (chụp slide vào ChatGPT, "do cả 2"), Note 2 (viết tắt trên slide, 30–60 phút, nản), Note 3 (phát hiện bí khi sai quiz, tự tra lúc được lúc không, rồi hỏi người), Note 4 (bí khi làm Lab, hỏi AI ngoài, mang bài về nhà).

**Điều vẫn chưa được chứng minh:**
- Chỗ bí chủ yếu do **thiếu kiến thức nền** (H1) hay do **cách trình bày / cách hỏi** (H2). 4 note đều nghiêng H2 nhưng đó là lời tự đánh giá.
- Người học có **bỏ qua phần không hiểu** hay không (Note 3 nói không bỏ qua; các note khác chưa hỏi).
- Đưa trợ giúp vào ngay trong bài (in-context) có làm người học bỏ thói quen copy sang ChatGPT không.
- Pattern có đúng với người khác ngoài 4 người luyện phỏng vấn không. Practice interview chưa phải validation.

**GATE 1 check:** Có đủ user / situation / job / barrier / consequence; có observation Day 17 từ cả 4 note; có điều chưa biết (H1 vs H2, in-context có thay được ChatGPT không).

---

## Chặng 2 — Bốn Solution Options

### 0. Hiện trạng VLearn (bối cảnh để thiết kế)

| | Hiện trạng |
|---|---|
| Hai chế độ | **Lý thuyết**: hiện chỉ có slide. **Lab**: trình đọc riêng. Sidebar có Slides / Videos / danh sách bước Lab đánh số (Brief → Chuẩn bị môi trường → Task 1.1 … → Trạm cứu hộ & FAQs → Nộp bài) / Kiến thức & Quiz cuối Day. Tiến độ tính theo "x/19 hoạt động". Hướng dẫn dạng text + ảnh + code. Phần lớn lab làm nhóm, nhưng có lab cá nhân (ví dụ Lab 3 ghi `workMode: "individual"`). |
| Nội dung | Khoảng 70% kỹ thuật (tech), 30% phi kỹ thuật (non-tech). |
| Trợ giảng AI | Đã có trên mỗi slide, video và lab: một khung chat hỏi đáp tự do ("Đặt câu hỏi với AI"), biết user đang mở slide/trang nào. |
| Hàm ý | Không cần chứng minh "có AI để hỏi". Câu hỏi của Day 18 là **khi user bí, ai xác định chỗ bí và ai khởi xướng**. Chat tự do hiện tại gần với Option A nhất, nhưng A thêm bước giúp user chỉ đúng chỗ chưa hiểu. VLearn cũng đã có nút **"Gửi yêu cầu"**; Option D dựa trên đó. Prototype thử ở cả **lý thuyết (slide)** và **Lab (bước hướng dẫn)**; tín hiệu hành vi ở Option C chỉ dùng những gì trình đọc có (thời gian dừng, quay lại trang trước, trả lời câu hỏi nhanh / checkpoint), không dùng tín hiệu video. |

**Phần bổ sung dùng chung cho cả A/B/C/D:** "Câu hỏi nhanh" dưới slide là tính năng nhóm thêm vào để cải thiện chế độ lý thuyết (ý tưởng mượn từ ví dụ trong bài giảng 3.2). Nó vừa là outcome của task (hiểu đủ để trả lời đúng), vừa là một tín hiệu bí cho Option C.

**Điểm vào chung "🙋 Tôi vẫn chưa hiểu":** hành trình giả định học viên chắc chắn sẽ bấm nút này hoặc trả lời câu hỏi nhanh khi bí, nên nút được làm nổi bật giống hệt nhau ở cả bốn option: màu đỏ VLearn, nhấp nháy 3 lần khi mở slide, có ở góc slide, ở thanh dính dưới màn hình, và trong câu hỏi nhanh khi trả lời sai. Vì có ở cả bốn option, nó không tạo khác biệt giữa các option.

### 1. Solution Parking Lot (nguồn)

| # | Hướng | Nguồn evidence | Quyết định |
|---|---|---|---|
| 1 | Học viên tự chỉ chỗ bí, AI giải thích đúng đoạn đó | Note 1 (không biết prompt nên ném nguyên slide) | **Chọn → A** |
| 2 | AI hỏi vài câu chẩn đoán trước khi giải thích | Case gốc "Diagnostic Refresher" | **Chọn → B** |
| 3 | AI tự phát hiện học viên bí (dừng lâu, sai quiz) và gợi ý | Note 3 (phát hiện bí khi sai quiz) | **Chọn → C** |
| 4 | Gửi câu hỏi cho TA / bạn cùng nhóm kèm ngữ cảnh | Note 3 (tra không được thì hỏi người) | **Chọn → D** |
| 5 | Chú giải thuật ngữ / từ viết tắt khi rê chuột trên slide | Note 2 (slide viết tắt nên tự ôn không hiểu) | Park: chỉ giải quyết một loại chỗ bí, trùng một phần với A |
| 6 | Tăng cỡ chữ, giãn dòng, rút gọn text checkpoint của Lab | Note 4 (chữ nhỏ, checkpoint dài dòng) | Park: là cải thiện UI nội dung, không phải tương tác Human–AI |
| 7 | Mốc thời gian trong video bài giảng gắn với slide | Note 4 (video lướt nhanh) | Park: phần lý thuyết hiện chỉ có slide |

Bốn hướng được chọn (xem mục 3). Bốn option dưới đây phủ đủ ba vị trí trên spectrum, có một hướng **user-led / no-inference** (A) và một hướng **human escalation** (D), đúng hai hướng mà đề nhắc phải có trong pool.

### 2. Những thứ giữ nguyên cho A/B/C/D

| Thành phần | Quyết định chung |
|---|---|
| Target user | Người tự học trên VLearn, học một mình ngoài giờ hoặc giữa buổi, không có người hỏi ngay. |
| Situation | Buổi chiều của ngày học dày; đang ở trình đọc slide của VLearn, đã đọc một slide 2 lần vẫn không hiểu; còn vài slide nữa là hết bài. |
| Task | Gỡ chỗ kẹt ở slide đó, bắt đầu từ panel Trợ giảng AI. |
| Desired outcome | Hiểu đủ để trả lời đúng **câu hỏi nhanh** ngay dưới slide và học tiếp, trong vài phút. |
| Content/data fixture | Một **chủ đề** trong ba chủ đề dưới đây, **giữ nguyên cho cả A/B/C/D trong cùng một phiên test**. Mỗi chủ đề có **2 tab riêng**: Lý thuyết (1 slide) và Lab (1 bước hướng dẫn) cùng chủ đề, dùng chung 4 khối nội dung ôn (3 phần kiến thức nền + "giải thích lại"), cùng câu chẩn đoán; mỗi tab có câu hỏi nhanh / checkpoint riêng. |

**Ba chủ đề × hai tab (Lý thuyết / Lab)**

| | Context window *(mặc định)* | ReAct agent | Gradient Descent |
|---|---|---|---|
| Tab Lý thuyết | "Bài 4 · Token và context window", slide 12: `context window ≥ token input + token output` | "Ngày 3 · Chatbot vs ReAct Agent", slide 9: Vòng lặp ReAct với Native Tool Calling | "Ngày 9 · Training mạng nơ-ron", slide 7: `w ← w − η·∂L/∂w` |
| Tab Lab | Lab 4 "Chatbot nhớ hội thoại", Task 2: cắt lịch sử chat cho vừa context window (`trim_history`) | Lab 3 "Chatbot vs ReAct Agent", Task 2.2: lập trình ReAct loop | Lab "Train MLP đầu tiên", Task 2: chọn learning rate (loss tăng vọt với lr = 1.0) |
| 3 phần kiến thức nền | Token là gì · Input + output dùng chung · Context window ≠ bộ nhớ dài hạn | Ai chạy tool (tool_calls) · Observation (role "tool") · Điều kiện dừng | Hàm loss · Đạo hàm & dấu trừ · Learning rate |
| Câu hỏi nhanh (LT) / checkpoint (Lab) | LT: 7.500 input + 1.000 output > 8.000 → bị cắt · Lab: reserve 1.000 → cắt lịch sử xuống ≤ 7.000, giữ system prompt | LT: Observation là gì · Lab: model trả về `get_weather(...)` → chạy tool, append role "tool", gọi model lại | LT: w = 3, η = 0.1 → 2.4 · Lab: loss 4 → 9 → 25 → 82 → giảm lr |
| Vì sao có | Tech dạng khái niệm. Bài giảng 3.2 (Day 18) cũng minh hoạ A/B/C bằng bài "Token và context window". | Tech dạng agent/code, đúng Lab 3 trong ảnh chụp VLearn. | Tech có công thức, kiểm tra cơ chế khi chỗ bí là phép tính. |

**Liên kết Lab ↔ Lý thuyết (trích dẫn):** mọi nội dung AI tạo ra (A, B, C) đều có nút trích dẫn đến đúng slide và đoạn liên quan: ở tab Lý thuyết là *"Nguồn: Slide 12 · '…'"*, ở tab Lab là *"Xem lại lý thuyết: Slide 12 · '…'"*. Bấm vào thì chuyển sang tab Lý thuyết và tô vàng đoạn đó ("Đoạn liên quan"). Đây là pattern **Citations / References** trong The Shape of AI, giúp user kiểm chứng câu trả lời của AI với bài giảng (đúng tinh thần dòng "Trợ giảng AI có thể sai — hãy đối chiếu với bài giảng" của VLearn). Tab Lab và Lý thuyết giữ trạng thái riêng; nếu đang chờ trả lời ở D mà chuyển tab thì tab kia có chấm đỏ báo.

Chọn chủ đề và tab bắt đầu theo relevant context của tester: ai thường bí khi đọc slide thì bắt đầu ở Lý thuyết, ai thường bí khi làm Lab thì bắt đầu ở Lab. Tester vẫn tự chuyển tab được. Ghi chủ đề + tab bắt đầu vào Feedback Note.

### 3. Những thứ khác nhau

| Thành phần | Option A: Hỏi có hướng dẫn | Option B: AI hỏi chẩn đoán | Option C: AI chủ động gợi ý | Option D: Nhờ người thật, AI soạn yêu cầu |
|---|---|---|---|---|
| **Solution mechanism** | User tự chỉ ra phần chưa hiểu trên slide + chọn kiểu giúp; hệ thống soạn sẵn câu hỏi rõ ràng, user sửa được rồi gửi. | AI hỏi 3 câu chẩn đoán ngắn, mỗi câu ứng với một phần kiến thức nền (từ nền nhất trở lên), đưa ra chẩn đoán kèm bằng chứng và độ chắc chắn; user xác nhận hoặc chọn phần khác. | AI suy luận từ tín hiệu hành vi trên slide (thời gian dừng, lật qua lại giữa các slide, trả lời sai câu hỏi nhanh, pattern của học viên khác) và tự mở sẵn phần ôn; user chấp nhận, đổi hoặc ẩn. | AI gom ngữ cảnh (slide đang học, thời gian dừng, kết quả câu hỏi nhanh) thành một yêu cầu hỗ trợ; user chọn gửi cho mentor/TA hoặc nhóm Lab, bỏ bớt dòng không muốn chia sẻ, thêm ghi chú rồi gửi; **người thật** trả lời. |
| **User làm gì?** | Tự chẩn đoán: chọn phần chưa hiểu, chọn kiểu giúp, duyệt câu hỏi. | Trả lời 3 câu; duyệt chẩn đoán. | Đọc gợi ý; nói "đúng" / "không phải" / ẩn. | Chọn người nhận, duyệt/sửa ngữ cảnh, gửi; chờ rồi đọc trả lời, hỏi tiếp nếu cần. |
| **AI làm gì?** | Chỉ trả lời câu được hỏi. Không đoán user thiếu gì. | Chẩn đoán lỗ hổng từ câu trả lời; đề xuất phần ôn. | Đoán lỗ hổng và hành động trước (hiện nội dung ôn ngay). | Chỉ soạn và chuyển yêu cầu. Không giải thích, không chẩn đoán. |
| **Trigger** | User bấm "Tôi vẫn chưa hiểu". | User bấm "Tôi vẫn chưa hiểu". | Tự động khi phát hiện dấu hiệu bí (prototype: sau ~12 giây trên slide, hoặc ngay khi trả lời sai câu hỏi nhanh) **hoặc** user bấm nút. | User bấm "Tôi vẫn chưa hiểu". |
| **Trade-off chính** | Kiểm soát cao, minh bạch; nhưng đòi user tự biết mình thiếu gì, đúng cái barrier của Hypothesis Problem. | Chẩn đoán dựa trên bằng chứng của chính user; nhưng tốn ~1 phút và có thể giống "bị kiểm tra" khi đang áp lực. | Nhanh nhất, user không phải nghĩ; nhưng dễ đoán sai, có thể gây phiền khi tự bật lên, dựa vào dữ liệu hành vi. | Người thật hiểu ngữ cảnh, đáng tin, có thể theo tiếp (gọi 5 phút, giải thích ở buổi Lab); nhưng phải **chờ** (~10 phút), phụ thuộc người có online không, có thể ngại hỏi, và phải chia sẻ dữ liệu học với người khác. |

### Distance check

- **A khác B vì:** ở A, *user* là người xác định chỗ hổng (AI không suy luận); ở B, *AI* xác định chỗ hổng dựa trên câu trả lời của user.
- **B khác C vì:** B hỏi trước rồi mới kết luận (AI **Ask**), dựa trên bằng chứng user chủ động đưa; C kết luận và hành động trước từ tín hiệu thụ động (AI **Act**), user chỉ duyệt sau.
- **A khác C vì:** A do user khởi xướng và tự soạn câu hỏi, không dùng dữ liệu hành vi; C do AI khởi xướng, dùng dữ liệu hành vi, và user chỉ phản hồi.
- **D khác A/B/C vì:** ở A/B/C, câu giải thích đến từ AI; ở D, **người thật** chẩn đoán và giải thích, AI chỉ đóng vai trò thư ký gom ngữ cảnh và chuyển đi. Đánh đổi chính chuyển từ "AI có hiểu đúng không" sang "có chờ được không và có ngại hỏi không".

```
USER CREATES / INITIATES          → Option A
USER + AI CO-CREATE               → Option B
AI CREATES / INITIATES, USER REVIEWS → Option C
HUMAN ESCALATION (AI chỉ chuẩn bị)   → Option D
```

D nằm ngoài thang trên: nó trả lời câu hỏi "có nên đưa người thật vào khi AI không đủ không", một hướng đề yêu cầu phải có trong pool. D không phải kết hợp của A/B/C nên vẫn giữ được một cơ chế chính rõ ràng.

**Liên hệ H1/H2:** B có nhánh "không thiếu kiến thức nền → giải thích lại slide" và A có kiểu "Giải thích lại dễ hơn". Nhờ đó cả hai giả thuyết H1 và H2 đều có đường đi trong prototype, không ép theo H1.

**GATE 2 check:** Cùng user/situation/task/outcome/fixture; khác ở *ai xác định chỗ hổng* (user / AI qua câu hỏi / AI qua hành vi / người thật) và *ai khởi xướng*, không phải màu hay layout.

---

## Chặng 3 — Human–AI Design pass

**Critical interaction:** khoảnh khắc từ lúc user kẹt ở slide → đến lúc nhận được phần ôn đúng chỗ (hoặc phát hiện AI đưa sai chỗ và sửa lại).

### Human–AI Decision Table


| Human–AI decision | Option A | Option B | Option C | Option D |
|---|---|---|---|---|
| **User làm gì? AI làm gì?** | User chọn phần chưa hiểu + kiểu giúp, sửa câu hỏi. AI trả lời đúng phạm vi câu hỏi. | User trả lời 3 câu (có "Không chắc", được bỏ trống). AI chẩn đoán và đưa phần ôn theo chẩn đoán. | User duyệt gợi ý. AI phát hiện kẹt, chọn phần ôn và hiện ngay. | User chọn người nhận, duyệt ngữ cảnh, gửi. AI soạn yêu cầu. Mentor/TA hoặc bạn cùng nhóm trả lời. |
| **AI Act / Ask / Don't Act? Vì sao?** | **Don't Act** về chẩn đoán: user giữ quyền định nghĩa vấn đề. Hợp với người biết mình kẹt ở đâu. | **Ask**: chẩn đoán sai thì mất thời gian ôn nhầm, nên hỏi để có bằng chứng trước khi đề xuất. | **Act** (đưa nội dung ôn nhưng không chặn bài học): khi sai, hậu quả thấp vì chỉ là một panel đóng được, đổi lại tiết kiệm thời gian. | **Act** ở việc soạn yêu cầu (AI tự điền ngữ cảnh) nhưng **Ask** trước khi gửi: user phải xem và bấm gửi, vì yêu cầu chia sẻ dữ liệu học với người khác. **Don't Act** ở phần giải thích: để người thật làm. |
| **User hiểu capability/limit bằng gì?** | Dòng kỳ vọng: "AI chỉ trả lời đúng câu bạn hỏi, dựa trên nội dung slide. AI không tự đoán bạn đang thiếu gì." | Dòng mở đầu: "Trả lời 3 câu rất ngắn (~1 phút) để AI đoán phần kiến thức nền… Không chấm điểm, không lưu kết quả." | Nhãn **TỰ NHẮC** + "Có vẻ bạn đang bí ở slide này…" + mục "Vì sao AI gợi ý phần này?" + "AI cũng có thể đoán sai". | Dòng kỳ vọng: "Trợ giảng AI soạn sẵn yêu cầu… Bạn xem, sửa rồi mới gửi. **Người thật** sẽ trả lời; AI không tự giải thích." + thời gian chờ dự kiến của từng người nhận. |
| **Evidence/uncertainty được thể hiện thế nào?** | Câu hỏi user đã gửi hiện thành bong bóng chat; nguồn "nội dung slide + câu hỏi của bạn"; nếu không nhận ra phần cụ thể thì nói rõ là đang giải thích lại cả slide. | Hàng chip ✓ / ✗ / ? / – theo từng câu **luôn hiện** trên thẻ chẩn đoán; nút "Xem chi tiết từng câu" mở ra lựa chọn của user và đáp án đúng; thanh **Độ chắc chắn Cao / Trung bình / Thấp** theo số câu sai hoặc không chắc. | Liệt kê tín hiệu (thời gian dừng ở slide, lật slide, trả lời sai câu hỏi nhanh, pattern học viên khác); "Độ chắc chắn: Trung bình. AI chưa hỏi bạn câu nào"; các phương án thay thế có % khả năng. | Người dùng thấy chính xác AI đã điền gì (từng dòng ngữ cảnh). Bất định nằm ở **thời gian chờ**: "Thường trả lời trong ~10 phút", "2/4 bạn đang online", trạng thái ⏳ đang chờ. |
| **User kiểm soát và recovery thế nào?** | Sửa câu hỏi trước khi gửi; "✎ Sửa câu hỏi" sau khi có trả lời (giữ nguyên lựa chọn); đóng panel. | "Không đúng chỗ, chọn phần khác"; "Làm lại 3 câu hỏi"; "Bỏ qua" / đóng panel. | "Không phải chỗ này" → chọn phần khác; ✕ / "Đóng và học tiếp"; "Tắt gợi ý tự động trong buổi này" (bật lại được). | Bỏ chọn dòng ngữ cảnh không muốn chia sẻ; đổi người nhận; "Huỷ yêu cầu" khi đang chờ; đóng panel học tiếp (có thông báo khi có trả lời); "Vẫn chưa hiểu" để hỏi tiếp; "Gửi yêu cầu mới". |

**Đường quay về task gốc (cả 4):** đóng panel Trợ giảng AI (slide và câu hỏi nhanh luôn nằm bên dưới); nút "↺ Làm lại" ở thanh trên xoá trạng thái và về lại đầu option; câu hỏi nhanh sai thì có "Thử lại" và "Tôi vẫn chưa hiểu".

### Feedback & data check (Option C)

- **Dữ liệu dùng:** thời gian xem slide, số lần lật slide, kết quả câu hỏi nhanh *trong phiên hiện tại*; thống kê tổng hợp "x/10 học viên" ở slide này.
- **Ghi nhớ:** chỉ ảnh hưởng phiên hiện tại, không lưu sau buổi học (ghi ở cuối panel).
- **Rút quyền:** "Tắt gợi ý tự động trong buổi này".
- Các con số "6/10 học viên" và "~55% / ~30% / ~15%" là **canned fixture** trong prototype, không phải dữ liệu thật.

### Feedback & data check (Option D)

- **Dữ liệu dùng:** slide đang học, thời gian dừng/lật slide, kết quả câu hỏi nhanh, ghi chú của user.
- **Ai thấy:** chỉ người nhận user đã chọn (mentor/TA hoặc nhóm Lab).
- **Rút quyền:** bỏ chọn từng dòng trước khi gửi; huỷ yêu cầu khi đang chờ.
- "TA Hà", "Tuấn" và các câu trả lời là **Wizard-of-Oz canned**: trả lời được mô phỏng sau ~15 giây nhưng ghi "khoảng 10 phút sau".

**GATE 3 check:** Mỗi option có expectation, agency phù hợp với hậu quả khi sai, evidence/uncertainty và ≥1 đường recovery.

---

## Chặng 4 — Micro-prototype

- **Link / cách chạy:** xem [prototype-link.md](prototype-link.md). Một file HTML duy nhất: `prototype/index.html`.
- **Giao diện:** mô phỏng trình đọc bài của VLearn (dựa trên bản ghi màn hình và ảnh chụp vlearn.dev). Có **tab Lý thuyết / Lab** ở đầu trang. Tab Lab dùng bố cục Lab: danh sách bước đánh số, tiến độ "x/y hoạt động", hướng dẫn text + code, checkpoint thay cho câu hỏi nhanh. Bố cục slide: thanh trên có tên bài + tiến độ, cột "Nội dung bài học" bên trái, slide ở giữa, **câu hỏi nhanh** dưới slide, panel **"Trợ giảng AI"** bên phải (trên điện thoại là bottom sheet), chân panel ghi "Trợ giảng AI có thể sai — hãy đối chiếu với bài giảng." như VLearn thật.
- **Cấu trúc:** `COMMON CONTEXT (slide/hướng dẫn Lab + câu hỏi nhanh/checkpoint)` → `CRITICAL INTERACTION (khác nhau)` → `RESULT (trả lời câu hỏi nhanh + hoàn tất)`.
- **Mỗi cơ chế xuất hiện ở đúng chỗ của nó** (bản trước nhét cả 4 vào cùng panel bên phải nên trông giống nhau). Vị trí được chọn theo pattern trong các thư viện AI UX [The Shape of AI](https://www.shapeof.ai/) và [AI UX Playground](https://aiuxplayground.com/):

| | Pattern tham khảo | Xuất hiện ở đâu |
|---|---|---|
| **A** | Inline Action | Ngay trên nội dung: chạm vào đoạn chưa hiểu (đoạn sáng vàng), thanh hỏi nổi ở đáy màn hình, câu trả lời mở ngay dưới đoạn đã chọn |
| **B** | Follow up + Verification | Panel chat bên phải: AI hỏi từng câu, user bấm đáp án, kết quả là thẻ chẩn đoán có thanh độ chắc chắn |
| **C** | Nudges + Disclosure + Caveat | Ngay trên nội dung: AI khoanh đỏ đoạn nó đoán ("AI nghĩ bạn bí ở đây"), thẻ gợi ý mở dưới đoạn đó kèm chip tín hiệu; "Không phải chỗ này" thì user chạm vào đoạn khác |
| **D** | Human-in-the-loop + Consent | Modal "Nhờ người hỗ trợ" (chọn người nhận, tick/bỏ dòng ngữ cảnh), sau đó panel theo dõi trạng thái Đã gửi → Đã xem → Đang trả lời → Đã trả lời |

- **Áp dụng luật UI UX Pro Max** ([nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)): icon chức năng dùng SVG thay vì emoji, focus rõ khi dùng bàn phím, tôn trọng `prefers-reduced-motion`, tương phản chữ ≥ 4.5:1, có dark mode, không dùng gradient tím kiểu "AI".
- **Thanh PROTOTYPE** (dải tối trên cùng) tách khỏi giao diện VLearn: chỉ chứa tên phương án, nút Làm lại và Danh sách.

| | Trạng thái 1 | Trạng thái 2 |
|---|---|---|
| **A** | Chạm chọn đoạn chưa hiểu + chọn kiểu giúp + xem/sửa câu hỏi (thanh nổi) | Thẻ trả lời ngay dưới đoạn đã chọn + "Sửa câu hỏi" |
| **B** | Chat: AI hỏi lần lượt 3 câu, user bấm đáp án (có "Không chắc", "Bỏ qua") | Thẻ chẩn đoán: độ chắc chắn + bằng chứng + phần ôn, kèm đổi phần ôn |
| **C** | AI khoanh đoạn + thẻ gợi ý tại chỗ (tự bật hoặc bấm nút) kèm chip tín hiệu + phần ôn | "Không phải chỗ này": chạm vào đoạn khác hoặc chọn từ danh sách |
| **D** | Modal soạn yêu cầu: chọn người nhận + tick ngữ cảnh + ghi chú | Panel theo dõi trạng thái → trả lời của người thật (+ hỏi tiếp) |

- **Phần dùng chung (~70%):** khung VLearn (header, sidebar, tab Lý thuyết / Lab, slide/hướng dẫn Lab, câu hỏi nhanh/checkpoint), nút "Tôi vẫn chưa hiểu", nút trích dẫn slide, content fixture, khối nội dung ôn, hình minh hoạ, thẻ AI (avatar, nhãn, thanh độ chắc chắn), màn hoàn tất, nút reset.
- **Facilitator log:** `#/log` ghi lại thao tác kèm mốc thời gian (first action, chấp nhận/từ chối, override, số lần trả lời câu hỏi nhanh…) để đối chiếu với ghi chép. Không hiện cho tester.

### Prototype annotation (không cho tester xem)

```
OPTION A
We expect the tester to: bấm "Tôi vẫn chưa hiểu", chạm 1–2 đoạn trên slide, gửi câu hỏi soạn sẵn, đọc thẻ trả lời ngay dưới đoạn đó rồi làm câu hỏi nhanh.
Watch for: có hiểu là phải chạm vào đoạn không; có biết chọn đoạn nào không (do dự? bấm "Hỏi cả slide này"?); có sửa câu hỏi không; có dùng "Sửa câu hỏi" khi trả lời chưa trúng không.
Do not explain: các kiểu giúp khác nhau thế nào; rằng AI không tự đoán.

OPTION B
We expect the tester to: bấm "Tôi vẫn chưa hiểu", trả lời lần lượt 3 câu trong chat, đọc thẻ chẩn đoán, ôn rồi quay lại câu hỏi nhanh.
Watch for: phản ứng khi bị "hỏi bài" (khó chịu? bấm Bỏ qua?); có đọc hàng chip bằng chứng (✓ / ? / ✗) và có bấm "Xem chi tiết từng câu" không (log ghi `open-why`); có dùng "Không chắc" không; có đổi phần ôn không.
Do not explain: vì sao phải trả lời câu hỏi; ý nghĩa độ chắc chắn.

OPTION C
We expect the tester to: đọc slide; AI khoanh một đoạn và mở thẻ gợi ý sau ~12 giây hoặc khi trả lời sai câu hỏi nhanh (hoặc tester tự bấm nút trước); đọc phần ôn, chấp nhận hoặc "Không phải chỗ này" rồi chạm đoạn khác.
Watch for: phản ứng khi AI tự khoanh đoạn (giật mình? đóng ngay?); có đọc chip tín hiệu và có bấm "Vì sao AI nghĩ vậy?" không (log ghi `open-why`); có nhận ra AI khoanh sai đoạn và chạm đoạn khác không; có tắt tự nhắc không.
Do not explain: panel tự bật vì đâu; dữ liệu hành vi được dùng thế nào.

OPTION D
We expect the tester to: bấm "Tôi vẫn chưa hiểu", trong modal chọn người nhận, xem ngữ cảnh AI điền sẵn, gửi; theo dõi trạng thái hoặc đóng panel học tiếp; đọc trả lời rồi làm câu hỏi nhanh.
Watch for: chọn mentor hay nhóm và vì sao; có bỏ chọn dòng ngữ cảnh nào không (lo ngại chia sẻ?); làm gì trong ~15 giây chờ (chờ / học tiếp / huỷ); phản ứng với "~10 phút"; có bấm "Vẫn chưa hiểu" không.
Do not explain: người trả lời là giả lập; thời gian chờ thật sẽ là bao lâu.
```

**GATE 4 check:** ✅ Đã nhờ Đỗ Lê Việt Anh tự mở và chạy thử cả 4 luồng, không gặp lỗi.

---

## Chặng 5 — Chuẩn bị test

**Relevant context (≤2 phút):**
> "Gần đây bạn có từng học một bài trên VLearn (hoặc khóa online) mà đọc lại vẫn không hiểu, rồi phải tự tìm cách gỡ không? Lần đó bạn đã làm gì?"

Dựa vào câu trả lời, chọn **chủ đề** (Context window / ReAct agent / Gradient Descent) và **tab bắt đầu** (Lý thuyết / Lab) trên màn hình chính, rồi giữ nguyên cho cả A/B/C/D.

**Outcome task (đọc giống nhau cho A/B/C/D):**
> "Trong tình huống này, hãy dùng từng phương án để hiểu slide này đủ để trả lời đúng câu hỏi nhanh bên dưới, rồi bấm hoàn tất."

**Phân công test** (theo [hướng dẫn chung của nhóm](https://github.com/vxtor012/Track1_Day18_02495_LaiBaQuan/blob/main/docs/HUONG_DAN_CHI_TIET_TUNG_NGUOI.md)): mỗi người facilitate 1 tester ngoài nhóm, cả 4 tester dùng **cùng chủ đề Context window, tab Lý thuyết (slide 12)** để so sánh được; mỗi người cho tester thử option mình phụ trách trước:

| Tester | Facilitator | Thứ tự | Link mở đầu |
|---|---|---|---|
| Tester 1 (Học viên Khóa 3) | Lại Bá Quân | A → B → C → D | `#/context/theory/A` |
| Tester 2 (Thiều Quang Vinh) | Đỗ Lê Việt Anh | B → A → C → D | `#/context/theory/B` |
| Tester 3 (Lan - VLearn) | Nguyễn Thị Minh Khánh | C → A → B → D | `#/context/theory/C` |
| **Tester 4 · Phạm Minh Hiếu (2A202602919)** | **Nguyễn Quang Huy** | **D → A → B → C** | `#/context/theory/D` |

Lưu ý: Thứ tự này không cân bằng hoàn toàn (D luôn ở cuối với 3 tester), nên khi so sánh D cần nhớ tester đã quen bài từ 3 option trước.

**Timeline 20 phút cho 4 option:** 0–2 phút làm quen + relevant context · 2–15 phút dùng A/B/C/D (~3 phút mỗi option) · 15–18 phút so sánh · 18–20 phút ghi Feedback Note.

Lưu ý: Vì cùng một slide và câu hỏi nhanh được dùng cho cả bốn option, từ option thứ hai trở đi tester đã biết đáp án. Khi quan sát option thứ 2 trở đi, tập trung vào **cách tương tác với Trợ giảng AI**, không dùng việc trả lời đúng câu hỏi nhanh làm thước đo.

**Observation focus (5):**
1. **First action** ở mỗi option.
2. **Hesitation / misunderstanding**: chỗ dừng >3 giây, đọc lại, hỏi.
3. **Evidence read / ignored**: có đọc "Vì sao AI gợi ý" (C), danh sách bằng chứng (B), câu hỏi soạn sẵn (A), ngữ cảnh AI điền sẵn (D) không.
4. **Correction / recovery**: có từ chối / sửa / đổi phần ôn / đóng panel không, bằng đường nào; có bấm trích dẫn để đối chiếu slide không (nhất là khi đang ở tab Lab).
5. **Option được chọn + trade-off** (phần so sánh cuối).

**Luật facilitation:** tester tự điều khiển · cùng task cho A/B/C/D · không narrate, không giải thích icon · không lấp im lặng · không hỏi "Bạn có thích không?" · khi bị hỏi cách hoạt động → "Theo bạn, nó nên hoạt động như thế nào?"

**Ba câu cứu hộ:** "Bạn cứ nói to suy nghĩ của mình nhé." · "Bạn sẽ làm gì tiếp theo?" · "Theo bạn, nó nên hoạt động như thế nào?"

**Opening:** "Chúng mình đang thử bốn cách thiết kế, không kiểm tra bạn. Không có câu trả lời đúng hoặc sai. Bạn hãy tự thao tác và nói to điều mình đang nghĩ; mình sẽ cố gắng không hướng dẫn."

**Compare:** "Trong tình huống này, bạn chọn A, B, C hay D? Vì sao?" · "Bạn muốn tự làm phần nào và giao cho AI phần nào?" · "Điều gì ở phương án đã chọn khiến bạn chưa thoải mái?"

Lưu ý: Nút "Tôi vẫn chưa hiểu" rất nổi bật nên tester có thể bấm trước khi C kịp tự bật sau ~12 giây. C vẫn tự bật khi trả lời sai câu hỏi nhanh. Ghi lại tester thấy C tự bật hay tự bấm nút.

**Trước mỗi tester:** mở `#/log` → "Xoá log (trước tester mới)".
