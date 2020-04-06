
# CCNA-Tutorials-Day1

## I. Các thành phần cơ bản của hệ thống mạng
###  Mạng là gì? 
- Các thiết bị được gọi là hệ thống mạng khi và chỉ khi đáp ứng được 2 yếu tố sau: 
  + Chúng được kết nối với nhau.
  + Chúng có khả năng truyền thông với nhau.
- VD: Hai máy tình được kết nối với nhau qua sợi cáp đồng FastEthernet, hai smartphone kết nối Bluetooth => Được gọi là hệ thống mạng.
- Một hệ thống mạng cơ bản bao gồm: Các thiết bị đầu cuối(Máy tính bảng, smartphone, laptop...), Switch, Router, môi trường mạng....
- 
'![alt](https://images.viblo.asia/2b600a47-f91b-47d7-abb0-ba0a114c5684.png)

## II. Các yếu tố cơ bản ảnh hưởng đến tốc độ của hệ thống mạng
###  Các yếu tố cơ bản  ảnh hưởng đến tốc độ của hệ thống mạng bao gồm: 
   #### Tốc độ(Speed): Bao gồm tốc độ bên trong hệ thống mạng và tốc độ bên ngoài hệ thống mạng.
 1.  Các yếu tố cơ bản  ảnh hưởng đến tốc độ bên trong hệ thống mạng: 
 -  Điều kiện đạt được tốc độ tối ưu nhất trong hệ thống mạng là:Tốc độ trên all thiết bị phải đồng nhất(bao gồm hệ thống mạng cap, thiết bị đầu cuối, các thiết bị Switch, Router)
 - Bên cạnh đó còn có yếu tố ảnh hưởng đến tốc độ bên trong hệ thống mạng đó là giới hạn về tài nguyên phần cứng trên server cụ thể là tốc độ đọc dữ liệu trên phần cứng của server, để khắc phục điều này ngta trang bị kĩ thuật Raid cho phép người dùng đọc dữ liệu trên đồng thời trên 4 ổ cứng của server => cải thiện đáng kể tốc độ đọc dữ liệu. 
 2.  Các yếu tố cơ bản  ảnh hưởng đến tốc độ bên ngoài hệ thống mạng: 
 - Một trong những yếu tố ảnh hưởng đến tốc độ của hệ thống mạng là chuẩn không dây bên ngoài hệ thống mạng cụ thể là tốc độ của access point(Wifi): 
		 + Nếu  access point hoạt động ở chuẩn 802.11 b/g thì tốc độ cơ bản cho Access point sẽ là 11Mbp.
		 +  Nếu  access point hoạt động ở chuẩn 802.11 b/a thì tốc độ cơ bản cho Access point sẽ là 54Mbp
		 + Nếu  access point hoạt động ở chuẩn 802.11 b/n thì tốc độ cơ bản cho Access point sẽ là 150Mbp.
		 + Nếu  access point hoạt động ở chuẩn 802.11 b/ac thì tốc độ cơ bản cho Access point sẽ là 1300Mbp.
- Một lưu ý khác cho tốc độ truyền dẫn cho hệ thống mạng là: Tốc độ truyền dẫn của mạng không dây sẽ không bao giờ bằng tốc độ truyền dẫn của mạng có dây do có sự chi sẻ băng thông trong quá trình nhiều thiết bị kết nối với nhau. 
- Nguyên nhân bị giới hạn băng thông của tốc độ từ bên ngoài hệ thống mạng vào bên trong hệ thống mạng là do sự giới hạn của từng phiên kết nối từ server trên internet(2Mbp/Connection). Để khắc phục điều này ngta sử dụng trình download file IDM cho phép người dùng mở đồng thời nhiều phiên kết nối tới server ngoài internet từ đó tốc độ load file có thể tăng lên đáng kể. 
  #### Chi phí(Cost)
  1. Chi phí triển khai ban đầu => chi phí tốn kém nhất
  2. Chi phí duy trì hạ tầng mạng
  3. Chi phí bảo dưỡng và  nâng cấp hệ thống mạng
  #### Tính bảo mật của hệ thống(Security): Có thể triển khai trên nhiều thiết bị và nhiều lớp: 
  - Đối với thiết bị đầu cuối: Sử dụng phần mềm diệt virus có uy tín và liên tục cập nhật chúng các bản vá mới nhật, thường xuyên cập nhật hệ điều hành....
  - Đối với các thiết bị như Switch, Router: Trang bị các thiết bị đầy đủ các tính năng bảo mật.
  
  #### Độ sẵn sàng(Availability)
  - Để đảm bảo độ sẵn sàng của hệ thống mạng kết nối đi internet ngta thường thuê 2 kết nối. Vd: Viettel & VNPT. 
  ####  Khả năng mở rộng hệ thống(Scalability)
  - Nên lựa chọn các thiết bị phù hợp với hệ thống  mạng của người dùng
  #### Độ tin cậy trong quá trình truyền thông(Reliability)
  - Để đảm bảo sự bảo mật trong  quá trình truyền thông ngta sẽ cấu hình server theo  chuẩn sFTP qua đó dữ liệu người dùng như Username, Password...sẽ được mã hóa nhanh chóng.

