# A Study in *PINK*

##  Thành viên 

`1612838` Vũ Lê Thế Anh

`1612842` Lê Thành Công

`1612849` Nguyễn Lê Hồng Hạnh

`1612869` Trần Mai Khiêm

`1612891` Phan Quốc Thắng

##  Ý tưởng: Hệ thống Tự động Điều khiển Đèn giao thông

### Website: https://vltanh.github.io/narubibi/

###  Thực trạng

Chúng ta đã huy động nhiều nguồn lực cả về nhân lực và thiết bị để giảm bớt tình trạng kẹt xe. Tuy nhiên, hiện tượng này vẫn diễn ra.

###  Nội dung

Một giải pháp hoàn chỉnh nhưng đơn giản điều khiển các luồng phương tiện bằng cảm ứng từ thông qua các đèn tín hiệu sẵn có.

###  Đối tượng

Người tham gia giao thông, các nhà quy hoạch

###  Làm thế nào?

* Nhận diện lưu lượng xe: 
    - Các cuộn dây đặt dưới mặt đường thành các rãnh. Các cuộn dây này được lái bởi một bộ tao dao động (Colpitts Oscillator). Một vi điều khiển sẽ có nhiệm vụ đọc tần số này và thông quá đó, dựa trên tính chất vật lý của sự dao động và ảnh hưởng của phương tiện lưu thông (căn bản là các khối kim loại di chuyển) lên cuộn dây, có thể biết được mật độ phương tiện trên đường.
    
