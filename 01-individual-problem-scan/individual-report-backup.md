> Case lựa chọn: **Daily log** 

Nhân vật ví dụ: Toàn, 1 UX/UI designer cho công ty X, khoảng 200 người. Mỗi ngày Toàn phải log work báo cáo công việc *hằng ngày* trên Lark và Jira.


| #   | Lăng kính             | Problem quan sát được                                                              | Ai chịu ảnh hưởng?   | Dấu hiệu thật                                                                                         |
| --- | --------------------- | ---------------------------------------------------------------------------------- | -------------------- | ----------------------------------------------------------------------------------------------------- |
| 1   | Lặp lại               | Thấp thỏm lên Lark để log từng công việc đã, đang, sẽ làm                          | Team Member          | Quên log và ngày hôm sau mới nhận ra                                                                  |
| 2   | Pain từ người khác    | Các thành viên khác trong team không nắm được đầu việc người kia                   | Cả team              | Cùng làm 1 task đó vô tình tạo ra 2 bản cùng 1 task -> phí thời gian                                  |
| 3   | Tốn thời gian         | Hết giờ hành chính mới vội vàng log work                                           | Cả team              | Chất lượng log không được cao, thiếu sót                                                              |
| 4   | Pain từ người khác    | Gây mâu thuẫn trong việc tính bảng lương                                           | HR, Member           | Thiếu ngày công -> trả lương thiếu                                                                    |
| 5   | Lặp lại               | Không nhớ mình đã làm gì vào đầu ngày hoặc giữa ngày                               | Team Member          | Cuối ngày phải mở lại Jira, Figma, Git để nhớ đã làm gì                                               |
| 6   | AI có thể tốt hơn     | Log chỉ là text, không có bằng chứng đi kèm                                        | Manager              | Manager phải hỏi thêm "đã xong thật chưa?"                                                            |
| 7   | AI có thể tốt hơn     | Daily được viết theo trí nhớ thay vì theo hoạt động thực tế                        | Team Member, Manager | Báo cáo ghi "4 giờ thiết kế", thực tế dành phần lớn thời gian để họp và review                        |
| 8   | Tốn thời gian         | Nhân viên coi daily log là việc hành chính bắt buộc                                | Team member          | Thường log sát deadline hoặc copy từ hôm trước                                                        |
| 9   | AI có thể làm tốt hơn | Working suite trên Lark không đi cùng ticket trên Jira                             | Manager              | Lộn xộn, weekly report thiếu thông tin, không khớp                                                    |
| 10  | AI có thể làm tốt hơn | Nếu xuất hiện các cuộc họp đột xuất, không thể kịp sắp xếp và không rõ log như nào | All                  | 1h đi làm nhưng họp đột xuất lúc 2h nhưng vẫn log là làm việc bình thường                             |
| 11  | Pain từ người khác    | Người mới hoặc stakeholder không nhìn được ai đang làm gì                          | Team member          | Nội dung log quá chung chung, không ai hiểu ai, mọi người chỉ log vì được bảo thế (nội dung vô nghĩa) |

## Top 3
| Rank | Problem                                             | Vì sao chọn                                            | Điều còn chưa chắc                                                    |
| ---- | --------------------------------------------------- | ------------------------------------------------------ | --------------------------------------------------------------------- |
| 1    | Nội dung log (ước lượng, chủ quan, thừa/thiếu, ...) | Gây thừa/thiếu giờ công thực tế, có thể đo metrics tốt | Nó có thực sự ảnh hưởng đến doanh nghiệp không? (dưới góc độ quản lý) |
| 2    | Các nền tảng không liên kết nhau                    | Nhiều người đau, impact rộng                           | Platform access khó                                                   |
| 3    | Nhớ nhớ quên quên                                   | Pain to, impact trực tiếp đến cá nhân và tổ chức       | Tùy vào tính cách mỗi người                                           |

