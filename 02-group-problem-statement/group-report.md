## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|---:|---|---|---|
| 1 | Nguyễn Đăng Long | 2A202601934 | Ghi chép |
| 2 | Đào Minh Chiến | 2A202601184 | Workflow |
| 3 | Lê Đăng Tấn | 2A202601916 | Phản biện và điều phối |
| 4 | Lương Minh Quân | 2A202601308 | Research |

## Phase 3 - Group Convergence

### Danh sách 12 candidates

| # | Người đưa ra | Candidate problem | Actor chính | Bottleneck |
|---:|---|---|---|---|
| 1 | Nguyễn Đăng Long | Quản lý chi tiêu cá nhân tự động | Người dùng cá nhân | Nhập và phân loại giao dịch thủ công |
| 2 | Nguyễn Đăng Long | Phát hiện subscription không còn sử dụng | Người đăng ký nhiều dịch vụ | Không nhận ra giao dịch định kỳ đã bị trừ |
| 3 | Nguyễn Đăng Long | Chia tiền sau hoạt động nhóm | Nhóm bạn, người ở ghép, nhóm du lịch | Tập hợp người trả và tự tính phần đóng góp |
| 4 | Đào Minh Chiến | Ghi nhận và phân loại chi tiêu cá nhân | Người đi làm, sinh viên, người quản lý chi tiêu gia đình | Dữ liệu giao dịch thiếu vì thao tác nhập lặp lại |
| 5 | Đào Minh Chiến | Theo dõi ngân sách và cảnh báo vượt sớm | Sinh viên hoặc người có ngân sách cố định | Chỉ nhận ra vượt ngân sách khi đã quá muộn |
| 6 | Đào Minh Chiến | Đối soát chi tiêu chung trong gia đình | Người phụ trách tài chính gia đình | Handoff chi chung và chi riêng thiếu cấu trúc |
| 7 | Lê Đăng Tấn | Nhập và phân loại giao dịch từ nhiều nguồn | Người dùng có từ hai ngân hàng, ví hoặc khoản tiền mặt | Phải mở nhiều nguồn, nhớ ngữ cảnh và phân loại từng khoản |
| 8 | Lê Đăng Tấn | Cảnh báo vượt ngân sách quá muộn | Sinh viên, người có thu nhập cố định, gia đình | Tự suy luận tốc độ chi tiêu thay vì nhận cảnh báo sớm |
| 9 | Lê Đăng Tấn | Phát hiện giao dịch bất thường và đăng ký lãng phí | Người có nhiều tài khoản hoặc dịch vụ định kỳ | Phải tự so sánh nhiều giao dịch để tìm khoản lạ |
| 10 | Lương Minh Quân | Automatic Expense Classification | Người đi làm hoặc sinh viên ngại nhập dữ liệu | Nhập số tiền và chọn category sau mỗi lần thanh toán |
| 11 | Lương Minh Quân | Overspending Detection | Người muốn tiết kiệm hoặc kiểm soát ngân sách | Không có cảnh báo trước khi tiền gần hết |
| 12 | Lương Minh Quân | Personal Spending Insight | Người đi làm và gia đình | Dashboard hiển thị số liệu nhưng không giải thích nguyên nhân |

### Notes pitch và challenge

| Thành viên | Top 3 đã pitch | Workflow sau được đề xuất | Challenge từ nhóm |
|---|---|---|---|
| Nguyễn Đăng Long | Expense tracking; unused subscription; group expense splitting | Tự ghi nhận giao dịch, phát hiện khoản định kỳ và hỗ trợ đối soát chi nhóm | Ba workflow khác nhau có đang bị gộp thành một “ứng dụng tài chính toàn năng” không? |
| Đào Minh Chiến | Transaction classification; early budget warning; family reconciliation | Import/rule trước, AI chỉ hỗ trợ mô tả mơ hồ hoặc OCR | Data đầu vào có đủ sạch không và quyền riêng tư giữa chi chung với chi riêng nằm ở đâu? |
| Lê Đăng Tấn | Multi-source transaction entry; late budget alert; anomaly/subscription detection | Rule trích field, AI đề xuất category và người dùng review confidence thấp | Việc kết nối nhiều nguồn có làm scope nghiêng về integration hơn là giải quyết bottleneck không? |
| Lương Minh Quân | Automatic classification; overspending detection; spending insight | AI đọc notification, phân loại, dự báo và sinh insight | Có đang chọn Agent quá sớm cho một workflow cố định mà Rule hoặc Workflow đã đủ không? |

