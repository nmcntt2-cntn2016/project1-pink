#  A Study in *PINK*

##Thành viên

(1612838) Vũ Lê Thế Anh

(1612849) Nguyễn Lê Hồng Hạnh

(1612869) Trần Mai Khiêm

(1612891) Phan Quốc Thắng

## Ý tưởng 1:

### Thực trạng

Thay đổi kiểu tóc hiện nay là nhu cầu cần thiết của hầu hết mọi người, đặc biệt là phụ nữ. Tuy nhiên, trước khi bước vào tiệm cắt tóc, họ luôn phải đối mặt với câu hỏi, liệu thay đổi kiểu tóc này mình sẽ trông như thế nào. Để giải quyết vấn đề khó khăn đó, nhóm chúng tôi hướng đến nghiên cứu 1 phần mềm thay đổi kiểu tóc để giúp người dùng biết trước được dung mạo của mình.

### Nội dung

Ứng dụng giúp người dùng thử trước các kiểu tóc từ một tấm hình tùy chọn theo ý thích hoặc dựa trên tư vấn từ các chuyên gia tạo mẫu tóc.

### Đối tượng

Mọi cá nhân có nhu cầu thay đổi kiểu tóc
 
### Làm thế nào?

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

## Ý tưởng 2:

### Thực trạng

Kẹt xe đang là vấn đề nhức nhối của giao thông Việt Nam. Thế nhưng, ức chế nhất vẫn là tình huống kẹt cứng trong làn xe của mình khi mà nhìn về bên kia đường, các xe chạy ngược chiều vẫn đang ung dung kéo ga lướt gió. Điều này dẫn đến nhu cầu có một hệ thống dải phân cách có thể tự động điều chỉnh nới rộng hay bó hẹp tùy vào lưu lượng xe hai làn.

### Nội dung

Dải phân cách tự động dời vị trí phù hợp lưu lượng xe lưu thông trên hai làn

### Đối tượng

Người tham gia giao thông, các nhà quy hoạch

### Làm thế nào?

* Nhận diện lưu lượng xe: 
    - Ghi nhận hình ảnh thông qua camera đặt trên cột đèn giao thông, gửi hình ảnh thu được đến phần mềm để nhận diện tình trạng xe hiện tại trên đường.
    
    -  Phần mềm: có 2 chức năng chính:
         + Nhận diện xem khi nào kẹt xe bang cách đo lưu lượng xe có trên đường kết hợp với tín hiệu đèn giao thông hiện tại.
         
         + Phân biệt với lúc xe dừng đèn đỏ và lúc kẹt xe: khi đèn đỏ và lưu lượng xe đông -> bỏ qua; khi đèn xanh và lưu lượng xe đông -> kẹt xe.
         
         + Khi xác định được kẹt xe, gửi tín hiệu đến thiết bị điều khiển để tự động dời dải phân cách.
          
* Thiết bị điều khiển:
         + Khi nhận được tín hiệu từ phần mềm, bật đèn báo hiệu sắp dời dải phân cách.

## Ý tưởng 3:

### Thực trạng

Sau những giờ học tập và làm việc căng thẳng, mọi người thường muốn tụ tập nhóm bạn tổ chức các buổi đi chơi giải tỏa tinh thần. Các ứng dụng hiện tại cho phép tìm các địa điểm ăn uống, xem phim, nhưng chưa thực sự tạo được liên kết giữa chúng thành một kế hoạch cụ thể. Để lập thành một kế hoạch đi chơi đầy đủ, mọi người phải tìm kiếm địa điểm ăn uống rồi địa điểm giải trí từ nhiều nguồn. Điều này dẫn đến nhu cầu có một ứng dụng giúp tìm địa điểm, tổng kết và lập kế hoạch đi chơi phù hợp.

### Nội dung

Ứng dụng giúp người dùng lập kế hoạch đi chơi phù hợp

### Đối tượng

Các nhóm bạn học sinh - sinh viên

### Làm thế nào?

* Thống kê các địa điểm vui chơi, ăn uống kết hợp với bản đồ thành phố

* Lập kế hoạch đi chơi phù hợp:
 + Chọn địa điểm hẹn bắt đầu thuận tiện cho mọi thành viên trong nhóm
 
 + Tìm các địa điểm ăn uống và vui chơi ở gần nhau và đáp ứng mong muốn của nhóm
 
 + Tìm đường đi ngắn nhất và gửi hướng dẫn đến các thành viên trong nhóm
