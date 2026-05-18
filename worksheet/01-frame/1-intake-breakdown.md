---
artifact: 1 — Track & Big Ask + 2 — Tool Breakdown
bai-tap: Frame — nghe đúng đề rồi tách nhỏ
phase: Double Diamond vòng 1 · ◇ giãn (nghe rộng, chưa chốt)
time: ~12 phút (xem deck để biết khung giờ chính xác trong buổi)
input: 00-context.md · track card · prompts/01-breakdown.md
nop-cuoi: Không — file trung gian (bản chốt phase này ở 3-FINAL-problem-framing.md)
---

# 1 — Intake & Breakdown: nghe đúng đề, tách nhỏ

Mục tiêu: cả nhóm hiểu giống nhau "công cụ lớn stakeholder muốn", rồi tách nó thành 5–8 use case nhỏ làm được riêng. Đây là nửa "giãn ra" của [Double Diamond](https://www.thefountaininstitute.com/blog/what-is-the-double-diamond-design-process) vòng 1 — nghe rộng, tách rộng, chưa chọn.

Lý do làm bước này: hai cái bẫy chết người ở đây. Một, nhận đề literal ("làm con chatbot") rồi nhảy vào build — trong khi yêu cầu mơ hồ thường chỉ là triệu chứng. Hai, ôm cả công cụ lớn đi pitch "build cả platform" → trượt Gate 1 ngay. Tách nhỏ là động tác bắt buộc để từ "một ý tưởng to" sang "danh sách phần làm được".

Quy tắc: **nghe trước, tách trước, chưa chọn.** Bước này không được chốt Quick Win (việc đó ở file `2`).

## Bước 0 — Đọc track card + 00-context (2 phút)

Đọc track card được giao và `00-context.md` (mục 2 đã điền). Đừng lướt.

## Quy trình 12 phút

```text
2 phút  — Bước 0: đọc track card + context
4 phút  — Phần A: phát biểu lại Big Ask bằng lời nhóm
6 phút  — Phần B: tách 5–8 use case + check độc lập
```

---

## Phần A — Phát biểu lại Big Ask bằng lời nhóm

Đừng chép lại đề. Cả nhóm nói lại "công cụ lớn stakeholder muốn" bằng lời mình. Nếu 3 người nói 3 kiểu khác nhau → chưa hiểu giống nhau, bàn thêm.

Câu hỏi phụ (tự trả lời):

- Stakeholder nói họ muốn gì, và họ thực sự *cần* gì — có khác nhau không?
- "Tại sao bây giờ?" — ở quy mô ~500 người, cái gì đang đau khiến phải làm công cụ này lúc này?
- Ai là người dùng đầu tiên thật sự, không phải "cả khóa"?

### Trả lời

- **Big Ask, viết lại bằng lời nhóm (2–3 câu)**: Nhóm cần một công cụ AI đóng vai business owner/domain expert để hỏi khó trước khi nhóm pitch AI Pilot Plan thật. Công cụ không thay coach hoặc instructor, mà giúp nhóm tự phát hiện lỗ hổng về vấn đề, dữ liệu, metric, budget, rủi ro và tiêu chí dừng trước khi vào phiên phản biện chính thức.
- **Tại sao bây giờ**: Day 28 có khoảng 25-27 nhóm Product phải pitch trong thời gian ngắn; coach/instructor khó phản biện sâu từng nhóm trước khi nộp. Nếu nhóm chỉ phát hiện lỗ hổng lúc pitch thật thì đã quá muộn để sửa Problem Framing, Solution hoặc Pilot Plan.
- **Người dùng đầu tiên cụ thể**: Nhóm học viên Product chuẩn bị pitch 5 phút cho AI Pilot Plan Day 28.

## Phần B — Tách công cụ lớn thành 5–8 use case

Nhìn mục **Big Vision Modules** trong track card. Mỗi dòng = 1 use case làm được riêng, viết dạng *"AI làm X cho ai để họ Y"* — không phải tính năng mơ hồ. Cần 5–8 dòng (ít hơn 5 = chưa tách đủ; nhiều hơn 8 = đang liệt kê vụn).

| # | Use case (AI làm gì · cho ai · để họ làm được gì) | Người dùng | Làm được độc lập? |
|---|---|---|---|
| 1 | AI sinh 5 câu phản biện cho AI Pilot Plan dựa trên rubric 5 Gate để nhóm biết phần nào dễ bị hỏi | Học viên/nhóm pitch | Có |
| 2 | AI mô phỏng phiên Q&A business owner trong 5 phút để nhóm luyện trả lời dưới áp lực thời gian | Học viên/nhóm pitch | Có |
| 3 | AI đóng vai coach để hỏi sâu phần Problem Framing: ai đau, workflow nào, baseline là gì | Học viên/nhóm pitch | Có |
| 4 | AI đóng vai finance/business owner để hỏi về budget, ROI, chi phí ẩn và lời xin pilot | Học viên/nhóm pitch | Có |
| 5 | AI đóng vai privacy/legal reviewer để hỏi về dữ liệu, consent, human review và rủi ro khi dùng AI | Học viên/nhóm pitch | Có |
| 6 | AI đánh giá chất lượng câu trả lời Q&A theo rubric nhẹ để nhóm biết câu nào còn yếu | Học viên/nhóm pitch | Có — phụ thuộc vào #2 nếu muốn có transcript thật |
| 7 | AI gợi ý bằng chứng còn thiếu sau phiên luyện pitch để nhóm sửa lại worksheet trước khi nộp | Học viên/nhóm pitch | Có — phụ thuộc vào draft worksheet/pitch |
| 8 | AI tạo báo cáo ngắn cho coach: nhóm đang yếu ở Gate nào và cần coach can thiệp gì | Coach/instructor | Có — phụ thuộc vào output #1/#2 nếu muốn chính xác hơn |

Cần ít nhất **4 use case thật sự độc lập** (làm được mà không cần cái khác xong trước). Nếu nhiều cái phụ thuộc nhau → gộp hoặc viết lại cho tách bạch.

---

## Phát hiện ban đầu

- Công cụ lớn có thể trở nên quá rộng nếu cố làm đủ multi-persona, scoring, dashboard và coaching report ngay từ đầu.
- Lát cắt dễ pilot nhất là tạo câu hỏi phản biện + Q&A 5 phút, vì chỉ cần input là AI Pilot Plan draft, 5-slide pitch và rubric 5 Gate.

## Câu hỏi mở (mang sang bước chọn Quick Win)

- Câu hỏi do AI sinh cần bám rubric 5 Gate đến mức nào để coach coi là hữu ích?
- Sau phiên Q&A, AI có nên đưa "đánh giá pass/fail" không, hay chỉ nên flag rủi ro và câu hỏi cần sửa?

---

## Tổng kiểm tra trước khi sang `2-quick-win.md`

| Hạng mục | Xong? |
|---|---|
| Cả nhóm phát biểu lại Big Ask giống nhau, không cần nhìn card | Có |
| Có 5–8 use case dạng "AI làm X cho ai để Y" | Có |
| Có ≥4 use case thật sự độc lập | Có |
| Nhóm KHÔNG còn ý định pitch "build cả platform" | Có |

Sau bước này, mở `2-quick-win.md` — chấm điểm chọn 1 lát cắt làm trước.

*Liên quan: handbook §A1+§A2 · `prompts/01-breakdown.md` · `00-context.md`*
