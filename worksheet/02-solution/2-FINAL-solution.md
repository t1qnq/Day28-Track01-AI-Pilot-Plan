---
artifact: 5 — Solution Approach + 6 — Demo/Mockup/Flow (bản nộp phase Solution)
bai-tap: Solution — chốt cách làm + cho stakeholder nhìn thấy
phase: Double Diamond vòng 2 · ◆ siết (chốt 1 cách làm + 1 artifact trực quan)
time: ~12 phút (xem deck để biết khung giờ chính xác trong buổi)
input: 1-find-existing-solutions.md · 00-context.md · templates/demo-examples.md · prompts/05-demo-challenge.md
nop-cuoi: Có — bản nộp của phase Solution (Part B + C · A3 mục Solution Approach + Demo/Mockup/Flow)
---

# 2 — FINAL: Solution Approach + Demo/Mockup/Flow

Mục tiêu: chốt cách làm cho Quick Win (Build / Buy / Boost / Partner), nói rõ data & ai review cần có, và tạo 1 bản vẽ trực quan để stakeholder *nhìn* được. Đây là nửa "siết lại" của [Double Diamond](https://www.thefountaininstitute.com/blog/what-is-the-double-diamond-design-process) vòng 2 và là bản nộp của phase Solution.

Lý do làm bước này: hai cái bẫy. Một, "tự build" cho oai — trong khi 80–90% nhu cầu nội bộ chỉ cần Boost/Buy; tự build là quyết định khó rút lại nhất. Hai, chỉ nói bằng chữ — stakeholder không duyệt một đoạn văn, họ duyệt khi *nhìn thấy* flow. Không có bản vẽ → trượt Gate 4 dù lập luận tốt.

Quy tắc: **bản vẽ trực quan là BẮT BUỘC; demo chạy được chỉ là điểm cộng.** *Demo đơn giản + lập luận chặt > demo đẹp + lập luận yếu.*

## Quy trình 12 phút

```text
4 phút  — Phần A: chốt Build/Buy/Boost/Partner (decision tree + ego check)
3 phút  — Phần B: data & ai review cần có
5 phút  — Phần C: vẽ 1 artifact trực quan + đánh dấu chỗ người review
```

---

## Phần A — Chốt cách làm

Đi decision tree, đừng chọn theo cảm giác:

```text
Bài này có phải LỢI THẾ CẠNH TRANH CỐT LÕI không?
 ├─ CÓ  → đội có AI engineer mạnh? CÓ → Build · KHÔNG → Boost
 └─ KHÔNG (chỉ là productivity layer) → có tool sẵn?
          CÓ → Buy · KHÔNG → Boost (model sẵn + data riêng)
```

Câu hỏi phụ:

- Nhóm chọn cách này vì *cần* hay vì *thích tự build*? Một câu thành thật.
- Hướng nào ở file `1` (đã tìm được người làm rồi) khớp với cách này — "đi từ 5 lên"?

### Trả lời

- **Cách làm chốt**: **Boost** — dùng model/chat tool có sẵn + prompt/persona riêng + rubric 5 Gate + worksheet/pitch của nhóm + coach review.
- **Lý do CẦN (không phải thích), 2–3 câu**: Quick Win này là một lớp luyện phản biện trước pitch, không phải lợi thế cạnh tranh cốt lõi cần tự xây model. Cái cần riêng của AI20k là rubric 5 Gate, bối cảnh Day 28 và cách hỏi đúng vào lỗ hổng của AI Pilot Plan; những phần đó có thể đưa vào prompt/context. Boost giúp nhóm thử nhanh trong lab, đo được câu hỏi có bám Gate không, và sửa prompt/rubric mapping nếu output chưa tốt.
- **Vì sao KHÔNG "Build từ số 0"**: Build full Expert Review Simulator sẽ kéo theo UI, timer, multi-persona, lưu transcript, scoring, dashboard coach và calibration phức tạp. Với pilot nhỏ, phần rủi ro nhất không phải code mà là chất lượng câu hỏi có sát rubric hay không; vì vậy cần chứng minh bằng prompt + review trước khi build.
- **Tool / API / vendor cần + ước lượng chi phí thô** (budget nhỏ, ưu tiên sẵn có): Dùng ChatGPT/Custom GPT hoặc OpenAI API/Responses API; nếu chạy qua API có thể dùng File Search hoặc upload context để đưa `rubric-gate-sheet.md`, worksheet và prompt. Chi phí thô cho pilot 25–27 nhóm: 🧮 nếu mỗi nhóm chạy 1–2 lượt sinh câu hỏi + Q&A ngắn, chi phí API dự kiến ở mức thấp (vài USD đến dưới ~20 USD, tùy model/token); cần kiểm lại bảng giá OpenAI tại thời điểm chạy pilot: https://developers.openai.com/api/docs/pricing. Không mua tool role-play riêng trong pilot.

## Phần B — Data & ai review (cách làm này cần gì để chạy được)

| Cần gì | Có sẵn trong AI20k? | Trong lab dùng (mẫu/giả định) | Privacy? |
|---|---|---|---|
| Data: rubric 5 Gate + checklist phản biện | Có trong `templates/rubric-gate-sheet.md`, README, handbook | Dùng trực tiếp rubric 5 Gate và 3 câu phản biện mặc định | Thấp, là tài liệu khóa học. |
| Data: draft AI Pilot Plan / worksheet / 5-slide pitch của nhóm | Có khi nhóm tự cung cấp | Dùng 1 bản draft của nhóm hoặc 3–5 draft mẫu ẩn danh | Có. Chỉ dùng dữ liệu nhóm tự gửi; không công khai transcript. |
| Data: persona phản biện | Có từ track card: business owner/domain expert, finance, privacy/legal, coach | Pilot chỉ dùng 1 persona chính: business owner bám 5 Gate; persona phụ chỉ dùng nếu cần follow-up | Thấp nếu chỉ là vai giả lập; tránh giả làm chuyên gia thật ở domain sâu. |
| Data: ví dụ câu hỏi tốt/xấu để calibrate | Chưa chắc có | Coach tạo hoặc duyệt 10–20 câu hỏi mẫu đầu tiên | Thấp, nhưng cần người review để tránh câu hỏi chung chung. |

- **Output nào rủi ro cao** (sai gây hậu quả): Câu hỏi phản biện và feedback sau Q&A có thể làm nhóm sửa sai hướng, tưởng mình đã luyện đủ, hoặc hiểu nhầm là đã "pass" trước khi coach xem. Output rủi ro cao nhất là phần nhận xét sau Q&A nếu AI tự đánh giá chất lượng câu trả lời như chấm điểm.
- **Ai review + bao nhiêu mẫu + pass/fail theo gì**: 1 coach/instructor review ít nhất 20 output đầu hoặc 20% số phiên pilot, tùy số nào lớn hơn. Pass khi: (1) ≥80% câu hỏi map rõ vào 1 trong 5 Gate; (2) mỗi câu hỏi chỉ ra lý do hỏi hoặc lỗ hổng cần kiểm; (3) 0 câu hỏi bịa thông tin ngoài draft; (4) 0 output kết luận pass/fail thay coach; (5) học viên đọc xong biết cần chuẩn bị bằng chứng gì.
- **Có cần citation / nói "không biết" khi thiếu nguồn không**: Có. Nếu câu hỏi dựa trên rubric/tài liệu Day 28 thì phải ghi Gate hoặc nguồn liên quan. Nếu draft nhóm thiếu thông tin, AI phải hỏi ngược "chưa đủ dữ liệu để phản biện mục này" thay vì tự bịa vấn đề.

## Phần C — Bản vẽ trực quan (BẮT BUỘC)

Chọn **Dạng 3 — Luồng prompt + Dạng 5 — Ví dụ vào–ra**. Đây là artifact tối giản nhất vì stakeholder cần nhìn ngay: input là draft nào, AI tạo câu hỏi kiểu gì, con người review ở đâu.

```text
LUỒNG PROMPT — QUICK WIN: 5 CÂU PHẢN BIỆN BÁM 5 GATE

[INPUT: nhóm dán vào tool]
  - 5-slide pitch draft hoặc AI Pilot Plan draft
  - Track + Quick Win của nhóm
  - Rubric 5 Gate
  - Ràng buộc: formative, không pass/fail, không bịa, hỏi theo business owner
      │
      ▼
[B1: lấy nguồn/rubric]
  - Gate 1: Breakdown
  - Gate 2: Quick Win
  - Gate 3: Problem Framing
  - Gate 4: Solution + visual
  - Gate 5: Pilot Plan
  Nếu thiếu thông tin trong draft → ghi "chưa đủ dữ liệu", không tự đoán
      │
      ▼
[B2: prompt + model]
  Persona: business owner khó tính nhưng công bằng.
  Nhiệm vụ: sinh đúng 5 câu hỏi, mỗi câu map 1 Gate,
  kèm "vì sao hỏi" và "bằng chứng nhóm nên chuẩn bị".
      │
      ▼
[OUTPUT DRAFT: 5 câu phản biện]
  ┌─────────────────────────────────────────────────────────────┐
  │ Gate 3 — Problem Framing                                     │
  │ Câu hỏi: Số 25-27 nhóm và baseline lỗi Gate lấy từ đâu?      │
  │ Vì sao hỏi: Nếu baseline chỉ là ước lượng, pilot khó chứng   │
  │ minh tốt hơn hiện tại.                                      │
  │ Chuẩn bị: nêu nguồn giả định + cách đo 3-5 draft trước pilot.│
  └─────────────────────────────────────────────────────────────┘
      │
      ▼
[NGƯỜI REVIEW]
  Coach/instructor xem mẫu output:
  - câu hỏi có bám Gate không?
  - có hỏi chung chung không?
  - có bịa thông tin ngoài draft không?
  - có biến thành chấm pass/fail không?
      │
      ▼
[NHÓM DÙNG ĐỂ LUYỆN]
  Nhóm trả lời 5 câu trong 5 phút,
  ghi lại phần cần sửa vào worksheet/pitch,
  không coi output là điểm chính thức.
```

### Ví dụ input–output thật (dùng dữ liệu mẫu từ chính worksheet nhóm)

```text
INPUT:
  Track 7 — Expert Review Simulator.
  Quick Win: AI sinh 5 câu phản biện bám rubric 5 Gate cho AI Pilot Plan Day 28.
  Problem framing nói rằng có khoảng 25-27 nhóm, coach không đủ thời gian Q&A thử,
  baseline hiện tại là nhóm chỉ chuẩn bị 3 câu phản biện mặc định.

OUTPUT MONG MUỐN:
  1. Gate 3 — Problem Framing
     Câu hỏi: "Bạn lấy số 25-27 nhóm và nhu cầu 125-135 phút coach time từ đâu,
     và trước pilot bạn sẽ đo baseline lỗi Gate như thế nào?"
     Vì sao hỏi: Gate 3 yêu cầu pain có số và baseline; nếu chỉ ước lượng thì
     stakeholder khó tin pilot đang giải đúng pain.
     Bằng chứng cần chuẩn bị: nguồn từ 80 học viên/nhóm 3 người + kế hoạch review
     3-5 draft trước pilot để đếm lỗi Gate nghiêm trọng.

  2. Gate 4 — Solution + visual
     Câu hỏi: "Stakeholder nhìn vào đâu để hiểu tool sẽ tạo câu hỏi khác với
     một chatbot hỏi chung chung?"
     Vì sao hỏi: red flag của track là AI hỏi câu chung chung.
     Bằng chứng cần chuẩn bị: flow prompt + mẫu output có Gate, câu hỏi, lý do hỏi,
     bằng chứng cần chuẩn bị.
```

**Chỗ con người review (output rủi ro cao) nằm ở**:

```text
Ngay sau OUTPUT DRAFT và trước khi cho nhiều nhóm dùng. Coach/instructor review mẫu câu hỏi để duyệt format, loại câu hỏi chung chung, và chặn output pass/fail. Trong pilot, AI chỉ được phản biện formative; coach vẫn là người đánh giá thật.
```

Câu hỏi phụ — một người đóng vai stakeholder nhìn 20 giây: *hiểu user làm gì, nhận lại gì, không cần giải thích thêm không? Có chỗ nào "đẹp nhưng rỗng" không?*

Trả lời: nhìn flow là thấy user dán draft → AI lấy rubric 5 Gate → sinh 5 câu hỏi có lý do → coach review → nhóm luyện và sửa pitch. Artifact không cần UI đẹp, timer, dashboard hay multi-persona để validate Quick Win này.

---

## Tổng kiểm tra trước khi sang `../03-pilot-plan/`

| Hạng mục | Xong? |
|---|---|
| Cách làm có lý do CẦN, không phải "mặc định tự build" | Có |
| Nói rõ data cần + ai review output rủi ro cao | Có |
| Có ≥1 bản vẽ trực quan, người ngoài hiểu trong ~20 giây | Có |
| Có đánh dấu chỗ con người review | Có |

⚑ Coach kiểm tra ở Mốc 3: *"Stakeholder nhìn vào đâu để hiểu flow? Mockup/sketch/demo đâu?"* → Nhìn vào **Luồng prompt — Quick Win: 5 câu phản biện bám 5 Gate** và ví dụ input–output ngay phía trên.

Sau bước này, mở `../03-pilot-plan/1-pilot-plan.md`.

*Liên quan: handbook §A5+§A6 · `templates/demo-examples.md` · `prompts/05-demo-challenge.md`*