## III. Các loại mô hình Topology của hệ thống mạng
### Có 3 loại mô hình Topology phổ biến
1. Bus Topology
![enter image description here](https://www.totolink.vn/public/uploads/img_article/cackieutopologycuamanglanbustopology.jpg)
Đặc điểm:  A muốn truyền dữ liệu sang B thì phải gửi dữ liệu ra ngoài môi trường truyền => All máy tính còn lại đều nhận được dữ liệu đó. Vì vậy tính bảo mật thông tin  không cao => Không còn được sử dụng rộng rãi
2.  Ring Topology
![enter image description here](https://www.totolink.vn/public/uploads/img_article/cackieutopologycuamanglanringtopology.jpg)
Đặc điểm: Dữ liệu được truyền theo vòng tròn. Từ A muốn truyền dữ liệu sang B thì phải thông qua các máy tính trung gian trong vòng cung quãng đường từ A sang B => Tính bảo mật cũng không cao => cũng không được sử dụng phổ biến. Thường sử dụng trong công nghệ StackWise của Cisco(Cho phép ghép 9 con Switch vật lí thành một con Switch hợp nhất => tổng hợp được nhiều port hơn).
Khuyết điểm: Multi point of failure - Nghĩa là bất cứ thiết bị nào trong Ring Topology bị mất kết nối thì đều ảnh hưởng tới toàn bộ hệ thống. Cách khắc phục là sử dụng mô hình Dual Ring: Bất kì đường truyền nào bị  mất thì hệ thống sẽ tự động sử dụng đường truyền còn lại.
![enter image description here](https://i.ytimg.com/vi/aus_Cwf234U/hqdefault.jpg)

3. Star Topology 
![enter image description here](https://www.totolink.vn/public/uploads/img_article/cackieutopologycuamanglanstartopology.jpg)
Đặc điểm: A muốn chuyển dữ liệu sang B thì chỉ cần thông qua điểm chính giữa mô hình => Tính bảo mật cao, dễ mở rộng, tốc độ truyền nhanh hơn hai mô hình còn lại => Được sử dụng rộng rãi.
Nhược điểm: Single point of failre - Nghĩa là nếu điểm chính giữa gặp sự cố thì toàn bộ hệ thống đều gặp sự cố. Cách khắc phụclà sử dụng mô hình Extended Star Topology: Nếu 1 điểm tập trung bị gặp sự cố thì các điểm không liên quan đến điểm tập trung này vẫn sẽ hoạt động bình thường.
![enter image description here](https://i.ytimg.com/vi/3h97jDfLeeY/hqdefault.jpg)
4. Full Mesh Topology
![enter image description here](https://scontent-sin6-1.xx.fbcdn.net/v/t1.15752-9/92552988_215034423143701_4420625459121750016_n.png?_nc_cat=106&_nc_sid=b96e70&_nc_ohc=_juHjXnnbswAX8PM_mf&_nc_ht=scontent-sin6-1.xx&oh=6d5a0384369a56ee97bfbb2c5f1536a7&oe=5EB0302B)
Đặc điểm: Từ một điểm sẽ có kết nối đến tất cả các điểm còn lại => Đảm bảo được tính dự phòng, tính sẵn sàng.
Nhược điểm: Tốn chi phí cao để triển khai mô hình Ful-Mesh => Cách khắc phục: Sử dụng mô hình Part-Mesh - chỉ kết nối những điểm cần thiết từ đó giảm thiểu được chi phí.

