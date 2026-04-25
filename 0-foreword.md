
## Lời nói đầu

Thật đáng kinh ngạc, và cũng khá đáng lo, khi nhận ra rằng **chúng ta đang chạy rất nhiều phần mềm mà hoàn toàn không biết chắc nó thực sự làm gì. **
Chúng ta mua phần mềm trong các hộp đóng gói sẵn trên kệ, được bọc nhựa kín. 
Chúng ta chạy các chương trình cài đặt, chúng cài vô số tệp, thay đổi thiết lập hệ thống, xóa hoặc vô hiệu hóa các phiên bản cũ và tiện ích lỗi thời, đồng thời chỉnh sửa những phần quan trọng trong registry. 

Mỗi lần truy cập một trang web, có thể chúng ta đang gọi hoặc tương tác với hàng chục chương trình và đoạn mã, tất cả nhằm tạo ra giao diện, cảm giác và hành vi sử dụng như mong đợi. 
Chúng ta mua các đĩa CD chứa hàng trăm trò chơi và tiện ích, hoặc tải phần mềm về dưới dạng dùng thử; rồi chia sẻ các chương trình đó với đồng nghiệp, bạn bè, dù mới chỉ dùng một phần rất nhỏ tính năng. 
Chúng ta tải bản cập nhật, cài đặt các bản vá, và tin rằng nhà cung cấp đã kiểm tra đầy đủ, mọi thay đổi đều chính xác và trọn vẹn. 
Chúng ta gần như “nhắm mắt tin” rằng các thay đổi mới nhất sẽ vẫn tương thích với mọi chương trình còn lại trong hệ thống. 
Nói ngắn gọn, chúng ta đang phụ thuộc vào rất nhiều phần mềm mà chính mình không hiểu rõ. 

Tôi không chỉ nói tới máy tính để bàn hay laptop cá nhân. 
Khái niệm ubiquitous computing (tính toán mọi nơi) – hay software everywhere (phần mềm ở mọi chỗ)– đang nhanh chóng đưa phần mềm điều khiển và kết nối vào vô số thiết bị xung quanh ta. 
Một chiếc ô tô trung bình ngày nay có số dòng mã trong hệ thống điều khiển động cơ còn nhiều hơn số dòng mã từng cần để đưa phi hành gia Apollo lên Mặt Trăng. 

**Phần mềm hiện đại đã trở nên phức tạp và liên kết chằng chịt** đến mức ngay cả nhà phát triển cũng thường không nắm hết tất cả tính năng và mọi hệ quả trong ứng dụng của họ. 
Việc kiểm thử mọi nhánh điều khiển của chương trình và mọi tổ hợp tùy chọn người dùng thường quá tốn kém và mất thời gian. 
Với nhiều tầng kiến trúc khác nhau và vô số nền tảng kết nối mạng mà phần mềm phải chạy trên đó hoặc tương tác, việc kiểm tra mọi kết hợp khả dĩ gần như bất khả thi. 
Giống như việc rất khó dự đoán trước mọi tương tác giữa các loại thuốc trị bệnh, nhiều hệ thống phần mềm được tung ra sử dụng trong khi vẫn tồn tại những vấn đề chưa được biết tới và khó lường. 

**Reverse engineering (dịch ngược)** là tập hợp các kỹ thuật và công cụ then chốt để hiểu phần mềm thực sự là gì và hoạt động ra sao. 
Về chính danh, nó là “quá trình phân tích một hệ thống đối tượng nhằm xác định các thành phần của hệ thống, mối quan hệ giữa chúng, và tạo ra các biểu diễn của hệ thống đó dưới một hình thức khác hoặc ở mức trừu tượng cao hơn” (IEEE 1990). 
Nhờ đó, chúng ta có thể hình dung được cấu trúc phần mềm, cách nó vận hành, và những tính năng điều khiển hành vi của nó. 
Các kỹ thuật phân tích, cùng việc áp dụng những công cụ tự động để kiểm tra phần mềm, đem lại cho chúng ta một cách tiếp cận hợp lý để nắm bắt độ phức tạp của phần mềm và khám phá bản chất thật bên trong. 

Reverse engineering đã xuất hiện từ lâu. 
Về mặt ý niệm, quá trình “reversing” diễn ra mỗi khi ai đó xem xét mã nguồn của người khác. 
Nó cũng xảy ra khi một lập trình viên nhìn lại mã của chính mình sau vài ngày hoặc lâu hơn. 
Reverse engineering là một quá trình khám phá: khi nhìn lại mã nguồn với con mắt mới – dù là mã của mình hay người khác – ta xem xét, học hỏi và nhận ra những điều trước đây có thể không ngờ tới. 

