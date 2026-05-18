---
artifact: 5 — Solution Approach (phần khám phá)
bai-tap: Solution — tìm lời giải đã có sẵn trước khi tự xây
phase: Double Diamond vòng 2 · ◇ giãn (mở hết lựa chọn, chưa chốt)
time: ~8 phút (xem deck để biết khung giờ chính xác trong buổi)
input: 01-frame/3-FINAL-problem-framing.md · 00-context.md · prompts/04-find-solutions.md
nop-cuoi: Không — file trung gian (bản chốt ở 2-FINAL-solution.md)
---

# 1 — Find existing solutions (đừng xây lại từ số 0)

Mục tiêu: trước khi quyết Build / Buy / Boost / Partner, nhóm phải biết bài này đã có ai giải ở chỗ khác chưa, và họ giải bằng cách nào. Đây là nửa "giãn ra" của [Double Diamond](https://www.thefountaininstitute.com/blog/what-is-the-double-diamond-design-process) vòng 2 — mở hết các lời giải đang tồn tại, chưa chốt cái nào.

Lý do làm bước này: đây là chỗ nhiều nhóm hỏng mà không biết. Hỏng vì nhảy thẳng vào "tự build" cho oai, trong khi 80–90% nhu cầu nội bộ chỉ cần Boost hoặc Buy. Hỏng vì không hỏi "ai làm rồi" nên đi lại từ số 0. Gần như bài nào cũng đã có người giải ở một ngành khác — không thấy thì phí cả pilot.

Quy tắc: **không có nguồn = giả định.** Mỗi cái AI/web nói ra, hỏi lại "lấy ở đâu?". Không chỉ được nguồn thì đánh dấu 🧮 (giả định để giảng), đừng xài như fact.

## Bước 0 — Bài này thực ra là dạng bài gì? (2 phút)

Bỏ context AI20k sang một bên. Quick Win của nhóm là **AI sinh 5 câu phản biện bám rubric 5 Gate cho AI Pilot Plan Day 28; mô phỏng Q&A 5 phút chỉ là cách dùng thử, không phải hệ thống chấm điểm**.

- **Quick Win của nhóm, viết lại thành 1 dạng bài chung (không có chữ domain)**: Từ một bản nháp kế hoạch + rubric đánh giá, hệ thống sinh câu hỏi phản biện có mục tiêu để người viết tự phát hiện lỗ hổng trước khi trình bày.
- **Input → output thực chất là gì**: `draft plan + rubric + vai phản biện + ràng buộc` → `5 câu hỏi phản biện được map vào rubric + lý do hỏi + gợi ý bằng chứng cần chuẩn bị`.
- **Ràng buộc không bỏ được (lấy từ `00-context.md`)**: ngân sách pilot nhỏ; dùng tool/API có sẵn; output chỉ formative; câu hỏi phải bám 5 Gate/rubric; không kết luận pass/fail thay coach; dữ liệu nhóm tự cung cấp cần privacy; output rủi ro cao cần coach review.

## Quy trình 8 phút

```text
2 phút  — Bước 0: gọi tên dạng bài
4 phút  — Phần A: deep research 4 tầng "ai giải dạng bài này rồi"
2 phút  — Phần B: rút về 2–3 hướng khả thi, đánh dấu nguồn
```

---

## Phần A — Deep research: ai giải dạng bài này rồi, giải sao?

Không phải gõ 1 câu vào AI rồi chép. Chạy 4 tầng, **tầng sau lấy kết quả tầng trước làm input**. Khung câu lệnh ở `prompts/04-find-solutions.md`.

### Trả lời — điền theo 4 tầng

| Tầng | Hỏi AI/web câu gì | Tìm được gì | Nguồn / 🧮 nếu là giả định |
|---|---|---|---|
| 1 · Map | "Dạng bài draft plan + rubric → câu hỏi phản biện/role-play practice thường giải bằng hướng nào?" | Có 5 hướng chính: (1) role-play chatbot theo persona, (2) rubric-based feedback generator, (3) mock panel/Q&A simulator, (4) LLM-as-judge/evaluator có rubric, (5) human coach dùng AI để tăng tốc feedback. Với pilot nhỏ, hướng (1)+(2) là sát nhất; hướng (4) chỉ dùng để kiểm chất lượng câu hỏi, không dùng để chấm học viên. | OpenAI Education newsletter có ví dụ custom GPT role-play để sinh feedback sau luyện phỏng vấn: https://edunewsletter.openai.com/p/doan-winkel. Harvard ghi nhận giảng viên dùng ChatGPT để đọc topic sinh viên, chắt lọc vấn đề và hỗ trợ feedback: https://www.harvard.edu/ai/2024/02/02/using-chatgpt-to-assist-with-feedback/ |
| 2 · Tiền lệ | "Ai đã dùng AI để mô phỏng vai/đưa feedback cho người học hoặc người thuyết trình?" | Trong entrepreneurship education, custom GPT đã được dùng để đóng vai khách hàng/phỏng vấn, cho sinh viên luyện và nhận feedback phát triển. Harvard Business School cũng có ví dụ dùng ChatGPT để hỗ trợ feedback trên ý tưởng/kế hoạch ở nhiều thị trường khác nhau, vì giảng viên không thể chuyên sâu mọi domain. | OpenAI Education newsletter mô tả role-play customer interview + developmental feedback: https://edunewsletter.openai.com/p/doan-winkel. Harvard AI faculty voice của Rem Koning: https://www.harvard.edu/ai/2024/02/02/using-chatgpt-to-assist-with-feedback/ |
| 3 · Phản chứng | "Ca nào làm AI feedback/evaluator dễ thất bại? Nguyên nhân là gì?" | Bẫy chính là làm AI feedback nghe thuyết phục nhưng không được chuyên gia kiểm; LLM grader hoặc model-based evaluation vẫn cần human audit. Nếu nhóm biến tool thành chấm điểm/đánh giá pass-fail, rủi ro sẽ cao hơn nhiều so với chỉ sinh câu hỏi luyện tập. | OpenAI viết về evals: LLM grader có thể scale nhưng domain expert vẫn cần audit thường xuyên và review log hành vi hệ thống: https://openai.com/index/evals-drive-next-chapter-of-ai/. HBS working paper về "GenAI as a Power Persuader" cảnh báo con người có thể khó validate output AI trong bài toán quan trọng: https://www.hbs.edu/faculty/Pages/item.aspx?num=68073 |
| 4 · Thu hẹp | "Với budget nhỏ, có người review, cần citation/rubric, pilot 6 tuần thì hướng nào khả thi?" | Hướng khả thi nhất là **Boost**: dùng model sẵn có + prompt/persona riêng + rubric 5 Gate + vài ví dụ câu hỏi tốt/xấu + coach review 20 output đầu. Không cần mua role-play platform; không cần build app nhiều persona/dashboard; có thể làm bằng Custom GPT/ChatGPT/API + template output. | OpenAI File Search hỗ trợ đưa tài liệu riêng vào tool để truy hồi nguồn: https://developers.openai.com/api/docs/guides/tools-file-search. OpenAI Evals/graders docs cho thấy có thể dùng rubric/model grader để thử nghiệm chất lượng output, nhưng cần dùng như eval nội bộ, không thay expert: https://platform.openai.com/docs/guides/graders/ |

---

## Phần B — Rút về 2–3 hướng khả thi

Câu hỏi phụ:

- Hướng nào *kế thừa được nhiều nhất* từ người đã làm?
- Hướng nào nghe hay nhưng nhóm **không có nguồn** để tin?

### Trả lời

| Hướng giải khả thi | Ai làm rồi (gần bài mình nhất) | Nguồn / 🧮 | Hợp ràng buộc `00-context`? |
|---|---|---|---|
| **Buy**: mua/dùng sẵn tool role-play, interview simulator hoặc sales coaching simulator | Các tool role-play AI cho phỏng vấn, sales, customer interview; mô hình tương tự nhưng thường không bám rubric Day 28 | OpenAI Education newsletter nêu custom GPT role-play; Judgebot là ví dụ tool roleplay/rubric scoring nhưng không phải nguồn học thuật chính: https://judgebot.app/ | **Không chọn làm hướng chính**. Nhanh nhưng khó kiểm soát rubric 5 Gate, khó đảm bảo dữ liệu riêng tư/nguồn, và dễ kéo sang scoring thay vì phản biện formative. |
| **Boost**: model sẵn có + prompt/persona + rubric 5 Gate + file/context riêng + coach review | Custom GPT role-play trong giáo dục; ChatGPT hỗ trợ feedback entrepreneurship; OpenAI File Search/Evals cho retrieval và kiểm output | OpenAI Education newsletter; Harvard AI feedback; OpenAI File Search; OpenAI Evals/graders | **Chọn**. Nhỏ, rẻ, bám đúng dữ liệu AI20k, dễ thử trong lab, có human review, không tự chấm điểm. |
| **Build**: tự xây Expert Review Simulator nhiều persona, timer, transcript, scoring, coach dashboard | Các hệ role-play/simulation chuyên dụng hoặc LMS tích hợp AI | 🧮 Có thể làm sau nếu pilot chứng minh adoption; chưa có nguồn nội bộ cho nhu cầu dashboard/score | **Không chọn cho pilot**. Quá rộng, cần UI, lưu transcript, permission, calibration, dashboard; dễ trượt vì pitch full platform. |

**"Đi từ 5 lên" — nhóm kế thừa cụ thể cái gì**:

```text
Nhóm kế thừa pattern role-play + developmental feedback đã có trong giáo dục, và pattern rubric-based evaluation đã có trong OpenAI Evals. Phần nhóm tự làm không phải model mới, mà là prompt/persona "business owner phản biện AI Pilot Plan Day 28", mapping mỗi câu hỏi về 1 trong 5 Gate, và quy trình coach review để tránh AI hỏi chung chung hoặc chấm thay người thật.
```

---

## Phát hiện ban đầu

- Hướng đúng cho pilot là **Boost**, không phải Build: dùng AI có sẵn + rubric 5 Gate + prompt riêng + review của coach.
- Câu hỏi phản biện phải có cấu trúc: `Gate liên quan → câu hỏi → vì sao hỏi → bằng chứng nhóm cần chuẩn bị`. Nếu chỉ có 5 câu hỏi "nghe hay" thì chưa giải quyết red flag.
- Ranh giới an toàn: AI được sinh câu hỏi và gợi ý lỗ hổng, nhưng **không được kết luận nhóm đạt/trượt**, không thay coach/domain expert.

## Câu hỏi mở (mang sang bước chốt)

- Coach muốn review bao nhiêu output đầu tiên để calibrate: 10, 20 hay theo % nhóm dùng thử?
- Mỗi câu hỏi có cần citation tới rubric/worksheet cụ thể, hay chỉ cần map về Gate 1–5?
- Sau Q&A, tool nên lưu transcript hay chỉ xuất checklist sửa bài để giảm rủi ro privacy?

---

## Tổng kiểm tra trước khi sang `2-FINAL-solution.md`

| Hạng mục | Xong? |
|---|---|
| Gọi được dạng bài trong 1 câu, không còn chữ domain | Có |
| Đủ 4 tầng deep research, tầng nào cũng có kết quả | Có |
| Mỗi kết quả có nguồn, hoặc đánh dấu 🧮 nếu là giả định | Có |
| Rút về 2–3 hướng + nói được "đi từ 5 lên" cái gì | Có |

Hàng nào chưa xong → quay lại Phần A, đừng sang bước chốt vội.

Sau bước này, mở `2-FINAL-solution.md` — chốt Build/Buy/Boost/Partner + data & ai review + bản vẽ trực quan (đây là bản nộp của phase này).

*Liên quan: handbook §A5 · `prompts/04-find-solutions.md` · `00-context.md`*
