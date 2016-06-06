#Báo cáo tuần 1
##I.Mô hình OSI
<img src="http://i.imgur.com/kUahocC.png">
##II.Bộ giao thức TCP/IP
###1. Khái niệm
 TCP/IP là bộ giao thức cho phép kết nối các hệ thống mạng không đồng nhất với nhau. Ngày nay TCP/IP được sử dụng rộng rãi trong mạng cục bộ cũng như mạng toàn cầu.
TCP/IP được xem như giản lược của mô hình tham chiếu OSI với 4 tầng như sau:
<ul>
<li>Tầng Liên Kết (Datalink Layer)
<li>Tầng Mạng (Internet Layer)
<li>Tầng Giao Vận (Transport Layer)
<li> Tầng Ứng Dụng (Application Layer)

<img src="http://i.imgur.com/1t0SWDp.png?1">
</ul>

####Tầng liên kết:
 Tầng liên kết (còn được gọi là tầng liên kết dữ liệu hay tầng giao tiếp mạng) là tầng thấp nhất trong mô hình TCP/IP, bao gồm các thiết bị giao tiếp mạng và các chương trình cung cấp các thông tin cần thiết để có thể hoạt động, truy nhập đường truyền vật lý qua các thiết bị giao tiếp mạng đó.
####Tầng Internet: 
Tầng Internet ( hay còn gọi là tầng Mạng) xử lý quá trình truyền gói tin trên mạng, các giao thức của tầng này bao gồm : IP ( Internet Protocol) , ICMP ( Internet Control Message Protocol) , IGMP ( Internet Group Message Protocol )
####Tầng giao vận: 
Tầng giao vận phụ trách luồng dữ liệu giữa 2 trạm thực hiện các ứng dụng của tầng trên, tầng này có 2 giao thức chính là TCP ( Transmisson Control Protocol) và UDP ( User Datagram Protocol )
<li>TCP cung cấp luồng dữ liệu tin cậy giữa 2 trạm, nó sử dụng các cơ chế như chia nhỏ các gói tin ở tầng trên thành các gói tin có kích thước thích hợp cho tầng mạng bên dưới, báo nhận gói tin, đặt hạn chế thời gian timeout để đảm bảo bên nhân biết được các gói tin đã gửi đi. Do tầng này đảm bảo tính tin cậy nên tầng trên sẽ không cần quan tâm đến nữa
<li>UDP cung cấp một dịch vụ rất đơn giản hơn cho tầng ứng dụng . Nó chỉ gửi dữ liệu từ trạm này tới trạm kia mà không đảm bảo các gói tin đến được tới đích. Các cơ chế đảm bảo độ tin cậy được thực hiện bởi tầng trên
####Tầng ứng dung: 
Tầng trên của mô hình TCP/IP bao gồm các tiến trình và các ứng dụng cung cấp cho người sử dụng để truy cập mạng. Có rất nhiều ứng dụng được cung cấp trong tầng này , mà phổ biến là Telnet: sử dụng trong việc truy cập mạng từ xa, FTP ( File Transport Protocol ) dịch vụ truyền tệp tin., EMAIL : dịch vụ truyền thư tín điện tử. WWW ( Word Wide Web )
</ul>
###2. Nguyên tắc hoạt động của nó như sau: 
<ul>
<li>Dữ liệu truyền từ một ứng dụng TCP/IP hoặc ứng dụng mạng thông qua một cổng TCP hay UDP tới giao thức lớp TCP hoặc UDP. Các chương trình có thể truy cập mạng qua TCP hoặc UDP, điều này phụ thuộc vào yêu cầu của chương trình. 
<ul>
<li>TCP là một giao thức định hướng kết nối. Các giao thức định hướng kết nối cung cấp khả năng kiểm soát giao thông và kiểm tra lỗi tinh vi hơn các giao thức không định hướng kết nối. TCP đảm bảo việc lưu chuyển của dữ liệu và đáng tin cậy hơn UDP, nhưng việc có thêm những chức năng này đồng nghĩa rằng TCP chậm hơn UDP. 
<li> UDP là giao thức không định hướng kết nối. Nó nhanh hơn TCP, nhưng mức độ tin cậy thấp hơn. 
</ul>
</ul>
<ul>
 <li>Khi các gói dữ liệu đi tới cấp Internet, tại đây giao thức IP cung cấp thông tin địa chỉ logic và gắn thông tin đó vào gói dữ liệu. 
</ul>
<ul> 
<li>Gói dữ liệu có IP tiến vào Lớp Truy cập mạng, tại đây nó chuyển giao cho bộ phận phần mềm được thiết kế để tương tác với mạng vật lý. Lớp Truy cập mạng tạo ra một hoặc nhiều khung dữ liệu để nó có thể vào mạng vật lý. 
</ul>
<ul>
<li>Khung dữ liệu sẽ được chuyển đổi thành một dải bit để tới bộ phận trung gian mạng. 





