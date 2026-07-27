## Tôi đã tham gia vào phần nào?

|Hoạt động|Tôi đã làm gì?|Kết quả / ảnh hưởng|
|---|---|---|
|Scan cá nhân|Tôi scan các vấn đề liên quan đến nhập giao dịch từ nhiều nguồn, cảnh báo vượt ngân sách quá muộn và phát hiện giao dịch bất thường hoặc subscription lãng phí. Tôi cố gắng mô tả actor, workflow và metric thay vì chỉ nêu ý tưởng tính năng.|Ba problem của tôi bao phủ cả bottleneck đầu nguồn, hệ quả về ngân sách và rủi ro từ giao dịch bất thường. Trong đó, bài toán nhập và phân loại giao dịch được đưa vào cluster chính của nhóm.|
|Pitch Problem Card|Tôi pitch ba Problem Cards: nhập và phân loại giao dịch từ nhiều nguồn; cảnh báo vượt ngân sách quá muộn; phát hiện giao dịch bất thường và đăng ký lãng phí. Tôi nhấn mạnh current workflow, bottleneck và human boundary.|Nhóm thấy rõ rằng các bài toán cảnh báo ngân sách và phát hiện bất thường đều phụ thuộc vào dữ liệu giao dịch đầy đủ. Điều này góp phần đưa transaction classification thành candidate ưu tiên.|
|Challenge bài của bạn khác|Tôi đặt câu hỏi về việc nhóm có đang chọn Agent quá sớm, dữ liệu đầu vào có đủ sạch không, Rule có thể giải quyết bao nhiêu phần và AI sai thì ai chịu trách nhiệm kiểm tra.|Các challenge giúp nhóm không tiếp tục với hướng “AI quản lý tài chính toàn năng”, mà thu hẹp về một workflow cố định có Rule, AI suggestion và human review.|
|Gom trùng / cluster|Tôi tham gia đối chiếu các candidate có nội dung gần nhau, đặc biệt là nhóm nhập và phân loại giao dịch, nhóm cảnh báo ngân sách và nhóm giao dịch bất thường.|Nhóm gom 12 candidates thành bốn cluster, giảm trùng lặp và nhìn được chuỗi nguyên nhân từ dữ liệu giao dịch thiếu đến báo cáo và cảnh báo kém tin cậy.|
|Chọn candidate problem|Tôi ủng hộ chọn ghi nhận và phân loại giao dịch cá nhân vì đây là bottleneck đầu nguồn. Tôi cũng phản biện rằng classification không phải mục tiêu cuối, nên cần chứng minh nó tạo nền tảng cho các outcome tiếp theo.|Nhóm chọn candidate có tổng điểm cao nhất là ghi nhận và phân loại giao dịch cá nhân, nhưng không phóng đại classification như một mục tiêu tài chính cuối cùng.|
|Validation / research|Tôi tham gia kiểm tra chéo các Problem Cards, so sánh baseline, non-AI alternatives và các giả định chưa được xác thực. Tôi phân biệt rõ evidence nội bộ với số liệu chỉ mới là ước lượng.|Nhóm ghi rõ các con số 3 phút/giao dịch và 5–15 phút/ngày là giả định cần đo lại, đồng thời xác định các giả định về consent, capture rate và classification accuracy cần kiểm chứng trong pilot.|
|Workflow nhóm|Tôi tham gia vẽ current workflow và future workflow, đặc biệt là xác định bước nghẽn, điểm AI can thiệp, confidence threshold, human review và fallback.|Future workflow được thu hẹp thành notification/import → parser → merchant rule → AI cho case mơ hồ → người dùng xác nhận → cập nhật báo cáo.|
|Problem Statement|Tôi góp ý để Problem Statement có actor cụ thể, workflow quan sát được, metric đo trên cùng một tập giao dịch và boundary rõ.|Problem Statement v1 có actor là Lan, metric giảm ít nhất 50% thời gian, capture rate 90%, accuracy 85% và giới hạn không tự thực hiện hành động tài chính.|
|Rule / Workflow / Agent|Tôi phản biện việc chọn Agent và đề xuất tách case rõ cho Rule, case mơ hồ cho AI, còn người dùng giữ quyền xác nhận cuối.|Nhóm chọn Workflow có Rule và AI hỗ trợ một bước, không chọn Agent. Điều này làm solution phù hợp hơn với độ phức tạp và mức rủi ro của bài toán.|
|Decision|Tôi tham gia đánh giá Go / Not Yet / No-Go dựa trên actor, metric, dữ liệu, failure handling và non-AI baseline.|Nhóm quyết định Go cho pilot nhỏ có human review, nhưng chưa Go triển khai thực tế vì baseline và dữ liệu vẫn chưa được kiểm chứng.|

