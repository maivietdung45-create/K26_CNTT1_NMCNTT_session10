
## Phần 1. Phân tích

-   Input: Dữ liệu nhiệt độ, độ ẩm đất từ cảm biến.
    
-   Output: Tín hiệu điều khiển máy bơm và nhật ký hoạt động.
    
-   Sơ đồ phần cứng: Cảm biến → SoC → Rơ-le → Máy bơm.
    

## Phần 2. README.md

# 🚀 Smart-Farm

## 1. Mô tả

Smart-Farm là hệ thống IoT giúp theo dõi môi trường và tự động tưới cây tại trang trại Lan.

## 2. Hướng dẫn cài đặt

```
Kết nối cảm biến với SoC
Kết nối SoC với rơ-le và máy bơm
Cài đặt ngưỡng tưới
Khởi động hệ thống
```

## 3. Tính năng

-  [x] Theo dõi nhiệt độ và độ ẩm đất.
    
-  [x] Tự động điều khiển máy bơm.
    
-  [x] Lưu nhật ký hoạt động.
    

## 4. Bảng thông số

Thành phần|Chức năng
|:-:|:-:
Cảm biến|Thu thập dữ liệu
SoC|Xử lý dữ liệu
Rơ-le|Điều khiển máy bơm
Máy bơm|Tưới cây

## 5. Chu kỳ Fetch - Decode - Execute

> Fetch: CPU lấy lệnh từ bộ nhớ.
> 
> Decode: CPU giải mã lệnh.
> 
> Execute: CPU thực hiện lệnh điều khiển tưới cây thông qua rơ-le.

## 6. Mô hình DIKW

```
        Wisdom - Hành động tưới
       Knowledge - Kiến thức
      Information - Thông tin
     Data - Dữ liệu cảm biến
```

-   Data: Nhiệt độ 36°C, độ ẩm đất 25%.
    
-   Information: Nhiệt độ cao, đất khô.
    
-   Knowledge: Đất cần được tưới theo ngưỡng cài đặt.
    
-   Wisdom: Bật máy bơm khi điều kiện an toàn.
    

## 7. Lưu ý khi RAM đầy

-   Kiểm tra tiến trình đang sử dụng RAM.
    
-   Sao lưu nhật ký trước khi dọn dẹp.
    
-   Giới hạn kích thước và xoay vòng nhật ký.
    
-   Không tự ý tắt tiến trình điều khiển máy bơm.
    
-   Kiểm tra lại hệ thống sau khi xử lý.
