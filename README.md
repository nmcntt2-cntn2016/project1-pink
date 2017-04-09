# A Study in *PINK*

##  Thành viên 

`1612838` Vũ Lê Thế Anh

`1612842` Lê Thành Công

`1612849` Nguyễn Lê Hồng Hạnh

`1612869` Trần Mai Khiêm

`1612891` Phan Quốc Thắng

##  Ý tưởng: Hệ thống Tự động Điều khiển Đèn giao thông

### Website: https://vltanh.github.io/narubibi/
### Poster: https://vltanh.github.io/narubibi/images/NMCNTT2.png

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