## Bảng dùng AI trong reflection

|Phase|Tôi dùng AI để làm gì?|AI hữu ích ở đâu?|AI sai/hời hợt ở đâu?|Tôi sửa gì bằng nhận định của mình?|
|---|---|---|---|---|
|Scan|Tôi dùng AI để mở rộng danh sách problem theo các lăng kính lặp lại, tốn thời gian, AI có thể hỗ trợ và pain từ người khác.|AI giúp tôi tách một chủ đề rộng là “quản lý chi tiêu” thành các problem cụ thể như nhập giao dịch, cảnh báo muộn và phát hiện khoản bất thường.|Một số gợi ý ban đầu quá rộng, giống danh sách tính năng của một ứng dụng tài chính toàn năng và chưa có evidence thật.|Tôi loại bỏ các ý như tự động đầu tư, tự thay đổi ngân sách hoặc xây trợ lý tài chính toàn năng; chỉ giữ các pain có workflow quan sát được.|
|Problem Card|Tôi dùng AI để cấu trúc problem theo actor, workflow, bottleneck, impact, metric, non-AI alternative và AI hypothesis.|AI giúp tôi không bỏ sót field và diễn đạt workflow theo trình tự rõ ràng.|AI có xu hướng đưa metric nghe hợp lý nhưng chưa có dữ liệu kiểm chứng, ví dụ tỷ lệ giảm vượt ngân sách hoặc độ chính xác dự kiến.|Tôi ghi rõ các con số chỉ là mục tiêu hoặc giả định, không trình bày như bằng chứng đã đo.|
|Workflow|Tôi dùng AI để gợi ý current state, future state, fallback và human boundary.|AI hữu ích khi biến problem thành chuỗi bước và chỉ ra điểm nào có thể dùng Rule, AI hoặc người thật.|AI ban đầu dễ tự động hóa quá nhiều bước và giả định hệ thống có thể đọc mọi nguồn giao dịch.|Tôi thu hẹp phạm vi vào notification hoặc file import có consent, đưa giao dịch confidence thấp cho người dùng duyệt và giữ nhập thủ công làm fallback.|
|Research|Tôi dùng AI để gợi ý tiêu chí so sánh các giải pháp hiện có và những giả định cần kiểm tra.|AI giúp nhóm nhìn ra rằng import, merchant rule và category editing đã là baseline mạnh.|AI không thể thay thế evidence thực tế từ interview, log hoặc thử nghiệm với dữ liệu giao dịch.|Tôi phân biệt rõ research takeaway, evidence từ Problem Cards và giả định cần validation tiếp.|
|Problem Statement|Tôi dùng AI để kiểm tra Problem Statement có đủ actor, workflow, bottleneck, impact, metric và boundary hay chưa.|AI giúp phát hiện các câu còn solution-first hoặc quá rộng.|AI có thể làm câu văn trông đầy đủ nhưng actor vẫn chung chung hoặc impact quá xa so với workflow được chọn.|Tôi cùng nhóm cụ thể hóa actor thành Lan và giữ claim chính ở giảm ma sát nhập, phân loại giao dịch thay vì khẳng định trực tiếp sẽ giúp người dùng tiết kiệm tiền.|
|Rule / Workflow / Agent|Tôi dùng AI để so sánh các mức can thiệp và thử đặt câu hỏi phản biện về Agent.|AI giúp mô tả sự khác nhau giữa Rule, Workflow và Agent, đồng thời gợi ý decision tree.|AI đôi khi đánh đồng “có AI” với “cần Agent”, hoặc đề xuất hệ thống tự hành động quá mức.|Tôi phản biện rằng workflow khá cố định, không cần tự lập kế hoạch; AI chỉ nên xử lý case mơ hồ và không được thực hiện hành động tài chính.|
|Decision|Tôi dùng AI để rà lại tiêu chí Go, Not Yet và No-Go, cũng như gợi ý pilot và rollback.|AI giúp nhóm xây một pilot nhỏ có metric, failure category và exit condition.|AI có thể đưa ra quyết định Go quá nhanh dựa trên giả định chưa đo.|Tôi giữ quyết định ở mức “Go cho pilot nhỏ có human review; chưa Go triển khai thực tế” và yêu cầu đo lại baseline trước khi mở rộng.|

