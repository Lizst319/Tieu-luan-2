# Bien so xe
_Một hệ thống nhận dạng biển số xe tự động cho biển số Việt Nam_

Hệ thống này có thể phát hiện và nhận dạng 2 loại biển số xe ở Việt Nam, biển số chữ nhật và biển số vuông

## Tong quat
- Hệ thống này có thể phát hiện và nhận dạng biển số xe từ hình ảnh, video và webcam.
- Trong dự án này, vị trí của camera là cố định và mỗi lần chỉ có một xe ô tô chạy qua cổng. Do đó, hệ thống chỉ có thể phát hiện 1 tấm trên mỗi khung hình.
## Phuong phap
1. Phát hiện mảng
   - Sobel X để phát hiện các cạnh dọc theo sau bởi một sự biến đổi hình thái.
   - Tìm các đường bao thỏa mãn tỷ lệ của tấm để có được các tấm có thể
   - Kiểm tra các ký tự trên biển số có thể tìm thấy để đảm bảo đó là biển số xe.
2. Nhận dạng tấm
   - Để nhận dạng ký tự, tôi đã sử dụng MobileNet_v1_0.5_128 vì nó nhẹ và phù hợp để nhận dạng thời gian thực.

## Yeu cau
- python 3.6 - 3.9
- chạy `pip install -r request.txt

## Thuc hien
- chạy `test.py` để thử nghiệm trên video.
- chạy `test_image.py` để thử nghiệm trên một hình ảnh.
## Ket qua
- ![Demo](https://github.com/Lizst319/Tieu-luan-2/blob/main/screenshot_1.png)
- ![Demo](https://github.com/Lizst319/Tieu-luan-2/blob/main/screenshot_2.png)