## Problem Card #1 — Nhớ nhớ quên quên

**Problem (1 câu)**
Nhân viên thường quên ghi daily log đúng thời điểm, dẫn đến báo cáo thiếu chính xác hoặc bỏ sót hoàn toàn.

**Actor*
- Primary: Team Member
- Secondary: Manager, HR

**Current workflow**
1. Làm việc cả ngày.
2. Kết thúc giờ làm.
3. Về nhà hoặc chuyển sang việc cá nhân.
4. Hôm sau mới nhớ chưa log.
5. Cố nhớ lại công việc hôm trước.

**Bottleneck**
- Daily log phụ thuộc vào trí nhớ.
- Không có nhắc nhở theo ngữ cảnh.
- Sau một ngày gần như không thể nhớ đầy đủ.

**Impact**
Employee
- Thiếu giờ công.
- Áp lực khi phải nhớ lại.

Manager / HR
- Thiếu dữ liệu báo cáo.
- Sai lệch timesheet.

**Success metric**
- Tỷ lệ quên log <5%.
- Tăng tỷ lệ hoàn thành daily đúng hạn.
- Giảm số lần HR phải nhắc.

**Non-AI alternative**
- Notification lúc 5:30 PM.
- Checklist cuối ngày.
- Calendar Reminder.
- Policy bắt buộc.

**AI hypothesis**
AI phát hiện người dùng chuẩn bị kết thúc ngày làm việc hoặc đã hoàn thành phần lớn hoạt động, tự tạo draft daily log và chủ động nhắc review trước khi rời công ty.

**Quick gut**
Rule

Nếu chỉ là nhắc đúng giờ thì rule-based là đủ. Nếu cần nhận biết ngữ cảnh (đã họp xong, commit cuối ngày, đóng laptop, hoàn thành task...) rồi tự tổng hợp và nhắc đúng thời điểm thì phù hợp với Agent.

### Draft current workflow
```
CURRENT STATE - 25p

[1 Chuẩn bị kết thúc ca làm]
→ [2 Nhận ra là quên log]
→ [3 Mở lại các working tool để kiểm tra: 3p]
→ [4 Nhớ lại những gì mình làm: 10p]
→ [5 Ghi log theo đúng yêu cầu: 10p]
```

### Draft future workflow
```
[1 AI phát hiện sắp kết thúc ngày làm việc]
→ [2 AI tổng hợp hoạt động trong ngày: 10s]
→ [3 AI tạo draft daily log: 10s]
→ [4 User review + chỉnh sửa: 30–60s]  <-- human boundary
→ [5 Submit lên Lark/Jira: 5s]
```

| Card                               | Actor                    | Bottleneck                                                                                      | Metric                                                                                               | Quick gut        | Vì sao chưa chọn làm #1                                                                                                      |
| ---------------------------------- | ------------------------ | ----------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Nội dung daily log không chính xác | Team Member; Manager; HR | Cuối ngày phải nhớ lại công việc và ước lượng thời gian, dẫn đến log thiếu, sai hoặc bị làm đẹp | Thời gian log dưới 2 phút; ≥90% nội dung khớp hoạt động thực tế; giảm hỏi lại và chỉnh sửa timesheet | Agent            | Cần dữ liệu hoạt động đủ đáng tin cậy và cơ chế đo độ chính xác; rủi ro quyền riêng tư và khai khống vẫn khó xử lý hoàn toàn |
| Dữ liệu công việc phân tán         | Team Member; Manager     | Phải mở nhiều nền tảng, tự tổng hợp và liên kết các hoạt động thuộc cùng một task               | Giảm thời gian tổng hợp trên 70%; giảm số nền tảng phải mở; tăng độ đầy đủ của log                   | Workflow + Agent | Khó triển khai do phụ thuộc API, OAuth, quyền truy cập và phạm vi tích hợp rộng; phần lớn effort nằm ở integration hơn là AI |