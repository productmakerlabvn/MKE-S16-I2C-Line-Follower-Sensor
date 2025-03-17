# MKE-S16 I2C Line Follower Sensor

![](/image/tren_duoi.jpg)

## Giới thiệu

Cảm biến dò đường MKE-S16 I2C Line Follower Sensor sử dụng 5 cảm biến CNY70 bao gồm 1 mắt phát và 1 mắt thu hồng ngoại, cảm biến dựa vào độ phản xạ của tia hồng ngoại theo màu sắc của vật thể ở gần để xác định 2 màu có độ tương phản cao (thường là trắng và đen), ứng dụng trong các mô hình xe dò đường (dò line), cảm biến trả ra giá trị thông qua việc gửi tín hiệu giao tiếp theo chuẩn I2C, ngoài ra cảm biến còn được bổ sung các thiết kế ổn định, chống nhiễu.

Cảm biến dò đường MKE-S16 I2C Line Follower Sensor thuộc hệ sinh thái phần cứng Robotics MakerEdu nên có thể sử dụng trực tiếp an toàn với các mạch điều khiển trung tâm ở cả hai mức điện áp 3.3VDC và 5VDC như: Arduino, Raspberry Pi, Jetson Nano, Micro:bit,....với chuẩn kết nối Connector XH2.54 thông dụng.

## Thông số kỹ thuật

- Model: MKE-S16 I2C Line Follower Sensor
- Điện áp hoạt động: 5VDC
- Dòng điện tiêu thụ khi hoạt động: khoảng 200mA
- Chuẩn giao tiếp: I2C
- Điện áp giao tiếp: TTL 3.3VDC / 5VDC
- Sử dụng trực tiếp an toàn với các board mạch giao tiếp ở cả hai mức điện áp 3.3VDC và 5VDC như: Arduino, Raspberry Pi, Jetson Nano, Micro:bit,....
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
- Nhấn 1 lần (click) trên button S1. Lúc này, từ LED1 đến LED5 sẽ nhấp nháy 3 lần, mỗi lần 1s (sáng 500ms, tối 500ms). Tùy thuộc vào số lượng sẽ tương ứng với từng địa chỉ:
![](/image/i2c_address_table3.png)  

<div align="center">
    <video src="https://github.com/user-attachments/assets/503f67e5-bcca-4757-b40e-602896822ca2" alt="epcb archery game" height=200/>
</div>






### Canh chỉnh ngưỡng (calibrate)


### Hướng dẫn sử dụng với Arduino (Code C)

[Hướng dẫn cài đặt phần mềm, nạp chương trình, cài đặt bộ thư viện Arduino cơ bản.](https://github.com/makerlabvn/Arduino-Vietduino)

- Tải và cài đặt [phần mềm Arduino tại đây.](https://www.arduino.cc/en/software)
- Trong Tools / Library Manager, tìm và cài đặt bộ thư viện tổng hợp "MAKERLABVN" by MakerLab.vn
- Mở chương trình mẫu "MKE_S16_I2C_Line_LCD_Serial" tại File / Examples / MAKERLABVN / Sensor / MKE_S16_I2C_Line_LCD_Serial hoặc [tải chương trình mẫu tại đây](/arduino)
- Chọn board là Arduino Uno (mạch Vietduino Uno tương thích với Arduino Uno), chọn đúng cổng COM Port của mạch và tiến hành nạp chương trình.
- Kết nối mạch Vietduino Uno với MakerEdu Shield, kết nối cảm biến và màn hình LCD vào cổng [I2C] trên MakerEdu Shield, cấp nguồn qua cổng USB của Vietduino Uno để thấy chương trình hoạt động.

## Hỗ trợ và liên hệ

- Website: [https://www.makerlab.vn/](https://www.makerlab.vn/)
- Facebook: [https://www.facebook.com/makerlabvn](https://www.facebook.com/makerlabvn)

## Nhà phân phối

- Các bạn có thể mua sản phẩm của MakerLab tại các [Nhà Phân Phối.](https://www.makerlab.vn/distributor/)