* Mô hình điều khiển
	
	![Mô hình](https://raw.githubusercontent.com/nmcntt2-cntn2016/project1-pink/master/Untitled%20Diagram.png "Mô hình")
    
	- Ở các nút ngã tư:
		+ Các nút này đọc tần số dao động từ cuộn dây và lưu trữ ngắn hạn để phân tích và gửi lên trung tâm.
		+ Khi hoạt động trong chế độ đơn (standalone), hệ thống sẽ thay đổi thời gian đèn đỏ xanh dựa trên lưu lượng: nhánh đông xe sẽ được ưu tiên đèn xanh lâu hơn.
		+ Khi hoạt động trong chế độ kết hợp (group), hệ thống sẽ nhận lệnh và chia thời gian theo sự sắp xếp của nút trung tâm.
	- Ở nút trung tâm:
		+ Nhận dữ liệu từ các nút ngã tư và thể hiện chúng.
		
### Lợi ích
* Giảm thiểu sự ùn tắc giao thông không đáng có. Từ đó giảm thiểu các tác hại do ùn tắc giao thông gây nên.
* Giảm chi phí cũng như về nhân lực.
* Các thông tin về lưu lượng cho phép đưa ra phân tích thích hợp, từ đó có một tầm nhìn đúng đắn cho hướng phát triển đô thị hóa trong khi vẫn điều tiết lưu lượng.

---------------------------------------------------------------------------------

##  Ý tưởng 1:

###  Thực trạng

Thay đổi kiểu tóc hiện nay là nhu cầu cần thiết của hầu hết mọi người, đặc biệt là phụ nữ. Tuy nhiên, trước khi bước vào tiệm cắt tóc, họ luôn phải đối mặt với câu hỏi, liệu thay đổi kiểu tóc này mình sẽ trông như thế nào. Để giải quyết vấn đề khó khăn đó, nhóm chúng tôi hướng đến nghiên cứu 1 phần mềm thay đổi kiểu tóc để giúp người dùng biết trước được dung mạo của mình.

###  Nội dung

Ứng dụng giúp người dùng thử trước các kiểu tóc từ một tấm hình tùy chọn theo ý thích hoặc dựa trên tư vấn từ các chuyên gia tạo mẫu tóc.

###  Đối tượng

Mọi cá nhân có nhu cầu thay đổi kiểu tóc
 
###  Làm thế nào?

- Xây dựng trên nền tảng Android/ iOS.
- Chức năng chính của ứng dụng:
 * ChangeYourself: cho phép bạn thử thay đổi kiểu tóc trên chính gương mặt mình, dựa trên một kiểu tóc mẫu.
     + Sử dụng một bức ảnh chụp gương mặt của bạn, bức ảnh này có thể là ảnh đã chụp từ trước (phải rõ ràng để ứng dụng có thể nhận diện được mặt và tóc, nếu ảnh lớn quá kích cỡ sẽ tự động crop về kích cỡ phù hợp) hoặc được chụp bằng camera điện thoại/iPad ngay lúc đó.
     
     + Kết hợp một hình ảnh khác, có kiểu tóc mà bạn muốn cắt, cũng được nhận diện gương mặt, mắt và tóc.
     
     + Cắt ghép, chỉnh sửa hình ảnh: phần mềm sẽ tự động ghép tóc mà bạn muốn cắt thay thế cho tóc của bạn
     
     + Đo độ phù hợp: phần mềm sẽ tự động tính toán xem tóc mới sau khi ghép có hợp với mặt bạn không (dựa vào các số liệu thông số về tỉ lệ khuôn mặt và tóc trong mỹ thuật)
          
   * ChatRoom: có vai trò như một phòng tư vấn online giữa chuyên gia làm tóc và người dùng
       + Người dùng/ chuyên gia làm tóc: tạo một tài khoản riêng, lưu thông tin.
       
       + Khi cần tư vấn về ý định muốn thay đổi kiểu tóc, họ sẽ đăng lên ChatRoom (như đăng stt fb); sau đó các chuyên gia vào bình luận, tư vấn và đưa hình các kiểu tóc mẫu.
       
        + Thấy kiểu tóc nào phù hợp, người dung có quyền lưu hình ảnh đó, và hình ảnh tự động đc lưu vào thiết bị di động/ ipad.
        
    * Sharing (chức năng phụ): chia sẻ hình ảnh cho bạn bè hoặc các trang mạng xã hội.
        + Lấy thông tin từ Mess và Fb để chia sẻ hình ảnh.
        
        + Lấy thông tin số điện thoại từ danh bạ đt để gửi hình ảnh qua tin nhắn.

##  Ý tưởng 2:

###  Thực trạng

Tình trạng kẹt xe ở Việt Nam hiện nay đang gây nhiều tranh cãi và đáng báo động. Tuy nhiên, kẹt xe không phải lúc nào cũng diễn ra ở hai làn đường. Do đó, chúng tôi hướng đến nghiên cứu hệ thống dịch chuyển dải phân cách, thông qua nhận diện lưu lượng xe, nhằm mở rộng làn đường đang kẹt để giảm áp lực và thu hẹp làn đường thông thoáng.

###  Nội dung

Dải phân cách tự động dời vị trí phù hợp lưu lượng xe lưu thông trên hai làn.

###  Đối tượng

Người tham gia giao thông, các nhà quy hoạch

###  Làm thế nào?

* Nhận diện lưu lượng xe: 
    - Ghi nhận hình ảnh thông qua camera đặt trên cột đèn giao thông, gửi hình ảnh thu được đến phần mềm để nhận diện tình trạng xe hiện tại trên đường.
    
    -  Phần mềm: có 3 chức năng chính:
         + Nhận diện kẹt xe bằng cách đo lưu lượng xe có trên đường kết hợp với tín hiệu đèn giao thông hiện tại.
         
         + Phân biệt với lúc xe dừng đèn đỏ và lúc kẹt xe: khi đèn đỏ và lưu lượng xe đông -> bỏ qua; khi đèn xanh và lưu lượng xe đông -> kẹt xe.
         
         + Khi xác định được kẹt xe, gửi tín hiệu đến thiết bị điều khiển để tự động dời dải phân cách.
          
* Thiết bị điều khiển:
   - Khi nhận được tín hiệu từ phần mềm, bật đèn báo hiệu sắp dời dải phân cách.
   - Di chuyển dải phân cách sau khi đã báo hiệu
   
##  Ý tưởng 3:

###  Thực trạng

Sau những giờ học tập và làm việc căng thẳng, mọi người thường muốn tụ tập nhóm bạn tổ chức các buổi đi chơi giải tỏa tinh thần. Các ứng dụng hiện tại cho phép tìm các địa điểm ăn uống, xem phim, nhưng chưa thực sự tạo được liên kết giữa chúng thành một kế hoạch cụ thể. Để lập thành một kế hoạch đi chơi đầy đủ, mọi người phải tìm kiếm địa điểm ăn uống rồi địa điểm giải trí từ nhiều nguồn. Điều này dẫn đến nhu cầu có một ứng dụng giúp tìm địa điểm, tổng kết và lập kế hoạch đi chơi phù hợp.

###  Nội dung

Ứng dụng giúp người dùng lập kế hoạch đi chơi phù hợp.

###  Đối tượng

Các nhóm bạn học sinh - sinh viên.

###  Làm thế nào?

* Thống kê các địa điểm vui chơi, ăn uống kết hợp với bản đồ thành phố.

* Lập kế hoạch đi chơi phù hợp:
 + Chọn địa điểm hẹn bắt đầu thuận tiện cho mọi thành viên trong nhóm.
 
 + Tìm các địa điểm ăn uống và vui chơi ở gần nhau và đáp ứng mong muốn của nhóm.
 
 + Tìm đường đi ngắn nhất và gửi hướng dẫn đến các thành viên trong nhóm.

## Ý tưởng 4:

### Thực trạng:

Sự phát triển của khoa học kĩ thuật ngày nay đã được ứng dụng vào nông nghiệp, cụ thể là ứng dụng điều khiển tự động trong nhà kính trồng rau sạch, tuy nhiên vẫn còn có sự can thiệp của con người ở khâu kiểm tra tình trạng rau xanh, hằng ngày người ta vẫn ra thăm vườn rau. Để ứng dụng điều khiển tự động được hoàn thiện hơn và đồng thời phát triển theo hướng vườn rau thông minh, nhóm chúng tôi đề xuất hướng nghiên cứu về thu thập tất cả dữ liệu từ các cảm biến nhiệt độ, độ ẩm và ánh sáng của vườn rau nhằm kiểm soát chặt chẽ tình trạng cây trồng, đồng thời chẩn đoán bệnh của rau ngay cả khi con người không có mặt ở vườn, thông qua truyền thông không dây đến máy tính hoặc điện thoại của người dùng. Có thể áp dụng trong trồng rau quy mô vừa và lớn, tiết kiệm tiền và sức người.

### Nội dung:

Ứng dụng giúp thu thập dữ liệu từ các cảm biến gắn vào từng loại cây trồng, giúp kiểm soát chặt chẽ tình trạng của từng cây, từng loại cây và đưa về trung tâm kiểm soát thông báo cho người dùng. Đồng thời ứng dụng giúp điều khiển tự động tưới nước và ánh sáng, chẩn đoán bệnh của cây trồng. Ứng dụng hướng đến một vườn rau tự động và thông minh.

### Đối tượng

- Người làm vườn
- Trồng rau tại gia
- Trồng rau quy mô vừa và lớn

### Làm thế nào

- Xây dựng chuẩn đoán bệnh bằng mạng neural network và đưa ra giải pháp, thuốc chữa bệnh trên Matlab. Tưới nước, chiếu sáng tự động và tối ưu sử dụng Fuzzy logic trên Matlab.
- Thu thập dữ liệu từ các cảm biển và truyền thông không dây và truyền về máy tính hoặc thiết bị di động và hiển thị trên màn hình các thông số của từng cây, từng loại cây, giúp người quản lý chặt chẽ tình hình vườn trong khi không có mặt ở đó. 
- Người dùng có thể điều khiển tưới nước, chiếu sáng hoặc có thể chuyển sang chế độ tự động hoàn toàn.
