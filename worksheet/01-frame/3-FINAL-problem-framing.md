---
artifact: 4 — Problem Framing (bản nộp phase Frame)
bai-tap: Frame — đóng khung vấn đề thật
phase: Double Diamond vòng 1 · ◆ output (chốt — owner xác nhận)
time: ~13 phút (xem deck để biết khung giờ chính xác trong buổi)
input: 2-quick-win.md · prompts/03-problem-framing-challenge.md
nop-cuoi: Có — đây là bản nộp của phase Frame (Part A · A3 Working Canvas mục Problem Framing)
---

# 3 — FINAL: Problem Framing

Mục tiêu: đóng khung Quick Win đã chọn cho thật cụ thể. Đây **không phải** bản đề xuất giải pháp — là tài liệu trả lời đúng 1 câu: *"nhóm đã hiểu đúng vấn đề chưa?"*. Đây là output chốt của [Double Diamond](https://www.thefountaininstitute.com/blog/what-is-the-double-diamond-design-process) vòng 1, và là một mục trong A3 Working Canvas nộp cuối buổi.

Lý do làm bước này: một AI Pilot Plan cho vấn đề SAI — dù viết hay — vẫn sai. Đa số nhóm trượt Gate 3 vì khung chung chung ("học viên cần học tốt hơn", "coach quá tải") — câu đó không đo được, không ai chịu trách nhiệm, không biết khi nào thành công.

Quy tắc: **pain phải có số.** "Nhiều người phàn nàn" không phải evidence. "200 câu hỏi/tuần × 20 phút = 67 giờ/tuần" mới là evidence. Trong lab dùng số giả định cũng được, nhưng phải nói rõ số đến từ đâu.

## Quy trình 13 phút

```text
9 phút  — Điền 9 mục Problem Framing
3 phút  — Tự phản biện
1 phút  — Chốt: owner (giả định) có xác nhận đúng vấn đề không
```

---

## 9 mục Problem Framing

Câu hỏi phụ (tự trả lời trước khi điền):

- Một người ngoài đọc khung này có biết CHÍNH XÁC ai đau, đau cái gì không?
- Nếu KHÔNG có baseline thì nhóm đo "tốt hơn" bằng cách nào?
- Mục Open Questions trống = nguy hiểm (chưa nghĩ đủ). Nhóm còn chưa biết gì?

### Trả lời

1. **Original Ask** (stakeholder nói gì, nguyên văn): Xây một công cụ AI mô phỏng business owner/domain expert để phản biện Problem Framing, Solution Approach, AI Pilot Plan và pitch trước khi học viên present thật.
2. **Reframed problem** (vấn đề thật sau khi tách): Các nhóm Day 28 thường chỉ phát hiện lỗ hổng trong AI Pilot Plan khi bị hỏi ở lúc pitch thật; lúc đó đã quá muộn để sửa sâu Problem Framing, metric, budget, exit criteria hoặc lời xin. Vấn đề cần giải trước tiên là tạo một phiên phản biện giả lập ngắn, bám rubric, để nhóm tự phát hiện điểm yếu trước khi trình bày.
3. **Current workflow** (hiện tại đang xử lý thế nào, kể cả "không ai làm gì"): Nhóm tự đọc rubric 5 Gate, chuẩn bị 5-slide pitch và 3 câu phản biện mặc định trong worksheet. Coach/instructor có thể hỏi ở các mốc, nhưng không đủ thời gian để mô phỏng Q&A sâu cho từng nhóm trước khi pitch cuối.
4. **Pain evidence — bằng SỐ** (ai đau · đau ở khoảnh khắc nào trong việc · tần suất · quy mô; số giả định ghi rõ nguồn giả định):

```text
Giả định từ bối cảnh lab:
- Track Product có khoảng 80 học viên, chia nhóm 3 người -> khoảng 25-27 nhóm.
- Nếu mỗi nhóm cần 5 phút Q&A thử với coach trước pitch, tổng nhu cầu là khoảng 125-135 phút coach time, chưa tính thời gian đọc bản nháp và góp ý.
- Lab Day 28 chỉ khoảng 70 phút, nên không đủ thời gian để coach phản biện riêng từng nhóm.
- Khoảnh khắc đau nhất: 5-10 phút trước pitch, nhóm không biết AI Pilot Plan còn thiếu baseline, metric, exit criteria, budget hay lời xin rõ ràng.
- Baseline hiện tại: nhóm chỉ chuẩn bị 3 câu phản biện mặc định; chưa có Q&A cá nhân hóa theo chính bản nháp của nhóm.
```

5. **Affected people** (ai dùng · ai quyết · ai là người review/expert): Người dùng đầu tiên là nhóm học viên chuẩn bị pitch Day 28. Người hưởng lợi gián tiếp là coach/instructor vì nhóm vào pitch với plan ít lỗi cơ bản hơn. Người review/expert là coach hoặc instructor kiểm tra xem câu hỏi AI có bám rubric và không thay thế phản biện thật.
6. **Constraints** (từ `00-context.md`: privacy / human review / citation / budget / formative / adoption): Chỉ dùng dữ liệu nhóm tự cung cấp như worksheet, AI Pilot Plan draft và 5-slide pitch; không dùng dữ liệu riêng tư ngoài phạm vi lab. AI chỉ hỗ trợ luyện tập/formative, không kết luận pass/fail và không thay coach. Câu hỏi phải bám rubric 5 Gate; thiếu thông tin thì hỏi ngược, không bịa. Pilot phải dùng tool/API có sẵn, không xây platform lớn. Adoption phải nằm trong workflow thật: nhóm dùng trước pitch.
7. **Quick Win đã chọn** (1 dòng, lấy từ file `2`): AI sinh 5 câu phản biện cho AI Pilot Plan Day 28 và mô phỏng 1 phiên business owner Q&A trong 5 phút.
8. **Open questions** (còn chưa biết gì — không được để trống): Coach đánh giá thế nào là "câu hỏi bám rubric"? Một phiên Q&A 5 phút nên có bao nhiêu câu hỏi follow-up? Sau Q&A, AI nên đưa feedback theo format nào để nhóm sửa nhanh mà không hiểu nhầm là chấm điểm? Có cần lưu transcript để coach xem lại không?
9. **Validation** (đóng vai owner: *"đúng, đây là vấn đề đáng giải"* — Có / Chưa, vì sao):

```text
Có, owner giả định xác nhận đây là vấn đề đáng giải vì nó nhỏ, đo được và nằm đúng khoảnh khắc đau trước pitch. Quick Win không cố xây full Expert Review Simulator; chỉ kiểm tra một lát cắt có giá trị rõ: nhóm có phát hiện thêm lỗ hổng trước khi pitch hay không.
```

---

## Tự phản biện

- Khung này còn câu chung chung kiểu "cần học tốt hơn" không?
- 3 câu sẽ bị hỏi: *số/giả định lấy ở đâu · giả định chính sai thì sao · tình huống nào khiến dừng.* Trả lời thử 1 câu.

Trả lời thử: Số 25-27 nhóm là ước tính từ bối cảnh track Product khoảng 80 học viên, nhóm 3 người. Nếu giả định này sai, pilot vẫn chạy được vì đơn vị đo chính là số nhóm dùng thử và chất lượng câu hỏi trên từng nhóm, không phụ thuộc chính xác vào tổng số nhóm toàn track.

---

## Tổng kiểm tra trước khi sang `02-solution/`

| Hạng mục | Xong? |
|---|---|
| Chỉ rõ 1 nhóm người + 1 khoảnh khắc cụ thể (không "user nói chung") | Có |
| Pain có số (hoặc kế hoạch lấy số), nói rõ số từ đâu | Có |
| Có baseline (hoặc cách đo baseline) + ≥1 chỉ số có ngưỡng | Có |
| Mục 9: owner (giả định) xác nhận đúng vấn đề = qua cổng phase Frame | Có |

⚑ Coach kiểm tra ở Mốc 2: *"Ai đau? Baseline là gì? Không có baseline thì đo thế nào?"*

Owner chưa xác nhận → quay lại file `1`/`2`, đừng sang Solution. Owner xác nhận → mở `../02-solution/1-find-existing-solutions.md`.

*Liên quan: handbook §A4 · `prompts/03-problem-framing-challenge.md`*
