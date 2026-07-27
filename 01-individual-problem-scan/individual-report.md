> Case lựa chọn: **Quản lý chi tiêu cá nhân tự động**

Nhân vật ví dụ: Toàn, 1 UX/UI designer cho công ty X, lương tháng 30 triệu 1 tháng, nhưng không biết tiền đã chi vào đâu, thường xuyên vượt ngân sách, ngại nhập từng khoản, và cuối cùng là tài khoản cứ thế sụt giảm mà không biết tại sao

# 01 — Individual Problem Scan

| #   | Lăng kính                             | Problem quan sát được                                                                                                        | Ai chịu ảnh hưởng?                                                   | Dấu hiệu thật                                                                                                      |
| --- | ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| 1   | Lặp lại, tốn thời gian                | Người dùng phải nhập thủ công từng khoản chi từ thông báo ngân hàng, ví điện tử và tiền mặt vào app quản lý chi tiêu.        | Người đi làm, sinh viên, người quản lý chi tiêu gia đình             | Có thể mất 5–15 phút/ngày; thao tác xuất hiện gần như mỗi ngày; nhiều người bỏ nhập sau vài ngày hoặc vài tuần.    |
| 2   | AI có thể tốt hơn                     | Nội dung giao dịch khó hiểu nên người dùng không biết khoản tiền thuộc nhóm ăn uống, mua sắm, đi lại hay hóa đơn.            | Người dùng có nhiều tài khoản ngân hàng và ví điện tử                | Tên đơn vị nhận tiền thường viết tắt hoặc không giống tên cửa hàng; người dùng phải tự nhớ hoặc tìm lại giao dịch. |
| 3   | Lặp lại, AI có thể tốt hơn            | Một giao dịch thường bị phân loại sai và người dùng phải sửa lại cùng một loại giao dịch nhiều lần.                          | Người dùng thường xuyên mua tại cùng cửa hàng hoặc dùng cùng dịch vụ | Ví dụ giao dịch tại cửa hàng tiện lợi có thể là ăn uống, đồ gia dụng hoặc nạp tiền; lỗi lặp lại hàng tuần.         |
| 4   | Pain từ người khác                    | Các thành viên trong gia đình không ghi lại đầy đủ khoản chi chung, khiến người quản lý ngân sách không biết tiền đã đi đâu. | Gia đình, cặp đôi, nhóm ở chung                                      | Cuối tháng phải hỏi lại từng người; có khoản không ai nhớ; dễ phát sinh tranh luận về mức chi tiêu.                |
| 5   | Tốn thời gian                         | Người dùng phải mở nhiều ứng dụng ngân hàng và ví điện tử để tổng hợp toàn bộ chi tiêu trong tháng.                          | Người dùng sử dụng nhiều ngân hàng, thẻ và ví điện tử                | Có thể mất 30–60 phút mỗi lần tổng hợp; giao dịch nằm rải rác ở 3–6 nguồn khác nhau.                               |
| 6   | AI có thể tốt hơn                     | Người dùng chỉ phát hiện vượt ngân sách sau khi tiền đã gần hết hoặc khi kiểm tra vào cuối tháng.                            | Sinh viên, người có thu nhập cố định, gia đình                       | Thường xuyên thiếu tiền vào tuần cuối tháng; ngân sách tháng bị vượt nhưng không có cảnh báo sớm.                  |
| 7   | AI có thể tốt hơn                     | Người dùng không nhận ra các khoản chi bất thường, giao dịch trùng hoặc mức giá tăng đột biến.                               | Người dùng có nhiều giao dịch nhỏ hoặc thanh toán tự động            | Giao dịch nhỏ dễ bị bỏ qua; có thể phát hiện muộn các khoản trừ tiền hai lần hoặc phí đăng ký tăng.                |
| 8   | Lặp lại                               | Các khoản đăng ký định kỳ như ứng dụng, giải trí, lưu trữ hoặc phòng tập tiếp tục bị trừ tiền dù ít sử dụng.                 | Người đi làm, sinh viên                                              | Nhiều khoản nhỏ được trừ hàng tháng; người dùng chỉ phát hiện khi xem sao kê hoặc số dư giảm mạnh.                 |
| 9   | Tốn thời gian, AI có thể tốt hơn      | Người dùng có dữ liệu chi tiêu nhưng không biết nên cắt khoản nào để đạt mục tiêu tiết kiệm.                                 | Người muốn lập quỹ khẩn cấp, mua tài sản hoặc trả nợ                 | Báo cáo chỉ hiển thị biểu đồ, không đưa ra hành động cụ thể; người dùng vẫn phải tự phân tích.                     |
| 10  | Pain từ người khác, AI có thể tốt hơn | Người quản lý tài chính gia đình khó phân biệt khoản chi cá nhân, khoản chi chung và khoản cần hoàn trả.                     | Gia đình, cặp đôi, nhóm ở chung                                      | Phải nhắn tin hỏi lại hoặc chia hóa đơn thủ công; dễ quên hoàn tiền và tính sai phần đóng góp.                     |
# Top 3

