---
artifact: 7 — AI Pilot Plan core
bai-tap: Pilot Plan — cam kết hai chiều: xin – hứa – đo – dừng
phase: Double Diamond vòng 2 · ◇ giãn → ◆ siết (liệt kê hết rồi chốt gọn)
time: ~10 phút (xem deck để biết khung giờ chính xác trong buổi)
input: 02-solution/2-FINAL-solution.md · 00-context.md · prompts/06-pilot-plan-challenge.md
nop-cuoi: Không — file trung gian (bản nộp ở 2-FINAL-pitch.md)
---

# 1 — AI Pilot Plan core

Mục tiêu: viết phần kế hoạch xin pilot — scope, người, data, budget, timeline, metric, exit criteria, adoption, lời hứa, lời xin. Bước này giãn ra (liệt kê hết những thứ cần) rồi siết lại (chốt bản gọn đủ để stakeholder quyết).

Lý do làm bước này: đây là thứ stakeholder dùng để **quyết approve hay dừng**. AI Pilot Plan **không phải proposal xin tiền** — là *cam kết hai chiều*: nhóm xin nguồn lực, đổi lại hứa giao evidence + chấp nhận dừng nếu metric fail. Demo đẹp mà không nói được "xin gì, hứa gì, đo gì, dừng khi nào" → trượt Gate 5.

Quy tắc: **budget tách từng hạng mục, không gộp 1 cục; không có mục "miscellaneous".** Exit criteria phải có người có quyền thực thi, không chỉ trên giấy.

## Quy trình 10 phút

```text
6 phút  — Điền 10 mục core (kéo nguyên liệu từ 00 + 01-frame + 02-solution)
3 phút  — Phần exit criteria + adoption (chỗ nhóm hay bỏ quên)
1 phút  — Tự phản biện
```

---

## 10 mục core

Câu hỏi phụ (tự trả lời):

- Nếu tóm vấn đề không gọn trong 1 câu → nhóm chưa hiểu vấn đề.
- Exit criteria của nhóm có ai DÁM thực thi khi sếp vẫn thích pilot không?
- Adoption: ai dùng đầu tiên — không phải "cả khóa ~500 người"?

### Trả lời

1. **Tóm tắt vấn đề (1 câu)**: Các nhóm học viên track Product đã có draft AI Pilot Plan nhưng thiếu công cụ tự rà soát theo 5 Gate trước khi pitch, dẫn đến mất thời gian Q&A thực tế của coach vào các lỗi cơ bản.
2. **Cách làm + Lý do KHÔNG chọn cách khác**: **Boost** — dùng AI chat tool/API có sẵn kết hợp prompt và rubric 5 Gate. KHÔNG tự build model vì tính năng này không phải lợi thế cạnh tranh cốt lõi, phần quan trọng nhất cần kiểm chứng là chất lượng câu hỏi từ prompt có bám sát rubric hay không.
3. **Phạm vi (Scope)**: Phục vụ 25-27 nhóm học viên (track Product) đang chuẩn bị pitch. Chạy thử nghiệm trong 2 tuần, chia 2 phase nhỏ (thử trên 3-5 nhóm trước, sau đó mở rộng).
4. **Người (Nhân sự & Quyền hạn)**: Nhóm 3 (Quang, Hưng, Thuận) chịu trách nhiệm build prompt và setup. **Coach/Instructor** đóng vai trò expert review bắt buộc cho 20 output đầu. AI KHÔNG được tự quyết định điểm số/kết quả (pass/fail).
5. **Dữ liệu & Privacy**: Sử dụng dữ liệu draft AI Pilot Plan và worksheet học viên (ẩn danh, tự nguyện nộp). Không lưu transcript ngoài phạm vi pilot; nếu cần lưu để coach review thì chỉ lưu bản ẩn danh, giới hạn người xem và xóa sau khi tổng hợp insight. Chọn tool/API có cấu hình lưu dữ liệu tối thiểu theo chính sách hiện hành. Yêu cầu AI bắt buộc **citation** (trích dẫn) Gate hoặc rubric tương ứng khi phản biện.
6. **Ngân sách (Budget) TỪNG HẠNG MỤC (đã bóc tách)**:
   - Chi phí API/Tool (model/chat tool có sẵn): Tối đa ~20 USD (khoảng 25 nhóm x vài lượt hỏi, tùy model/token thực tế).
   - Thời gian Coach/Instructor (Chi phí người ẩn): ~5-7 giờ để review chất lượng 20 câu hỏi đầu và 2-3 giờ hỗ trợ chấm baseline (so sánh draft trước/sau khi nhóm dùng tool).
   - Thời gian nhóm 3 setup & monitor: ~15 giờ trong 2 tuần.
   - Thời gian học viên (Hạng mục ẩn): 15-20 phút/nhóm để đọc hướng dẫn và dùng thử.