### Gom trùng và cluster

| Cluster | Candidates | Pattern chung |
|---|---|---|
| A - Ghi nhận và phân loại giao dịch | Long #1; Chiến #1; Tấn #1; Quân #1 | Người dùng phải nhập hoặc phân loại giao dịch thủ công, khiến dữ liệu chi tiêu thiếu và nhanh chóng bị bỏ cập nhật |
| B - Ngân sách và cảnh báo sớm | Chiến #2; Tấn #2; Quân #2 | Người dùng chỉ nhận ra vượt ngân sách khi kỳ chi tiêu gần kết thúc |
| C - Giao dịch định kỳ và bất thường | Long #2; Tấn #3 | Các khoản nhỏ, lặp lại hoặc khác thường bị hòa vào nhiều giao dịch hợp lệ |
| D - Chi tiêu chung và insight | Long #3; Chiến #3; Quân #3 | Người dùng cần tổng hợp, giải thích hoặc xác nhận dữ liệu chi tiêu từ nhiều người hoặc nhiều nhóm |

### Shortlist và score

Nhóm shortlist dựa trên actor, workflow, evidence, impact, scope và khả năng so sánh No AI, Rule, Workflow và Agent.

Thang điểm là 1-5.
Điểm evidence được giới hạn vì nhóm mới có cross-review nội bộ, chưa có interview hoặc log độc lập.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Ghi nhận và phân loại giao dịch cá nhân | 5 | 5 | 4 | 4 | 5 | 5 | 5 | 33 |
| Theo dõi ngân sách và cảnh báo vượt sớm | 5 | 5 | 3 | 4 | 4 | 5 | 5 | 31 |
| Personal Spending Insight | 4 | 4 | 3 | 3 | 4 | 4 | 5 | 27 |

Nhóm chọn candidate **Ghi nhận và phân loại giao dịch cá nhân**.

### Vì sao nhóm chọn candidate này

- Đây là điểm đầu nguồn trong chuỗi vấn đề tài chính cá nhân.
- Nếu giao dịch không được ghi nhận hoặc phân loại đầy đủ, báo cáo chi tiêu, cảnh báo ngân sách và spending insight đều kém tin cậy.
- Actor và workflow có thể mô tả rõ từ sau khi thanh toán đến lúc dữ liệu được lưu.
- Baseline có thể đo bằng thời gian nhập mỗi giao dịch, thời gian review mỗi ngày và tỷ lệ giao dịch bị bỏ sót.
- Có phương án No AI và Rule đủ mạnh để làm baseline trước khi dùng AI.
- Workflow có thể pilot với dữ liệu đã ẩn danh mà không cần xây một ứng dụng tài chính hoàn chỉnh.

### Vì sao không chọn các candidate còn lại

- Overspending Detection là hậu quả tiếp theo của dữ liệu thiếu, đồng thời hiệu quả còn phụ thuộc người dùng có thay đổi hành vi sau cảnh báo hay không.
- Personal Spending Insight cần dữ liệu đủ sạch và cần thống nhất thế nào là insight hữu ích trước khi đánh giá chất lượng.
- Subscription và anomaly detection có scope gần với transaction classification nhưng cần nhiều lịch sử giao dịch hơn và dễ tạo cảnh báo sai.
- Chi tiêu gia đình cần giải quyết thêm quyền riêng tư, quyền xem chi riêng và xác nhận giữa nhiều thành viên.

### Tự phản biện và disagreement

Nhóm tự phản biện từng candidate bằng các câu hỏi:

- Actor có đủ cụ thể không?
- Bottleneck có nằm ở một bước có thể quan sát không?
- Evidence có phải pain thật hay chỉ là mong muốn về tính năng?
- Rule hoặc process fix giải quyết được bao nhiêu phần?
- Agent có bị chọn quá sớm không?
- Nếu AI phân loại sai, ai phát hiện và sửa?

Disagreement chính xuất hiện ở mức can thiệp.

Quân nghiêng về Agent vì muốn hệ thống đọc notification, tự phân loại và học từ phản hồi.

Chiến và Tấn phản biện rằng phần lớn transaction có merchant và format rõ, nên import và merchant rule phải được thử trước.