## Reflection câu hỏi mở

### Tôi học được gì khi nghe top 3 problems của các bạn khác?

Khi nghe top 3 problems của các bạn khác, tôi nhận ra cả nhóm đang nhìn cùng một chuỗi vấn đề nhưng bắt đầu ở những điểm khác nhau. Có bạn tập trung vào thao tác nhập và phân loại, có bạn tập trung vào cảnh báo vượt ngân sách, có bạn chú ý đến subscription, chi tiêu chung hoặc spending insight.

Điều tôi học được là các problem này không hoàn toàn độc lập. Ghi nhận và phân loại giao dịch là đầu vào; cảnh báo ngân sách, phát hiện bất thường và insight là các bước sử dụng dữ liệu phía sau. Việc nhìn theo chuỗi nguyên nhân giúp nhóm tránh chọn một solution lớn bao phủ mọi thứ và xác định được bottleneck nào nên giải quyết trước.

Tôi cũng học được rằng một ý tưởng nghe có impact lớn chưa chắc là candidate phù hợp nhất cho pilot. Overspending Detection gần với mục tiêu cuối của người dùng hơn, nhưng khó đánh giá vì còn phụ thuộc hành vi sau cảnh báo. Ngược lại, transaction classification có workflow hẹp hơn, dễ đo và có thể thử nghiệm trong thời gian ngắn.

### Nhóm có lúc nào bị solution-first không?

Có. Ở giai đoạn đầu, nhóm có xu hướng mô tả một hệ thống đọc notification, tự phân loại, dự báo vượt ngân sách, phát hiện giao dịch bất thường, sinh insight và thậm chí tự đề xuất hành động. Cách mô tả này gần với một ứng dụng tài chính AI toàn năng hơn là một problem cụ thể.

Ngoài ra, khi nhắc đến việc hệ thống tự đọc nhiều nguồn và học từ phản hồi, nhóm có lúc nghiêng về Agent trước khi chứng minh rằng workflow thật sự cần khả năng tự lập kế hoạch hay tự quyết định bước tiếp theo.

Nhóm thoát khỏi solution-first bằng cách quay lại current workflow, xác định bước nghẽn là nhập và chọn category, sau đó so sánh No AI, Rule, Workflow và Agent. Kết quả là phần lớn case rõ được giao cho Rule, AI chỉ xử lý case mơ hồ và người dùng quyết định category cuối.

### Tôi có thay đổi ý kiến sau khi bị challenge không?

Có. Ban đầu tôi đánh giá cao các bài toán cảnh báo vượt ngân sách và phát hiện giao dịch bất thường vì chúng có impact tài chính rõ hơn đối với người dùng. Tuy nhiên, sau khi nhóm challenge về dữ liệu đầu vào, độ chính xác và khả năng đo outcome, tôi đồng ý rằng transaction classification phù hợp hơn để làm candidate chính.

Tôi cũng thay đổi cách nhìn về AI intervention. Ban đầu có thể mô tả AI như thành phần tự phân loại gần như toàn bộ giao dịch. Sau phản biện, tôi thấy merchant rule và parser có thể xử lý nhiều trường hợp ổn định tốt hơn, rẻ hơn và dễ kiểm soát hơn. AI chỉ thực sự cần thiết ở những giao dịch có merchant mơ hồ hoặc phụ thuộc context cá nhân.

Tuy vậy, tôi vẫn giữ quan điểm rằng classification chỉ là phương tiện chứ không phải mục tiêu cuối. Vì thế metric pilot nên đo trực tiếp thời gian, capture rate và accuracy; còn tác động đến vượt ngân sách chỉ nên được xem là giả thuyết cần kiểm chứng ở giai đoạn sau.

### Tôi đóng góp gì thật sự vào artifact cuối?

