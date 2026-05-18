---
artifact: 8 — 5-slide Pitch + AI Support Log (bản nộp cuối lab)
bai-tap: Pilot Plan — dồn thành pitch, sẵn sàng phản biện
phase: Double Diamond vòng 2 · ◆ output (bản nộp cuối + present)
time: ~5 phút (xem deck để biết khung giờ chính xác trong buổi)
input: 1-pilot-plan.md + toàn bộ 01-frame + 02-solution · templates/5-slide-pitch.md
nop-cuoi: Có — bản nộp cuối lab (Part E · 5-slide Pitch + AI Support Log)
---

# 2 — FINAL: 5-slide Pitch + AI Support Log

Mục tiêu: dồn cả A3 Working Canvas thành 5 slide pitch (5 phút), chuẩn bị trả lời 3 câu phản biện, và ghi AI Support Log. Đây là bản nộp cuối cùng của lab.

Lý do làm bước này: nguyên tắc *demo đơn giản + lập luận chặt > demo đẹp + lập luận yếu*. Slide đẹp mà không trả lời được "số này lấy ở đâu" thì hỏng. Pitch không phải kể chuyện — là đưa evidence để stakeholder ra được một quyết định.

Quy tắc: **slide cuối phải là một lời xin rõ ràng** (xin gì · đổi lại hứa gì). Không có lời xin = stakeholder không biết approve cái gì.

## Quy trình 5 phút

```text
3 phút  — Dồn 5 slide (mỗi slide 1 thông điệp)
1 phút  — Chuẩn bị 3 câu phản biện
1 phút  — AI Support Log
```

---

## Phần A — 5 slide (mỗi slide 1 thông điệp)

Kéo nguyên liệu từ các file đã làm, đừng viết mới. Khung đầy đủ: `templates/5-slide-pitch.md`.

| # | Slide | Lấy từ | Nội dung 1–2 gạch đầu dòng | Ai nói |
|---|---|---|---|---|
| 1 | Problem & user | 01-frame/3-FINAL | - Thiếu công cụ tự rà soát trước pitch, gây mất thời gian Q&A các lỗi cơ bản. <br> - Người dùng: 25-27 nhóm học viên track Product. | Quang |
| 2 | Breakdown & Quick Win | 01-frame/1,2 | - Bóc tách: từ full Expert Review Simulator thành các use case nhỏ: sinh câu hỏi, Q&A thử, red-team Problem Framing, privacy review, coach report. <br> - Quick Win: AI sinh 5 câu phản biện bám rubric 5 Gate; Q&A 5 phút chỉ là cách dùng thử, không phải hệ thống chấm điểm. | Hưng |
| 3 | Solution + bản vẽ trực quan | 02-solution/2-FINAL | - Boost: sử dụng model/chat tool có sẵn + prompt + rubric 5 Gate + kiểm soát lưu dữ liệu tối thiểu. <br> - Flow: Draft vào → AI phân tích 5 Gate → 5 câu hỏi/phản biện → Coach review. | Hưng |
| 4 | AI Pilot Plan | 03-pilot-plan/1 | - Scope: 2 tuần, chia 2 phase (Phase 1 thử 3-5 nhóm). <br> - Budget: 20 USD API, 10h của Coach (review 20 mẫu & đo baseline), 15h của nhóm. | Thuận |
| 5 | Metric · exit criteria · **lời xin** | 03-pilot-plan/1 | - Metric: 80% câu bám Gate, giảm 50% lỗi. <br> - Exit: Dừng ngay nếu AI phán quyết Pass/Fail. <br> - **Lời xin**: Xin 20 USD, 10h Coach, 3-5 nhóm tiên phong; hứa giao Báo cáo chất lượng và Bộ Prompt tối ưu. | Thuận |

## Phần B — Chuẩn bị 3 câu phản biện

Business owner/instructor sẽ hỏi mỗi nhóm 1–2 câu. Viết sẵn câu trả lời:

1. *"Số liệu / giả định này lấy ở đâu?"* → Quy mô 25-27 nhóm lấy từ track Product hiện tại (80 người). Baseline lỗi Gate được đếm thực tế bằng tay từ 3-5 draft đầu tiên nộp trước khi dùng AI.
2. *"Nếu giả định quan trọng nhất của bạn sai thì sao?"* → Giả định lớn nhất là "nhóm sẽ dùng thử". Nếu không ai dùng, pilot sẽ đóng cửa sớm, không tốn thêm API/nhân sự; nhóm sẽ phát phiếu tìm hiểu rào cản adoption để có bài học.
3. *"Tình huống nào sẽ khiến bạn dừng pilot?"* → Khi AI vượt quyền hạn, tự phán xét "Pass/Fail" ảnh hưởng tâm lý học viên, hoặc AI bịa thông tin ngoài tài liệu khóa học.

## Phần C — AI Support Log

| Câu hỏi | Trả lời |
|---|---|
| AI giúp được gì trong lab này? | Đóng vai trò phản biện (Challenge) dựa trên prompt 06 để bóc tách các "hạng mục chi phí ẩn" (thời gian Coach đo baseline, thời gian user học cách dùng) và siết chặt tính khả thi của AI Pilot Plan. |
| AI đưa output nào nghe hợp lý nhưng nhóm phải sửa? | AI thường hứa những kết quả to tát ("nâng cao chất lượng pitch toàn khóa"), nhóm phải hạ xuống thành lời hứa cụ thể có thể giao được ngay cả khi pilot thất bại: "Bộ prompt tối ưu" và "Báo cáo nghiệm thu". |
| Phần nào nhóm tự lập luận, KHÔNG copy AI? | Quyền quyết định dừng pilot — nhóm dứt khoát trao quyền cho Instructor/Stakeholder thay vì tự nhóm giữ quyền quyết, đảm bảo tính tuân thủ và an toàn cho khóa học. |

---

## Tổng kiểm tra trước khi nộp

| Hạng mục | Xong? |
|---|---|
| 5 slide, mỗi slide 1 thông điệp, đã phân ai nói slide nào | [x] |
| Slide 5 có lời xin rõ ràng (xin gì · hứa gì) | [x] |
| Có câu trả lời sẵn cho cả 3 câu phản biện | [x] |
| AI Support Log điền đủ 3 dòng | [x] |
| Tất cả file worksheet/ đã commit + push, link dán vào Discord | [ ] |

Đây là file cuối. Pitch 5 phút + nhận phản biện theo bảng 5 Gate (`templates/rubric-gate-sheet.md`).

*Liên quan: handbook §A9 · `templates/5-slide-pitch.md` · `templates/ai-support-log.md`*