Dù chủ đề này từng xuất hiện ở một vài phiên trong các hội nghị và nhóm người dùng máy tính, nhưng reverse engineering phần mềm thực sự bước vào giai đoạn “trưởng thành” vào năm 1990. 
Nó được cộng đồng kỹ sư ghi nhận thông qua một bài báo phân loại về reverse engineering và khái niệm “phục hồi thiết kế” đăng trên tạp chí IEEE Software. 
Kể từ đó, đã có một khối lượng nghiên cứu rộng lớn và ngày càng tăng về các kỹ thuật reversing, trực quan hóa phần mềm, hiểu chương trình, reverse dữ liệu, phân tích phần mềm và các công cụ, phương pháp liên quan. 
Những diễn đàn nghiên cứu như hội nghị quốc tế thường niên Working Conference on Reverse Engineering (WCRE) đã và đang khám phá, nhấn mạnh, mở rộng giá trị của các kỹ thuật hiện có. 
Hiện nay, **sự quan tâm đến reverse ở mức nhị phân – trọng tâm chính của cuốn sách này** – đang tăng lên, nhằm hỗ trợ chuyển đổi nền tảng, khả năng tương tác, phát hiện malware và chẩn đoán lỗi. 

Là một tư vấn viên về quản lý và công nghệ thông tin, tôi thường được hỏi: “Làm sao anh có thể ủng hộ reverse engineering được?”. 
Tiếp theo là câu hỏi: “Anh từng phát triển và bán phần mềm. Anh không muốn người khác tôn trọng và bảo vệ bản quyền, tài sản trí tuệ của anh sao?”. 
Những cuộc tranh luận như vậy thường bắt nguồn từ sắc thái tiêu cực gán cho cụm từ “reverse engineering”, đặc biệt trong các thỏa thuận giấy phép phần mềm. 
Tuy vậy, công nghệ reverse engineering lại mang nhiều giá trị cho cả nhà sản xuất lẫn người dùng phần mềm trong toàn bộ chuỗi cung ứng. 

Một chiếc ống nghe có thể bị kẻ trộm dùng để nghe cơ chế khóa của két sắt khi các bánh bi rơi vào vị trí. 
Nhưng cũng chính chiếc ống nghe đó được bác sĩ gia đình dùng để phát hiện những vấn đề về hô hấp hoặc tim mạch. 
Hoặc nó có thể được kỹ thuật viên máy tính dùng để lắng nghe kỹ tiếng hoạt động của một ổ đĩa cứng kín nhằm chẩn đoán sự cố mà không cần mở ổ đĩa, tránh cho nó tiếp xúc với bụi và phấn hoa có thể gây hỏng hóc. 
**Bản thân công cụ không tự nó tốt hay xấu; vấn đề nằm ở cách nó được sử dụng. **

Vào đầu những năm 1980, IBM quyết định không còn cung cấp mã nguồn hệ điều hành máy tính lớn cho khách hàng. 
Trước đó, khách hàng mainframe luôn dựa vào mã nguồn để tham khảo khi giải quyết sự cố, cũng như để tùy chỉnh, chỉnh sửa, mở rộng sản phẩm hệ điều hành của IBM. 
Tôi vẫn giữ một chiếc huy hiệu của nhóm người dùng IBM Share với dòng chữ: “*Nếu SOURCE bị coi là bất hợp pháp, thì chỉ có ‘tội phạm’ mới có SOURCE”* – chơi chữ dựa trên khẩu hiệu nổi tiếng của những người phản đối luật kiểm soát súng. 
Áp dụng vào phần mềm ngày nay, điều này cho thấy các hacker và tác giả mã độc biết rất nhiều kỹ thuật để giải mã phần mềm của người khác. 
Vì vậy, thật hữu ích nếu “người tốt” cũng biết và sử dụng các kỹ thuật này. 

**Reverse engineering đặc biệt hữu ích trong phân tích phần mềm hiện đại, với nhiều mục đích:** 

– Tìm kiếm mã độc. 
Nhiều kỹ thuật phát hiện virus và malware dùng reverse engineering để hiểu cấu trúc và cách hoạt động của mã độc hại. 
Thông qua reversing, ta nhận ra những mẫu đặc trưng có thể dùng làm “chữ ký” cho các bộ phát hiện và quét mã độc hiệu quả, chi phí thấp. 

– Phát hiện lỗi và lỗ hổng bất ngờ. 
Ngay cả hệ thống được thiết kế tốt cũng có thể tồn tại lỗ hổng do bản chất của cách chúng ta làm “forward engineering”. 
Reverse engineering giúp nhận diện lỗi, lỗ hổng trước khi chúng trở thành các sự cố phần mềm nghiêm trọng, ảnh hưởng tới nhiệm vụ/hoạt động cốt lõi. 