Đóng góp rõ nhất của tôi là vai trò phản biện và điều phối mạch lập luận. Tôi thường xuyên đặt lại câu hỏi actor có đủ cụ thể chưa, bottleneck có quan sát được không, Rule đã đủ chưa, AI sai thì ai sửa và nhóm có đang chọn Agent quá sớm không.

Tôi cũng đóng góp vào việc nối các artifact thành một chuỗi logic:

```text
Dữ liệu giao dịch thiếu
→ Báo cáo và cảnh báo không đáng tin
→ Bottleneck đầu nguồn là nhập và phân loại
→ Merchant rõ dùng Rule
→ Case mơ hồ dùng AI suggestion
→ Người dùng review confidence thấp
→ Pilot đo thời gian, capture rate và accuracy
```

Ngoài ra, tôi góp phần làm rõ human boundary và failure handling. Hệ thống không được tự chuyển tiền, hủy subscription hoặc thay đổi ngân sách. Người dùng vẫn là owner của dữ liệu, category cuối và mọi hành động tài chính.

### Điều khó nhất khi viết Problem Statement là gì?

Điều khó nhất là giữ Problem Statement tập trung vào problem nhưng vẫn đủ cụ thể để dẫn đến một workflow có thể thử nghiệm.

Nếu viết quá rộng như “người dùng không kiểm soát được chi tiêu”, nhóm không xác định được bước nghẽn cụ thể, data cần dùng hay metric cần đo. Nếu viết quá gần solution như “cần AI đọc notification và phân loại giao dịch”, nhóm đã mặc định công nghệ trước khi so sánh các phương án đơn giản hơn.

Một khó khăn khác là chọn impact phù hợp. Việc giảm vượt ngân sách và tăng tiền tiết kiệm có ý nghĩa với người dùng, nhưng quá xa so với bước classification và chịu ảnh hưởng bởi nhiều yếu tố khác. Vì vậy, nhóm phải tách metric trực tiếp của pilot là thời gian xử lý, capture rate và accuracy khỏi outcome dài hạn về ngân sách.

Boundary cũng là phần khó vì dữ liệu giao dịch nhạy cảm. Problem Statement không chỉ cần nói hệ thống làm gì mà còn phải nói rõ hệ thống không được làm gì, dữ liệu nào được phép đọc và người thật kiểm tra ở đâu.

### Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn về evidence và baseline ngay từ đầu. Nhiều con số như 3 phút mỗi giao dịch, 5–15 phút mỗi ngày, capture rate 90% hoặc accuracy 85% nghe hợp lý nhưng chưa được đo. Tôi sẽ đề nghị cả nhóm bấm giờ một tác vụ thật trên cùng một mẫu giao dịch trước khi scoring candidate.

Tôi cũng sẽ challenge mạnh hơn về định nghĩa category đúng. Một merchant có thể thuộc nhiều category tùy mục đích mua, nên “accuracy” không thể chỉ so với một nhãn do AI hoặc nhóm tự đặt. Nhóm cần một rubric rõ và xem nhãn cuối do chính người dùng xác nhận là ground truth trong pilot.

Ngoài ra, tôi sẽ yêu cầu tách rõ ba failure mode:
1. Không lấy được giao dịch.
2. Trích xuất sai số tiền, thời gian hoặc merchant.
3. Trích xuất đúng nhưng phân loại sai category.

Ba lỗi này có nguyên nhân và cách rollback khác nhau. Nếu gộp chung thành “AI phân loại sai”, nhóm sẽ khó biết cần sửa parser, Rule, prompt hay thiết kế review.

Cuối cùng, tôi sẽ challenge thêm về privacy và consent. Việc người dùng có sẵn sàng cho phép đọc notification hoặc tải sao kê không phải chi tiết triển khai, mà có thể quyết định toàn bộ tính khả thi của workflow.

## Reflection tổng hợp

Trong bài lab này, tôi tham gia chủ yếu với vai trò phản biện và điều phối. Tôi bắt đầu từ ba vấn đề cá nhân gồm nhập và phân loại giao dịch từ nhiều nguồn, cảnh báo vượt ngân sách quá muộn và phát hiện giao dịch bất thường hoặc subscription lãng phí. Khi pitch, tôi cố gắng trình bày từng problem thông qua actor, current workflow, bottleneck, impact và metric thay vì mô tả trực tiếp một sản phẩm.