7. **Thời gian & Cổng giữa phase**:
   - Tuần 1 (Phase 1): Setup prompt, chạy nghiệm thu nghiệm ngặt với 3-5 nhóm tiên phong. 
   - **Cổng giữa**: Coach chốt "Prompt đã ổn định, AI không tự chấm pass/fail" thì mới đi tiếp.
   - Tuần 2 (Phase 2): Mở rộng cho ~20 nhóm còn lại tự luyện, khảo sát sự hữu ích.
8. **Chỉ số (SMART Metrics & Baseline)**:
   - *Metric 1 (Leading)*: Tỷ lệ câu hỏi AI map đúng 1 trong 5 Gate >= 80% (Coach trực tiếp đo trên 20 mẫu).
   - *Metric 2 (Lagging)*: Số nhóm dùng thử > 50% (13/26 nhóm) trong giai đoạn chạy pilot.
   - *Metric 3 (Outcome)*: Giảm 50% số lỗi Gate nghiêm trọng ở bản nộp cuối (Coach chấm điểm, lấy baseline từ việc so 3-5 draft trước khi dùng AI).
9. **Tiêu chí dừng (Exit Criteria) có trọng lượng**:
   - *Cảnh báo*: AI hỏi chung chung, học viên phản hồi < 50% mức hữu ích → Nhóm 3 tạm dừng để chỉnh prompt trong 1 ngày.
   - *Dừng nghiêm trọng*: AI bịa thông tin tài liệu học hoặc tự ý phán quyết "Pass/Fail" ảnh hưởng tâm lý học viên → **Instructor/Stakeholder có toàn quyền ra lệnh dừng pilot ngay lập tức** và thu hồi quyền dùng tool.
10. **Adoption (Áp dụng thực tế)**: Nhóm 3-5 nhóm tiên phong có tính chủ động cao dùng trước. Bắt buộc gắn tool vào bước "sau khi viết draft plan" và "trước buổi pitch thử". Nếu không ai dùng, nhóm cam kết gửi form để tìm hiểu (do sợ lộ data, do prompt quá lằng nhằng?) làm bài học rút kinh nghiệm.
11. **Lời hứa giao gì (Realistic)**: Giao nộp báo cáo kết quả đánh giá chất lượng prompt (tỷ lệ câu hỏi bám đúng Gate), độ thay đổi lỗi Gate trên 3-5 draft trước/sau pilot, và bộ "Prompt tối ưu" (kể cả khi kết luận cuối cùng là tool AI chưa đủ tin cậy thay thế con người).
12. **Lời xin (Rõ ràng)**: Xin phê duyệt ngân sách ~20 USD, quỹ thời gian ~10 giờ của 1 Coach chuyên trách để đồng hành lấy baseline/review, và quyền tiếp cận 3-5 nhóm tiên phong tham gia thử nghiệm Phase 1.

---

## Tự phản biện

- Budget thiếu hạng mục ẩn nào không?
- Exit criteria đủ mạnh để THẬT SỰ dừng, hay chỉ trên giấy?
- Giả định quan trọng nhất sai → plan gì?

---

## Tổng kiểm tra trước khi sang `2-FINAL-pitch.md`

| Hạng mục | Xong? |
|---|---|
| Tóm vấn đề trong 1 câu | [x] |
| Budget tách hạng mục, không "miscellaneous" | [x] |
| Metric có baseline + ngưỡng + ai đo | [x] |
| Exit criteria có người có quyền thực thi (≥2 mức) | [x] |
| Adoption: chỉ rõ ai dùng đầu tiên (không "cả khóa") | [x] |

⚑ Coach kiểm tra ở Mốc 4: *"Xin gì? Hứa gì? Đo gì? Dừng khi nào?"*

Sau bước này, mở `2-FINAL-pitch.md` — dồn tất cả thành 5-slide pitch + AI Support Log.

*Liên quan: handbook §A7+§A8 · `templates/ai-pilot-plan-core.md` · `prompts/06-pilot-plan-challenge.md`*
