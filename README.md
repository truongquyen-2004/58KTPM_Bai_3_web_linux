# 58KTPM_Bai_3_web_linux
###  Trương Văn Quyến
### MSSV K225480106083-K58-KTP
###  Bài tập 3   : môn Phát triển ứng dụng trên nền web
# Giảng viên  : Đỗ Duy Cốp
####  Lớp học phần: 58KTPM
####  Ngày giao   : 2025-10-24 13:50
####  Hạn nộp     : 2025-11-05 00:00
--------------------------------------------------
Yêu cầu     : LẬP TRÌNH ỨNG DỤNG WEB trên nền linux
###    1. Cài đặt môi trường linux: SV chọn 1 trong các phương án
enable wsl: cài đặt docker desktop
####    kết quả
  <img width="1889" height="278" alt="Screenshot 2025-11-05 171730" src="https://github.com/user-attachments/assets/9ca14bfd-d534-4011-92cc-9faaa66693f1" />
  <img width="1584" height="915" alt="image" src="https://github.com/user-attachments/assets/71e03206-27c3-4671-90c7-7f1a62ed7b3f" />
###     2. Cài đặt Docker (nếu dùng docker desktop trên windows thì nó có ngay)
####    kết quả:
  <img width="1889" height="278" alt="image" src="https://github.com/user-attachments/assets/d44b08a6-3ef6-4adb-aed8-3782c4be9010" />
###    3. Sử dụng 1 file docker-compose.yml để cài đặt các docker container sau: 
   mariadb (3306), phpmyadmin (8080), nodered/node-red (1880), influxdb (8086), grafana/grafana (3000), nginx (80,443)
  ###     kết quả:
   <img width="1914" height="1008" alt="image" src="https://github.com/user-attachments/assets/495fe66a-aa96-4666-9819-daa09987af33" />
   <img width="1901" height="997" alt="image" src="https://github.com/user-attachments/assets/13948535-ad24-4ff7-b5db-7df3a307c63e" />
   <img width="1911" height="1023" alt="image" src="https://github.com/user-attachments/assets/ae9a1929-f066-4718-87d8-3666ef08c152" />
###    4. Lập trình web frontend+backend:
 SV chọn 1 trong các web sau:
 4.1 Web thương mại điện tử
 - Tạo web dạng Single Page Application (SPA), chỉ gồm 1 file index.html, toàn bộ giao diện do javascript sinh động.
 ####     kết quả:
   <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/05374235-a215-4992-8fbf-c4c900d167e3" />
 - Có tính năng login, lưu phiên đăng nhập vào cookie và session
  ####   kết quả:
   <img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/09dede02-ad39-48df-808b-289467638bf5" />
 - Thông tin login lưu trong cơ sở dữ liệu của mariadb, được dev quản trị bằng phpmyadmin, yêu cầu sử dụng mã hoá khi gửi login.
 ####    kết quả:
   <img width="1516" height="1020" alt="image" src="https://github.com/user-attachments/assets/e7217447-1b2d-4487-b7fa-7b04d3bff21b" />
   Chỉ cần login 1 lần, bao giờ logout thì mới phải login lại.
 ####   kết quả:
   <img width="1853" height="597" alt="image" src="https://github.com/user-attachments/assets/45d7ab09-3db2-4a53-a573-97b93c48aa28" />
   Có tính năng liệt kê các sản phẩm bán chạy ra trang chủ
 - Có tính năng liệt kê các nhóm sản phẩm
   ####  kết quả:
   <img width="1919" height="1079" alt="Screenshot 2025-11-06 210706" src="https://github.com/user-attachments/assets/03a7063e-7292-4951-af83-ae628025845a" />
  Có tính năng liệt kê sản phẩm theo nhóm
####    kết quả:
<img width="1870" height="888" alt="image" src="https://github.com/user-attachments/assets/bd7a0dbd-ee73-496c-aadf-1d6f33c30269" />
  Có tính năng tìm kiếm sản phẩm
  ####  kết quả:
   <img width="1452" height="598" alt="image" src="https://github.com/user-attachments/assets/53ed621a-d8f5-4c47-a1ea-03c00dd3a190" />
###   5. Nginx làm web-server
 - Cấu hình nginx để chạy được website qua url http://fullname.com  (thay fullname bằng chuỗi ko dấu viết liền tên của bạn)
  ####   kết quả:
  <img width="1774" height="718" alt="image" src="https://github.com/user-attachments/assets/86228f87-851b-44bd-a332-ae83ab032acb" />
 - Cấu hình nginx để http://fullname.com/nodered truy cập vào nodered qua cổng 80, (dù nodered đang chạy ở port 1880)
  ####   kết quả:
  <img width="1915" height="879" alt="image" src="https://github.com/user-attachments/assets/f136ba2a-881e-4321-8fb1-f182f4c2df9b" />
 - Cấu hình nginx để http://fullname.com/grafana truy cập vào grafana qua cổng 80, (dù grafana đang chạy ở port 3000)
####  kết quả:
<img width="1912" height="819" alt="image" src="https://github.com/user-attachments/assets/ede1a38d-60e8-4e70-a15c-3cdda8cc0f4e" />
Yêu cầu sinh viên lưu code trên github
có file readme.md có hình ảnh + text: ghi lại nhật ký quá trình làm bài.

CÁCH ĐÁNH GIÁ:
1. Cài đặt được môi trường: 1đ
2. Cài đặt được các docker container với cấu hình phù hợp: 1đ
3. Web chạy được, giao diện phù hợp, chạy trên web sever nginx: 2đ
4. nodered api trả về json, test được: 2đ
5. front-end có js gọi được api nodered, nhận về json, hiển thị được kết quả từ json này. 2đ
6. Bài làm có dấu ấn, giải thích rõ ràng, hiểu vấn đề: 2đ