|Rank|Problem|Vì sao chọn|Điều còn chưa chắc|
|---|---|---|---|
|1|Người dùng phải tổng hợp và phân loại thủ công giao dịch từ nhiều nguồn|Xảy ra thường xuyên, workflow rõ, tốn thời gian và là nguyên nhân khiến dữ liệu chi tiêu không đầy đủ|Hệ điều hành và ngân hàng có cho phép đọc thông báo ổn định không; tỷ lệ giao dịch tiền mặt là bao nhiêu|
|2|Người dùng chỉ biết mình vượt ngân sách khi đã quá muộn|Impact trực tiếp đến hành vi chi tiêu và khả năng tiết kiệm; có metric rõ|Người dùng có thực sự thay đổi hành vi khi nhận cảnh báo không; cảnh báo ở mức nào là phù hợp|
|3|Người dùng không phát hiện giao dịch bất thường và khoản đăng ký không còn cần thiết|Có giá trị tài chính trực tiếp, dễ tạo cảm giác “AI giúp tiết kiệm tiền”|Định nghĩa “bất thường” khác nhau giữa từng người; cảnh báo sai có thể gây khó chịu|

---

# Problem Card 1 — Tự động thu thập và phân loại giao dịch

```text
┌──────────────────────────────────────────────────────┐
│ PROBLEM CARD #1                                      │
│                                                      │
│ Problem 1 câu: Người dùng phải tự tổng hợp và phân   │
│ loại giao dịch từ nhiều ngân hàng, ví và tiền mặt.   │
│                                                      │
│ Ai chịu ảnh hưởng? Người đi làm, sinh viên và người  │
│ quản lý tài chính gia đình có nhiều nguồn thanh toán.│
│                                                      │
│ Workflow hiện tại:                                   │
│ 1. Nhận thông báo → 2. Mở ứng dụng ngân hàng         │
│ → 3. Nhớ mục đích chi → 4. Nhập và phân loại         │
│                                                      │
│ Bước nghẽn nhất: Nhập và phân loại (5–15 phút/ngày)  │
│                                                      │
│ Đo thành công bằng gì?                               │
│ Giảm thời gian nhập từ 10 phút xuống dưới 2 phút/ngày│
│                                                      │
│ Quick gut: □ No AI □ Rule ☑ Workflow                 │
│            □ Agent □ Chưa biết                       │
└──────────────────────────────────────────────────────┘
```

## Problem Card chi tiết

**Problem 1 câu:**
Người dùng phải tự nhập và phân loại giao dịch từ nhiều ngân hàng, ví điện tử và các khoản tiền mặt nên dữ liệu thường thiếu hoặc nhanh chóng bị bỏ cập nhật.

**Actor:**
Người đi làm, sinh viên và người quản lý chi tiêu gia đình có từ hai nguồn thanh toán trở lên.

**Thời điểm / bối cảnh:**
Sau mỗi giao dịch hoặc khi người dùng tổng hợp chi tiêu vào cuối ngày, cuối tuần hoặc cuối tháng.

**Current workflow 3–7 bước:**
1. Người dùng nhận thông báo giao dịch từ ngân hàng hoặc ví điện tử.
2. Người dùng bỏ qua thông báo hoặc dự định nhập lại sau.    
3. Người dùng mở từng ứng dụng để xem lịch sử giao dịch.
4. Người dùng nhớ lại mục đích của từng khoản chi.
5. Người dùng nhập số tiền, thời gian và nội dung vào app quản lý.
6. Người dùng chọn danh mục chi tiêu.
7. Người dùng sửa các giao dịch nhập thiếu hoặc phân loại sai.