– Xác định việc sử dụng mã của người khác. 
Để sử dụng tài sản trí tuệ một cách có trách nhiệm, ta cần biết mã được bảo hộ hoặc kỹ thuật được bảo vệ đang được dùng ở đâu trong ứng dụng. 
Reverse engineering có thể được dùng để phát hiện có hay không sự hiện diện của các thành phần phần mềm gây quan ngại. 

– Phát hiện việc sử dụng mã shareware hoặc mã nguồn mở không đúng chỗ. 
Ở chiều ngược lại với lo ngại bị xâm phạm bản quyền, nếu một sản phẩm hướng đến bảo mật cao hoặc tính độc quyền, sự xuất hiện của mã công khai có thể là vấn đề. 
Reverse engineering cho phép phát hiện các vấn đề sao chép mã như vậy. 

– Học hỏi từ sản phẩm của người khác trong những lĩnh vực hoặc mục đích khác. 
Các kỹ thuật reverse engineering cho phép nghiên cứu những cách tiếp cận phần mềm tiên tiến, giúp người học mới “mổ xẻ” sản phẩm của các bậc thầy. 
Đây là một cách rất hữu ích để học và xây dựng trên kho tri thức mã nguồn đang không ngừng lớn lên. 
Rất nhiều website được xây dựng bằng cách xem người khác đã làm gì; nhiều lập trình viên web đã học HTML và kỹ thuật lập trình web bằng cách xem source của các site khác. 

– Khám phá những tính năng hoặc cơ hội mà chính nhà phát triển ban đầu cũng không nhận ra. 
Độ phức tạp của mã có thể thúc đẩy đổi mới; các kỹ thuật hiện có có thể được tái sử dụng trong bối cảnh mới. 
Reverse engineering có thể dẫn tới những khám phá mới về phần mềm và tạo ra cơ hội mới cho đổi mới sáng tạo. 

(Tùy vào bản PDF của bạn, phần Foreword có thể tiếp tục thêm 1–2 đoạn nữa nói về vai trò của cuốn sách đối với người làm bảo mật, nhà phát triển, nhà quản lý; nếu bạn thấy còn đoạn nào chưa rõ, gửi ảnh/chụp text thêm để mình dịch nốt cho khớp.) 

***

## Tóm tắt và giải thích ngắn gọn

1. **Ngữ cảnh chung**  
   - Con người đang phụ thuộc vào vô số phần mềm mà không thật sự hiểu bên trong nó làm gì. 
   - Phần mềm ngày nay quá phức tạp, đa nền tảng, nên không thể test hết mọi trường hợp, luôn tiềm ẩn lỗi và hành vi khó đoán. 

2. **Reverse engineering là gì và để làm gì**  
   - Reverse engineering là quá trình phân tích một hệ thống để hiểu thành phần, quan hệ giữa chúng và dựng lại mô hình ở mức trừu tượng cao hơn. 
   - Nó giúp ta “nhìn xuyên” vào cấu trúc, cách hoạt động và các yếu tố điều khiển hành vi của phần mềm. 

3. **Reverse không chỉ dành cho hacker**  
   - Tác giả nhấn mạnh: công cụ tự nó không tốt hay xấu, giống như chiếc ống nghe – dùng được cho bác sĩ, kỹ thuật viên hoặc kẻ trộm két. 
   - Vấn đề là người dùng nó với mục đích gì: tấn công, bảo vệ, phân tích lỗi, hay học tập. 

4. **Lịch sử và nghiên cứu**  
   - Reverse engineering từng chỉ là chủ đề nhỏ trong cộng đồng, nhưng được “chính danh” khoảng năm 1990 qua các bài báo IEEE và hội nghị WCRE. 
   - Sau đó, có cả một mảng nghiên cứu lớn về reversing, program understanding, visualization, data reverse engineering, v.v. 

5. **Ứng dụng thực tế quan trọng**  
   - Phát hiện và phân tích malware, tạo chữ ký nhận diện. 
   - Tìm lỗi, lỗ hổng thiết kế trước khi chúng gây ra sự cố lớn. 
   - Kiểm tra vi phạm tài sản trí tuệ (dùng mã của người khác trái phép), hoặc ngược lại phát hiện mã nguồn mở ở nơi cần tính độc quyền. 
   - Học hỏi kỹ thuật từ phần mềm khác, giống cách dev web xem “View Source” để học HTML/CSS/JS. 

6. **Thông điệp chính cho người học reversing**  
   - Hacker và tác giả malware đã biết và dùng các kỹ thuật này từ lâu; nếu bạn đứng “phe phòng thủ”, bạn cũng cần nắm reversing để hiểu mình đang đối mặt với cái gì. 
   - Cuốn sách (và phần Foreword) muốn hợp thức hóa reverse engineering như một kỹ thuật chuyên môn quan trọng, chứ không phải hoạt động chỉ dành cho “người xấu”. 