Long đặt câu hỏi liệu classification có đủ tạo impact hay không, vì mục tiêu cuối của người dùng là tránh vượt ngân sách.

Nhóm giải quyết disagreement bằng cách vẽ chuỗi nguyên nhân.

Classification không phải mục tiêu cuối, nhưng là bottleneck đầu nguồn.

Nếu dữ liệu thiếu hoặc sai category, overspending alert và spending insight không thể đáng tin.

Nhóm vì vậy chọn transaction classification làm candidate để đào sâu, nhưng không chốt Agent ở Phase 3.

## Phase 4 - Quick Validation và Research

### Quick validation

Nhóm kiểm tra chéo bốn individual reports ngay trong buổi lab.

- Người dùng phải mở app hoặc xem notification sau giao dịch.
- Việc nhập và chọn category lặp lại, nên thường bị trì hoãn.
- Khi dữ liệu thiếu, báo cáo ngân sách và insight cuối kỳ không còn đáng tin.
- Các card hiện có baseline tham khảo khoảng 3 phút cho một giao dịch và 5-15 phút mỗi ngày tùy số lượng giao dịch.

#### Kết quả kiểm tra chéo trong nhóm

| Nguồn | Số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Cách nhóm sửa problem |
|---|---:|---|---|---|
| Cross-review individual Problem Cards | 4 reports | Cả bốn thành viên đều đưa ra candidate liên quan đến ghi nhận, phân loại hoặc hệ quả của dữ liệu giao dịch thiếu | Các thành viên chọn mức can thiệp khác nhau: Rule, Workflow hoặc Agent | Chọn problem trước, chưa chốt công nghệ |
| So sánh current workflow | 4 reports | Bước nhập hoặc chọn category xuất hiện lặp lại trong các workflow | Baseline thời gian chưa thống nhất giữa các card | Xem số liệu thời gian là giả định, không trình bày như log đã đo |
| So sánh non-AI alternatives | 4 reports | Import sao kê, merchant rule và nhập nhanh đều có thể giải quyết một phần pain | AI không cần thiết cho merchant đã biết | Thu hẹp AI vào case mô tả mơ hồ hoặc confidence thấp |

### Bằng chứng đã có và giả định còn mở

| Trạng thái | Nội dung | Nguồn / cách kiểm tra tiếp |
|---|---|---|
| Bằng chứng từ Problem Cards | Cả bốn thành viên đều ghi nhận thao tác nhập hoặc phân loại giao dịch là bước lặp lại và dễ bị trì hoãn | Đối chiếu bốn individual reports |
| Bằng chứng từ Problem Cards | Non-AI alternatives như import sao kê, merchant rule và category mặc định có thể xử lý một phần workflow | So sánh current/future workflow của Chiến và Tấn |
| Baseline cần kiểm chứng | Khoảng 3 phút/giao dịch và 5-15 phút/ngày mới là ước lượng từ card cá nhân | Bấm giờ một phiên nhập 10-20 giao dịch trong lab |
| Giả định còn mở | Người dùng sẵn sàng cho phép đọc notification hoặc import sao kê | Phỏng vấn về consent, privacy và phương án dữ liệu được chấp nhận |
| Giả định còn mở | Có thể tự ghi nhận ít nhất 90% giao dịch điện tử | Đối chiếu output với một mẫu 10-20 giao dịch đã ẩn thông tin nhạy cảm |
| Giả định còn mở | Có thể đạt ít nhất 85% category đúng mà không tăng effort sửa lỗi | Review cùng mẫu giao dịch bằng category rubric |
| Giả định còn mở | Dữ liệu classification tốt hơn sẽ cải thiện cảnh báo ngân sách | Chỉ kiểm chứng ở pilot sau; không dùng làm claim chính của candidate hiện tại |

### Research giải pháp hiện có