**Bottleneck:**
Phải đọc nội dung giao dịch, nhớ ngữ cảnh và phân loại từng khoản. Công việc nhỏ nhưng lặp lại hằng ngày, dễ bị trì hoãn.

**Impact:**
- Mất khoảng 5–15 phút mỗi ngày.
- Dữ liệu chi tiêu không đầy đủ.
- Báo cáo ngân sách không chính xác.
- Người dùng bỏ sử dụng ứng dụng sau một thời gian ngắn.
- Khó xác định khoản chi có thể cắt giảm.

**Success metric:**
- Giảm thời gian nhập dữ liệu xuống dưới 2 phút/ngày.
- Ít nhất 90% giao dịch điện tử được ghi nhận tự động.
- Ít nhất 85% giao dịch được phân loại đúng mà không cần sửa.
- Tỷ lệ người dùng duy trì theo dõi chi tiêu sau 30 ngày tăng.
- Số ngày thiếu dữ liệu trong tháng giảm.

**Non-AI alternative:**
- Cho phép import file sao kê.
- Dùng rule theo tên người nhận tiền.
- Tạo phím tắt nhập nhanh.
- Lưu danh mục mặc định cho cửa hàng đã từng xuất hiện.
- Nhắc người dùng nhập chi tiêu vào cuối ngày.

**AI hypothesis:**
AI đọc nội dung thông báo giao dịch, nhận diện số tiền, đơn vị nhận tiền và thời gian; sau đó kết hợp lịch sử chỉnh sửa để đề xuất danh mục phù hợp. Các giao dịch độ tin cậy thấp được đưa vào danh sách chờ người dùng xác nhận.

**Quick gut:**
-  Agent

## Draft workflow

```text
CURRENT STATE — khoảng 45–90 phút/tháng

[Nhận thông báo giao dịch]
→ [Bỏ qua hoặc ghi nhớ để nhập sau]
→ [Mở từng app ngân hàng/ví: 15–25']
→ [Đối chiếu và nhớ mục đích chi: 15–30']  <-- bottleneck
→ [Nhập giao dịch: 10–20']
→ [Chọn danh mục: 5–10']
→ [Sửa dữ liệu thiếu hoặc sai]

FUTURE STATE — khoảng 5–15 phút/tháng

[Hệ thống đọc thông báo giao dịch]
→ [Rule trích xuất số tiền, thời gian, tài khoản]
→ [AI nhận diện đơn vị và đề xuất danh mục]
→ [Giao dịch tin cậy cao được ghi tự động]
→ [Người dùng duyệt giao dịch chưa chắc chắn: 5–15']  <-- human boundary
→ [Hệ thống học từ chỉnh sửa]

Fallback:
Không đọc được thông báo
→ yêu cầu import sao kê hoặc nhập nhanh thủ công.

AI phân loại sai
→ người dùng sửa danh mục và hệ thống lưu preference.
```

|Card|Actor|Bottleneck|Metric|Quick gut|Vì sao chưa chọn làm #1|
|---|---|---|---|---|---|
|Cảnh báo vượt ngân sách quá muộn|Sinh viên, người có thu nhập cố định, người đang trả nợ và gia đình quản lý ngân sách theo tháng|Phải tự theo dõi và suy luận tốc độ chi tiêu; thường chỉ phát hiện khi đã gần hoặc đã vượt ngân sách|Giảm tỷ lệ tháng vượt ngân sách ít nhất 30%; tăng số tiền tiết kiệm mỗi tháng; tăng tỷ lệ điều chỉnh sau cảnh báo|Workflow|Phụ thuộc vào dữ liệu giao dịch đầy đủ và chính xác; hiệu quả còn phụ thuộc việc người dùng có thay đổi hành vi sau cảnh báo hay không|
|Phát hiện giao dịch bất thường và đăng ký lãng phí|Người đi làm, sinh viên và gia đình có nhiều tài khoản, thẻ hoặc dịch vụ định kỳ|Phải nhớ thói quen chi tiêu và tự so sánh hàng chục giao dịch để tìm khoản lạ, trùng hoặc tăng giá|Giảm thời gian phát hiện; tăng tỷ lệ bất thường được phát hiện; giảm cảnh báo sai; tăng số tiền tiết kiệm từ khoản đăng ký được hủy|Workflow|Định nghĩa “bất thường” khác nhau theo từng người, cần dữ liệu lịch sử và dễ gây mất niềm tin nếu cảnh báo sai nhiều|