Khi làm việc nhóm, điều quan trọng nhất tôi đóng góp là giúp nhóm quay lại problem mỗi khi thảo luận bắt đầu nghiêng sang solution. Các candidate của nhóm có nhiều điểm trùng nhau và có nguy cơ bị gộp thành một ứng dụng tài chính AI toàn năng. Qua quá trình cluster và challenge, nhóm nhận ra ghi nhận và phân loại giao dịch là bottleneck đầu nguồn. Nếu dữ liệu này thiếu hoặc sai, các chức năng phía sau như cảnh báo ngân sách, phát hiện bất thường và spending insight đều khó đáng tin.

Tôi đã thay đổi quan điểm sau khi nghe phản biện. Ban đầu tôi cho rằng overspending alert hoặc anomaly detection có impact rõ hơn. Tuy nhiên, các bài toán đó cần dữ liệu lịch sử đủ sạch và có outcome khó đo trong một pilot ngắn. Transaction classification tuy không phải mục tiêu cuối nhưng có workflow rõ, baseline có thể đo và có thể so sánh trực tiếp No AI, Rule, Workflow và Agent.

Một bài học lớn của tôi là không phải bước nào có xử lý ngôn ngữ hoặc dữ liệu cũng cần Agent. Với bài này, parser và merchant rule có thể xử lý các trường hợp rõ. AI chỉ cần hỗ trợ khi mô tả giao dịch mơ hồ hoặc cần context từ lịch sử chỉnh sửa. Workflow không có nhu cầu tự lập kế hoạch hoặc tự thực hiện hành động tài chính, nên Agent vừa dư thừa vừa làm tăng rủi ro.

Tôi cũng hiểu rõ hơn vai trò của human boundary. Người dùng không chỉ là người sửa lỗi sau cùng mà phải là owner của quyền cấp dữ liệu, category cuối và mọi hành động tài chính. AI cần nêu confidence, đưa case chưa chắc chắn vào hàng chờ và cho phép người dùng sửa, bỏ qua hoặc reset preference.

Điểm tôi chưa hài lòng là evidence hiện tại chủ yếu đến từ cross-review nội bộ. Nhóm chưa có interview, log hoặc phiên bấm giờ chung. Vì vậy, các baseline và threshold vẫn là giả định. Quyết định “Go cho pilot nhỏ có human review; chưa Go triển khai thực tế” là hợp lý vì nó cho phép nhóm kiểm chứng giá trị mà không phóng đại mức độ sẵn sàng của solution.

Nếu làm lại, tôi sẽ yêu cầu đo current workflow sớm hơn, định nghĩa rubric cho category rõ hơn và tách riêng lỗi capture, parsing và classification. Tôi cũng sẽ challenge privacy và consent như một giả định cốt lõi thay vì coi đó chỉ là rủi ro triển khai.

Sau bài này, tôi có thể tự giải thích được mạch lập luận của nhóm:

```text
Problem:
Người dùng trì hoãn nhập và phân loại giao dịch.

Workflow:
Thanh toán → nhận notification → nhập lại → nhớ context → chọn category.

Metric:
Thời gian xử lý, capture rate và classification accuracy.

Boundary:
Chỉ dùng dữ liệu có consent; người dùng review confidence thấp;
không có hành động tài chính tự động.

Mức AI:
Rule cho case rõ, AI suggestion cho case mơ hồ,
Workflow thay vì Agent.

Decision:
Go pilot nhỏ có human review, chưa Go triển khai thực tế.
```

## Tự kiểm cuối bài

-  [12đ cá nhân] Cá nhân có 5+ problems và top 3 Problem Cards.
-  [12đ cá nhân] Tôi đã pitch rõ và challenge nhóm đúng trọng tâm.
-  Nhóm có nhật ký hội tụ từ candidates về 1 bài.
-  [15đ nhóm] Nhóm có workflow trước/sau.
-  [20đ nhóm] Nhóm có Problem Statement v0/v1 với metric và boundary rõ.
-  [15đ nhóm] Nhóm có so sánh No AI / Rule / Workflow / Agent.
-  [10đ nhóm] Nhóm có Go / Not Yet / No-Go và lý do rõ.
-  [10đ cá nhân] Reflection cá nhân có nói rõ vai trò trong nhóm, cách dùng AI, điều học được và nếu làm lại sẽ đổi gì.
-  [6đ cá nhân] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp với AI.

Tự chấm 90/100