| Nguồn / tool / case             | Link                                                                                                                    | Họ giải quyết phần nào?                                                                           | Điểm mạnh                                                                                  | Khoảng trống / rủi ro                                                           | Bài học cho nhóm                                                                                               |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| YNAB transaction categorization | [YNAB Categorizing Transactions](https://support.ynab.com/en_us/categorizing-transactions-a-guide-HyRl60sks)            | Import giao dịch, chọn hoặc sửa category và bulk categorize                                       | Có workflow rõ cho imported transactions và cho phép người dùng chỉnh category             | Không tự giải quyết đầy đủ giao dịch tiền mặt hoặc context riêng của từng người | Import và rule nên là baseline; AI chỉ hỗ trợ giao dịch mơ hồ                                                  |
| Rocket Money expense tracking   | [Rocket Money Expense Tracking](https://www.rocketmoney.com/learn/personal-finance/tracking-expenses-with-rocket-money) | Kết nối tài khoản, phân tích charge/merchant/frequency và tổ chức chi tiêu theo category          | Đã có pattern nhận diện recurring charges, category và cảnh báo                            | Cần kết nối dữ liệu tài chính, phụ thuộc provider và có rủi ro privacy          | Bài toán không phải chưa có app; khoảng trống nằm ở context, consent và workflow phù hợp người dùng địa phương |
| Splitwise                       | [Splitwise](https://www.splitwise.com/)                                                                                 | Ghi nhận, phân chia và theo dõi số dư chi tiêu nhóm                                               | Có group, balance, unequal split, receipt scanning và settle up                            | Tập trung vào chi tiêu chung, không phải phân loại toàn bộ chi tiêu cá nhân     | Chi tiêu nhóm là candidate riêng, không nên gộp vào pilot classification                                       |
| Google PAIR Guidebook           | [People + AI Guidebook](https://pair.withgoogle.com/guidebook/)                                                         | Hướng dẫn xác định nhu cầu người dùng, thiết kế feedback, failure handling và ranh giới người-máy | Nhấn mạnh AI phải hỗ trợ workflow và cho người dùng khả năng hiểu, sửa hoặc từ chối output | Không cung cấp solution cụ thể cho transaction classification                   | Cần confidence threshold, human review, feedback loop và fallback rõ ngay từ pilot                             |

Research takeaway:

Các sản phẩm hiện có cho thấy import, merchant rule, recurring detection và category editing đều có thể làm bằng workflow hoặc rule.

Khoảng trống phù hợp để nhóm đào sâu là giảm ma sát sau mỗi giao dịch, giữ người dùng trong vòng review, xử lý giao dịch có mô tả mơ hồ và không tự động thực hiện hành động tài chính.

Research đã làm nhóm điều chỉnh problem từ “AI quản lý chi tiêu tự động” thành “giảm ma sát ghi nhận và phân loại giao dịch điện tử”.

Nhóm không coi dashboard, overspending prediction hoặc Agent tự hành động là scope của pilot đầu tiên.

## Phase 5 - Workflow và Problem Statement

### Current workflow bản nhóm

Actor chính là Lan, một sinh viên sử dụng tài khoản ngân hàng và ví điện tử để thanh toán các khoản ăn uống, đi lại, học tập và mua sắm.

| Bước | Actor | Input | Output | Thời gian/tần suất | Handoff | Ghi chú |
|---:|---|---|---|---|---|---|
| 1 | Lan | Nhu cầu mua hàng hoặc dịch vụ | Giao dịch được thực hiện | Mỗi khi phát sinh chi tiêu | Ngân hàng hoặc ví ghi nhận giao dịch | Có thể dùng ngân hàng, ví hoặc tiền mặt |
| 2 | Ngân hàng/ví và Lan | Notification hoặc lịch sử giao dịch | Thông tin số tiền, merchant và thời gian | Ngay sau giao dịch | Notification được chuyển cho Lan | Lan thường bỏ qua khi đang bận |
| 3 | Lan | Nhiều notification trong ngày | Danh sách khoản cần ghi | Cuối ngày hoặc cuối tuần | Lan chuyển thông tin sang app/bảng tính | Dễ quên ngữ cảnh của khoản chi |
| 4 | Lan | Lịch sử giao dịch | Số tiền và nội dung được nhập | Khoảng 3 phút/giao dịch theo card cá nhân | Dữ liệu thô chuyển sang bước phân loại | Đây là bước thao tác lặp lại |
| 5 | Lan | Merchant và mục đích chi | Category | Sau khi nhập từng giao dịch | Giao dịch đã phân loại chuyển sang báo cáo | Category có thể sai nếu merchant không rõ |
| 6 | Lan | Dữ liệu đã nhập và phân loại | Báo cáo chi tiêu và ngân sách | Cuối tuần hoặc cuối tháng | Lan dùng báo cáo để tự điều chỉnh | Nếu thiếu giao dịch, báo cáo sai |

**Bottleneck chính:**

Lan phải đọc mô tả giao dịch, nhớ ngữ cảnh và chọn category sau khi giao dịch đã kết thúc.

### Future workflow bản nhóm

```text
FUTURE STATE

[1 Lan thanh toán]
→ [2 Hệ thống đọc notification hoặc import sao kê]
→ [3 Rule trích xuất số tiền, thời gian và merchant]
→ [4 Rule phân loại merchant đã biết]
→ [5 AI đề xuất category cho giao dịch mơ hồ]
→ [6 Lan xác nhận các giao dịch confidence thấp]
→ [7 Cập nhật dashboard và ngân sách]

Human boundary:
Lan duyệt giao dịch confidence thấp và có thể sửa category.

Fallback:
Không đọc được notification hoặc có giao dịch tiền mặt → import sao kê hoặc nhập nhanh thủ công.
```

| Bước tương lai | Cơ chế chính | Người chịu trách nhiệm | Boundary / failure handling |
|---:|---|---|---|
| 1. Nhận dữ liệu giao dịch | Notification hoặc file import | Người dùng cấp quyền hoặc tải file | Không truy cập nguồn chưa được consent |
| 2. Trích xuất field | Rule/parser | Hệ thống | Parse không đủ field thì đưa vào hàng chờ |
| 3. Phân loại merchant đã biết | Merchant rule | Hệ thống | Không dùng AI khi rule đã đủ |
| 4. Gợi ý case mơ hồ | AI classification kèm confidence | Hệ thống | Không tự ghi nhận nếu confidence thấp |
| 5. Xác nhận hoặc sửa | Human review | Lan | Người dùng là owner của category cuối |
| 6. Cập nhật báo cáo | Workflow | Hệ thống | Có log để rollback category sai |

### Before/after impact

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Thao tác chính | Nhập và chọn category thủ công | Tự ghi nhận high-confidence, người dùng chỉ review phần còn lại | Đếm số thao tác trên cùng một tập giao dịch |
| Thời gian | Khoảng 3 phút/giao dịch; 5-15 phút/ngày theo card cá nhân | Giảm ít nhất 50% thời gian trên cùng một mẫu | Bấm giờ thao tác trên 10-20 giao dịch trước và sau |
| Giao dịch được ghi nhận | Có thể bỏ sót giao dịch nhỏ hoặc tiền mặt | Ít nhất 90% giao dịch điện tử được ghi nhận | Đối chiếu app với sao kê |
| Độ chính xác category | Người dùng tự phân loại, dễ sai hoặc bỏ trống | Ít nhất 85% gợi ý category đúng trước khi sửa | So sánh gợi ý với nhãn cuối do người dùng xác nhận |
| Bước thủ công | Đọc, nhập, chọn category và sửa lỗi | Xác nhận giao dịch confidence thấp | Đếm số bước cần người dùng |
| Risk mới | Dữ liệu thiếu | Privacy, merchant sai, category sai và notification bị đọc nhầm | Ghi failure category trong pilot |

### Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Lan, một sinh viên sử dụng tài khoản ngân hàng và ví điện tử để quản lý chi tiêu cá nhân. |
| **Workflow** | Sau mỗi giao dịch, Lan nhận notification, bỏ qua hoặc nhớ tạm thời, sau đó mở lại lịch sử, nhập số tiền, nhớ mục đích, chọn category và xem báo cáo cuối kỳ. |
| **Bottleneck** | Việc nhập và phân loại lặp lại sau mỗi giao dịch khiến Lan trì hoãn, quên khoản nhỏ và mất context khi nhập dồn. |
| **Impact** | Dữ liệu chi tiêu thiếu hoặc sai, Lan không biết tiền đã đi vào đâu và thường phát hiện vượt ngân sách muộn. |
| **Success Metric** | Baseline thời gian được bấm trên mẫu 10-20 giao dịch. Pilot hướng tới giảm ít nhất 50% thời gian xử lý, ghi nhận ít nhất 90% giao dịch trong mẫu và đạt ít nhất 85% gợi ý category đúng trước khi sửa, so với nhãn cuối do người dùng xác nhận. |
| **Boundary** | Chỉ xử lý giao dịch điện tử có notification hoặc file sao kê được người dùng cho phép. Không tự truy cập tài khoản ngân hàng ngoài consent, không xử lý chuyển tiền, không tự hủy giao dịch và không tự quyết định thay đổi ngân sách. |

## Phase 6 - Rule / Workflow / Agent và Decision

### Bài toán nằm ở đâu trong ma trận

Bài toán có độ mơ hồ thấp đến trung bình vì category có thể được chuẩn hóa, nhưng một merchant có thể có nhiều context khác nhau.

Bài toán có độ phức tạp trung bình vì cần nối nguồn giao dịch, trích xuất field, áp dụng rule, đề xuất category, xác nhận và cập nhật báo cáo.

Vì vậy, bài toán phù hợp với **Workflow có Rule và AI hỗ trợ một bước**, không cần Agent tự hành động.

### Cây quyết định chọn mức can thiệp

```text
Category có thể xác định bằng merchant hoặc pattern cố định không?
├── CÓ → dùng Rule.
└── KHÔNG
    ↓
Giao dịch có thể được phân loại bằng context và lịch sử chỉnh sửa không?
├── CÓ → AI gợi ý category trong Workflow.
└── KHÔNG → yêu cầu người dùng nhập hoặc xác nhận thủ công.

AI có cần tự lập kế hoạch, tự gọi nhiều công cụ hoặc tự thay đổi bước tiếp theo không?
└── KHÔNG → không chọn Agent.
```

### So sánh No AI / Rule / Workflow / Agent

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI / process fix** | Nhập nhanh cuối ngày, bảng ngân sách, checklist và import sao kê thủ công | Đủ cho người ít giao dịch hoặc chỉ dùng một nguồn | Vẫn phụ thuộc thói quen và dễ bỏ cập nhật | Dùng làm baseline |
| **Rule** | Merchant mapping, category mặc định, recurring pattern và validation | Đủ cho merchant đã biết và transaction format ổn định | Không hiểu được giao dịch mơ hồ hoặc merchant dùng nhiều context | Dùng cho phần rõ |
| **Workflow** | Đọc notification/import → trích field → rule category → AI gợi ý case mơ hồ → người dùng xác nhận → cập nhật dashboard | Phù hợp vì các bước nối tiếp khá rõ và có human review | Privacy, parse sai và category sai | **Chọn** |
| **Agent** | Tự đọc nhiều nguồn, tự đặt câu hỏi, tự thay đổi ngân sách hoặc tự thực hiện hành động tài chính | Chỉ cần khi workflow có nhánh động và cần tự quyết định nhiều bước | Quá quyền hạn, khó kiểm soát, rủi ro tài chính và privacy cao | Không chọn |

### Mức chọn

**Workflow có Rule và AI hỗ trợ phân loại giao dịch mơ hồ.**

Nhóm không chọn Agent vì hệ thống không cần tự lập kế hoạch hoặc tự quyết định bước tiếp theo.

AI chỉ được phép đề xuất category, nêu confidence và đưa giao dịch chưa chắc chắn vào hàng chờ review.

Người dùng phải xác nhận các giao dịch confidence thấp và có quyền sửa hoặc bỏ qua đề xuất.

### Ranh giới người-máy theo PAIR

| Quyết định | Máy hỗ trợ | Người quyết định |
|---|---|---|
| Đọc và chuẩn hóa field | Parser/rule trích số tiền, thời gian và merchant | Người dùng quyết định có cấp dữ liệu hay không |
| Chọn category | Rule xử lý case rõ; AI gợi ý case mơ hồ | Người dùng xác nhận hoặc sửa category confidence thấp |
| Học từ phản hồi | Hệ thống lưu preference từ chỉnh sửa | Người dùng có quyền reset hoặc bỏ preference |
| Xử lý lỗi | Hệ thống đưa giao dịch vào hàng chờ và nêu lý do | Người dùng chọn nhập thủ công, sửa hoặc bỏ qua |
| Hành động tài chính | Không được phép | Người dùng giữ toàn quyền chuyển tiền, hủy dịch vụ và thay đổi ngân sách |

### Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Lan, sinh viên dùng tài khoản ngân hàng và ví điện tử để theo dõi chi tiêu cá nhân. |
| **Workflow** | Lan thanh toán, hệ thống đọc notification hoặc sao kê, rule trích xuất field và xử lý merchant đã biết, AI đề xuất category cho case mơ hồ, Lan duyệt phần confidence thấp và dashboard cập nhật dữ liệu. |
| **Bottleneck** | Nhập và phân loại thủ công sau mỗi giao dịch khiến dữ liệu bị thiếu, đặc biệt với khoản nhỏ hoặc giao dịch phát sinh khi người dùng đang bận. |
| **Impact** | Dữ liệu thiếu làm báo cáo chi tiêu và cảnh báo ngân sách kém tin cậy, đồng thời người dùng mất thời gian kiểm tra lại cuối ngày hoặc cuối tháng. |
| **Success Metric** | Trên cùng mẫu 10-20 giao dịch, giảm ít nhất 50% thời gian xử lý, ghi nhận ít nhất 90% giao dịch và đạt ít nhất 85% gợi ý category đúng trước khi sửa, so với nhãn cuối do người dùng xác nhận. |
| **Boundary** | Chỉ đọc dữ liệu sau khi người dùng cho phép; không tự thực hiện giao dịch, chuyển tiền, hủy subscription hoặc thay đổi ngân sách; giao dịch tiền mặt và notification không đọc được phải đi qua import hoặc nhập thủ công. |
| **AI intervention point** | Sau bước rule trích xuất field và trước bước người dùng xác nhận category cho giao dịch mơ hồ. |
| **Mức chọn** | Workflow với Rule cho case rõ và AI suggestion cho case mơ hồ. |
| **Rủi ro và người thật kiểm tra** | Rủi ro gồm merchant ambiguity, duplicate transaction, privacy và classification error. Người dùng kiểm tra confidence thấp, còn nhóm audit mẫu giao dịch và log lỗi trước khi mở rộng pilot. |

### Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú |
|---|---|---|
| Actor và workflow đã rõ chưa? | Yes | Actor là Lan và workflow bắt đầu sau mỗi giao dịch |
| Baseline và success metric đã đo được chưa? | Not Yet | Baseline 3 phút/giao dịch và 5-15 phút/ngày là từ card cá nhân, cần đo lại bằng log |
| Có data/input đủ dùng chưa? | Not Yet | Cần dùng dữ liệu transaction đã ẩn danh hoặc file sao kê có consent |
| Nếu AI sai, hậu quả có chấp nhận được không? | Yes, có điều kiện | AI chỉ đề xuất, người dùng duyệt và không có action tài chính tự động |
| Có người review/owner vận hành không? | Yes | Người dùng review confidence thấp và nhóm kiểm tra mẫu |
| Có cách non-AI đơn giản hơn không? | Yes | Import sao kê và merchant rule giải quyết một phần lớn case rõ |

**Decision:**

```text
Go cho pilot nhỏ có human review; chưa Go triển khai thực tế.
```

**Lý do:**

- Problem có actor, workflow và bottleneck rõ.
- Pain xuất hiện nhất quán trong các card của cả bốn thành viên.
- Có non-AI baseline mạnh nên nhóm không cần xây Agent để chứng minh giá trị.
- Workflow có thể pilot bằng dữ liệu ẩn danh và human review.
- Rủi ro tài chính được giới hạn vì hệ thống không tự chuyển tiền, hủy dịch vụ hoặc thay đổi ngân sách.

**Pilot nhỏ nhất:**

1. Chuẩn bị 10-20 giao dịch điện tử mẫu đã ẩn thông tin nhạy cảm.
2. Chia category thành 6-8 nhóm cố định.
3. Chạy merchant rule trước.
4. Dùng AI chỉ cho giao dịch rule không xác định.
5. Người dùng review toàn bộ prediction và ghi lại sửa đổi.
6. Đo capture rate, classification accuracy, thời gian review và failure category.

**Exit / rollback:**

- Nếu capture rate dưới 90% hoặc classification accuracy trước khi sửa dưới 85% trên mẫu review, quay về import sao kê và merchant rule.
- Nếu có duplicate transaction hoặc đọc sai dữ liệu nhạy cảm, dừng AI suggestion và chỉ giữ pipeline thủ công.
- Nếu người dùng không muốn cấp dữ liệu, không triển khai kết nối tự động và chuyển sang file import.

*Các baseline chưa được đo được ghi rõ là giả định; nhóm không dùng chúng như số liệu nghiên cứu đã xác nhận.*