# MKE-S16 I2C Line Follower Sensor

![](/image/tren_duoi.jpg)

## Giới thiệu

Cảm biến dò đường MKE-S16 I2C Line Follower Sensor sử dụng 5 cảm biến CNY70 bao gồm 1 mắt phát và 1 mắt thu hồng ngoại, cảm biến dựa vào độ phản xạ của tia hồng ngoại theo màu sắc của vật thể ở gần để xác định 2 màu có độ tương phản cao (thường là trắng và đen), ứng dụng trong các mô hình xe dò đường (dò line), cảm biến trả ra giá trị thông qua việc gửi tín hiệu giao tiếp theo chuẩn I2C, ngoài ra cảm biến còn được bổ sung các thiết kế ổn định, chống nhiễu và có thể điều chỉnh độ nhạy (calibrate), kiểm tra và thiết lập địa chỉ I2C bằng nút nhấn.

Cảm biến dò đường MKE-S16 I2C Line Follower Sensor thuộc hệ sinh thái phần cứng Robotics MakerEdu nên có thể sử dụng trực tiếp an toàn với các mạch điều khiển trung tâm ở cả hai mức điện áp 3.3VDC và 5VDC như: Arduino, Vietduino UNO, Vietduino MEGA 2560, Vietduino WiFi BLE ESP32 với mạch MakerEdu Shield for Vietduino và micro:bit V2 sử dụng với mạch MakerEDU Shield for Micro:bit, with 2 x DC Motor Driver.

## Thông số kỹ thuật

- Model: MKE-S16 I2C Line Follower Sensor
- Điện áp hoạt động: 5VDC
- Dòng điện tiêu thụ khi hoạt động: khoảng 200mA
- Chuẩn giao tiếp: I2C / Digital Output
- Điện áp giao tiếp: TTL 3.3VDC / 5VDC
- Bổ sung thêm các thiết kế ổn định, chống nhiễu.
- Chuẩn kết nối: connector XH2.54 4Pins
- Thuộc hệ sinh thái phần cứng Robotics MakerEdu, tương thích tốt nhất khi sử dụng với các mạch điều khiển trung tâm của MakerEdu và MakerEdu Shield.

## Hình ảnh sản phẩm

![](/image/tren_nghieng.jpg)
![](/image/duoi_nghieng.jpg)

## Kích thước sản phẩm

![](/image/kich_thuoc.png)

## Các chân tín hiệu

- GND: Chân cấp nguồn âm 0VDC
- 5V: Chân cấp nguồn dương 5VDC
- SDA: Chân I2C Data
- SCL: Chân I2C Clock

## Hướng dẫn sử dụng

### Cấu hình và kiểm tra địa chỉ I2C

> - Nhấn 1 lần (click) trên button S1. Lúc này, từ LED1 đến LED5 sẽ nhấp nháy 3 lần, mỗi lần 1s (sáng 500ms, tối 500ms). Tùy thuộc vào số lượng sẽ tương ứng với từng địa chỉ.
> - Nhấn 2 lần (double-click) trên button S1 sẽ vào chế độ chọn địa chỉ I2C. Lúc này LED1 đến LED5 sẽ nhấp nháy. Địa chỉ I2C phụ thuộc vào số LED đang nhấp nháy. Có thể nhấn 2 lần (double-click) để chuyển đổi giữa các địa chỉ từ 0x2A đến 0x2F.

![](/image/i2c_address_table3.png)  

<div align="center">
    <video src="https://github.com/user-attachments/assets/503f67e5-bcca-4757-b40e-602896822ca2" alt="epcb archery game" height=200/>
</div>
<div align="center">
    <video src="https://github.com/user-attachments/assets/d76a3913-eee5-4d72-bf05-90476b31d5f6" alt="epcb archery game" height=200/>
</div>
<div align="center">
    <video src="https://github.com/user-attachments/assets/aedaceb6-1f65-4b47-9fe6-f23fb784876a" alt="epcb archery game" height=200/>
</div>
<div align="center">
    <video src="https://github.com/user-attachments/assets/44368f72-b69c-4e4e-850e-8efde34bb425" alt="epcb archery game" height=200/>
