---
artifact: 3 — Quick Win Selection
bai-tap: Frame — chọn lát cắt làm trước
phase: Double Diamond vòng 1 · ◆ siết (hội tụ về 1 lựa chọn)
time: ~10 phút (xem deck để biết khung giờ chính xác trong buổi)
input: 1-intake-breakdown.md · prompts/02-quick-win-challenge.md
nop-cuoi: Không — file trung gian (bản chốt phase này ở 3-FINAL-problem-framing.md)
---

# 2 — Quick Win: chọn lát cắt làm trước

Mục tiêu: từ 5–8 use case ở file `1`, chấm điểm nhanh và chốt **1 Quick Win** để pilot đầu tiên — kèm lý do chọn và lý do *không* chọn các phần khác. Đây là nửa "siết lại" của [Double Diamond](https://www.thefountaininstitute.com/blog/what-is-the-double-diamond-design-process) vòng 1.

Lý do làm bước này: đây là quyết định quan trọng nhất của phase Frame. Quick Win **không phải** phần dễ nhất hay nghe hay nhất — là phần *chứng minh được giá trị nhanh và có người ủng hộ*. Chọn sai → pilot fail → mất uy tín → khó xin pilot tiếp. Nhóm phải chọn được *và bảo vệ được bằng lý do*, không bằng cảm tính.

Quy tắc: **điểm số chỉ là gợi ý, không phải đáp án.** Đừng để con số quyết thay nhóm — nó chỉ giúp so sánh.

## Bước 0 — Lấy 4–6 use case mạnh nhất từ file `1` (1 phút)

## Quy trình 10 phút

```text
1 phút  — Bước 0: chọn 4–6 ứng viên
5 phút  — Phần A: chấm điểm 4 trục
3 phút  — Phần B: 1 lý do nên / 1 lý do không cho top 2
1 phút  — Phần C: chốt + ai ủng hộ + cái KHÔNG chọn
```

---

## Phần A — Chấm điểm 4 trục (1–5 mỗi trục)

Câu hỏi phụ (tự trả lời):

- "Risk" ở đây là *sai thì mất gì* — chọn đúng việc chính của user (task centrality) thì sai cũng đỡ đau; chọn việc lớn nhất thì sai rất đắt. Use case nào risk thấp thật?
- Use case nào có sẵn data + có người trong AI20k thật sự muốn dùng?

| Use case | Impact | Feasibility | Evidence nhanh | Risk (cao = an toàn) | Tổng |
|---|:--:|:--:|:--:|:--:|:--:|
| Sinh 5 câu phản biện + mô phỏng Q&A business owner 5 phút | 5 | 5 | 5 | 4 | 4.80 |
| Red-team Problem Framing: hỏi sâu ai đau, baseline, số liệu | 4 | 5 | 5 | 4 | 4.50 |
| Multi-persona review panel: business/finance/privacy/coach | 4 | 3 | 4 | 3 | 3.55 |
| AI đánh giá chất lượng câu trả lời Q&A theo rubric | 4 | 3 | 3 | 2 | 3.05 |
| Báo cáo cho coach: nhóm yếu ở Gate nào | 3 | 3 | 3 | 3 | 3.00 |

(Thang điểm chi tiết: `templates/quick-win-scoring.md`.)

## Phần B — 1 lý do nên / 1 lý do không, cho top 2

**Ứng viên A — Sinh 5 câu phản biện + mô phỏng Q&A business owner 5 phút**

```text
Nên chọn vì: bám trực tiếp vào khoảnh khắc nhóm cần nhất trước khi pitch; input có sẵn là AI Pilot Plan draft, 5-slide pitch và rubric 5 Gate; có thể test trong 1 buổi với nhiều nhóm.
Không nên vì: nếu prompt yếu, AI có thể hỏi câu chung chung và tạo cảm giác luyện xong nhưng không thật sự làm plan chắc hơn.
```

**Ứng viên B — Red-team Problem Framing**

```text
Nên chọn vì: Problem Framing là chỗ dễ làm sai nhất; nếu sửa được sớm thì cả Solution và Pilot Plan phía sau tốt hơn.
Không nên vì: phạm vi chỉ nằm ở phase Frame, chưa giúp nhóm luyện câu hỏi về budget, metric, exit criteria và lời xin ở slide cuối.
```

## Phần C — Chốt Quick Win

- **Quick Win nhóm chọn**: AI sinh 5 câu phản biện cho AI Pilot Plan Day 28 và mô phỏng 1 phiên business owner Q&A trong 5 phút.
- **Vì sao chọn cái này trước** (2–4 câu, bám điểm + impact + evidence nhanh): Use case này có tổng điểm cao nhất vì tác động trực tiếp đến chất lượng pitch, dùng được ngay với tài liệu đã có và cho bằng chứng nhanh trong 1 buổi. Nó không cần xây dashboard hay model riêng; chỉ cần prompt, rubric 5 Gate và bản nháp của nhóm. Rủi ro cũng thấp vì output chỉ dùng để luyện tập trước pitch, không phải chấm điểm chính thức.
- **Ai trong AI20k sẽ ủng hộ pilot này** (và vì sao họ care — "có người ủng hộ" thường quan trọng hơn "impact cao"): Học viên/nhóm pitch sẽ ủng hộ vì được luyện phản biện trước khi trình bày thật; coach/instructor sẽ ủng hộ vì giảm số nhóm vào pitch mà vẫn thiếu baseline, metric, exit criteria hoặc lời xin rõ ràng.
- **Nhóm KHÔNG chọn gì + vì sao** (≥2 use case bị loại): 1. Không chọn multi-persona review panel vì phạm vi rộng, dễ sa vào nhiều vai hỏi trùng ý mà chưa chắc cải thiện pitch.  2. Không chọn AI chấm chất lượng câu trả lời vì rủi ro tạo cảm giác "pass/fail" giả và cần calibration kỹ với coach.  3. Không chọn báo cáo coach dashboard vì cần dữ liệu nhiều nhóm và workflow vận hành lớn hơn một Quick Win.

---

## Phát hiện ban đầu

- Quick Win nên dừng ở "phản biện và gợi ý lỗ hổng", không đưa kết luận nhóm đã đạt/chưa đạt thay coach.

## Câu hỏi mở (mang sang Problem Framing)

- Cần định nghĩa câu hỏi "bám rubric" là gì: có thể yêu cầu mỗi câu hỏi phải map về một trong 5 Gate.

---

## Tổng kiểm tra trước khi sang `3-FINAL-problem-framing.md`

| Hạng mục | Xong? |
|---|---|
| Có bảng chấm 4 trục cho ≥4 use case | Có |
| Chốt 1 Quick Win, lý do bám số/impact (không "nghe hay") | Có |
| Nêu rõ ai ủng hộ pilot này | Có |
| Ghi rõ ≥2 phần KHÔNG chọn + lý do | Có |

⚑ Đây là phần coach kiểm tra ở Mốc 1: *"Vì sao không làm full tool? Vì sao chọn lát cắt này trước?"*

Sau bước này, mở `3-FINAL-problem-framing.md` — đóng khung vấn đề thật (bản nộp của phase Frame).

*Liên quan: handbook §A3 · `templates/quick-win-scoring.md` · `prompts/02-quick-win-challenge.md`*