</div>
<div align="center">
    <video src="https://github.com/user-attachments/assets/10ad4042-c6da-49c0-a26f-9fcb32b2ee81" alt="epcb archery game" height=200/>
</div>

> Sau khi chọn địa chỉ, nhấn giữ button S1 (long-click) để lưu lại địa chỉ I2C đã chọn. Lúc này 5 LED sẽ nhấp nháy liên tục 5 lần, mỗi lần 200ms rồi tắt.

<div align="center">
    <video src="https://github.com/user-attachments/assets/5231e366-127b-4e34-bafb-812b8dfff47d" alt="epcb archery game" height=200/>
</div>

### Canh chỉnh ngưỡng (calibrate)
>
> - Khoảng cách lý tưởng của cảm biến với mặt đất là từ 0.5cm - 1cm
> - Khi canh chỉnh thì phải để cảm biến tiếp xúc với màu **tối hơn**

Đặt cảm biến vào vùng có màu tối hơn, nhấn giữ (long-click) button S1 để cảm biến tính toán độ nhạy (ngưỡng nhận). Các LED từ 1 đến 5 sẽ chớp 10 lần, mỗi lần 200ms.

### Hướng dẫn sử dụng với Arduino (Code C)

[Hướng dẫn cài đặt phần mềm, nạp chương trình, cài đặt bộ thư viện Arduino cơ bản.](https://github.com/makerlabvn/Arduino-Vietduino)

### Sơ đồ kết nối

- I2C
![](/image/vuno_mkeS16_i2c.jpg)

- Digital Out
![](/image/vuno_mkeS16_DO.jpg)

### Sử dụng cảm biến ở chế độ I2C

- Tải và cài đặt [phần mềm Arduino tại đây.](https://www.arduino.cc/en/software)
- Trong Tools / Library Manager, tìm và cài đặt bộ thư viện tổng hợp "MAKERLABVN" by MakerLab.vn
- Mở chương trình mẫu "I2C_Line_Follower_Sensor_Serial_Basic.ino" tại File / Examples / MAKERLABVN / Sensor / MKE_S16_I2C_LineFollower_LCD_Serial hoặc [tải chương trình mẫu tại đây](/arduino)
- Chọn board là Arduino Uno (mạch Vietduino Uno tương thích với Arduino Uno), chọn đúng cổng COM Port của mạch và tiến hành nạp chương trình.
- Kết nối mạch Vietduino Uno với MakerEdu Shield, kết nối cảm biến và màn hình LCD vào cổng [I2C] trên MakerEdu Shield, cấp nguồn qua cổng USB của Vietduino Uno để thấy chương trình hoạt động.

### Sử dụng cảm biến ở chế độ Digital Output

- Tải và cài đặt [phần mềm Arduino tại đây.](https://www.arduino.cc/en/software)
- Trong Tools / Library Manager, tìm và cài đặt bộ thư viện tổng hợp "MAKERLABVN" by MakerLab.vn
- Mở chương trình mẫu "I2C_Line_Follower_Sensor_Serial_Basic_5_Digital.ino" tại File / Examples / MAKERLABVN / Sensor / MKE_S16_I2C_LineFollower_LCD_Serial hoặc [tải chương trình mẫu tại đây](/arduino)
- Chọn board là Arduino Uno (mạch Vietduino Uno tương thích với Arduino Uno), chọn đúng cổng COM Port của mạch và tiến hành nạp chương trình.
- Kết nối mạch Vietduino Uno với MakerEdu Shield, kết nối cảm biến và màn hình LCD vào cổng [I2C] trên MakerEdu Shield, cấp nguồn qua cổng USB của Vietduino Uno để thấy chương trình hoạt động.

## Hỗ trợ và liên hệ

- Website: [https://www.makerlab.vn/](https://www.makerlab.vn/)
- Facebook: [https://www.facebook.com/makerlabvn](https://www.facebook.com/makerlabvn)

## Nhà phân phối

- Các bạn có thể mua sản phẩm của MakerLab tại các [Nhà Phân Phối.](https://www.makerlab.vn/distributor/)
