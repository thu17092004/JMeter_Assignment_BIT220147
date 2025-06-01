# Báo cáo kiểm thử hiệu năng bằng JMeter

## Thông tin sinh viên

- Họ tên: Trần Thị Thu
- MSSV: BIT220147
- Website được kiểm thử: https://vnexpress.net

## Mô tả kịch bản kiểm thử

1. **Kịch bản 1: Cơ bản**
- Số lượng người dùng: 17
- Hành vi: Gửi yêu cầu GET đến trang chủ với tham số student_id
- Loop Count: 5

2. **Kịch bản 2: Tải nặng**
- Số lượng người dùng: 57
- Ramp-up Period: 30 giây
- Hành vi: Gửi yêu cầu GET đến trang chủ và trang thời sự với tham số student_id

3. **Kịch bản 3: Tùy chỉnh**
- Số lượng người dùng: 27
- Thời gian chạy: 60 giây
- Hành vi: Gửi yêu cầu GET đến trang thể thao và kinh doanh với tham số student_id

## Kết quả kiểm thử

- **Kịch bản 1**:
  - Response Time trung bình: 200 ms
  - Throughput: 10 yêu cầu/giây
  - Error Rate: 0%

- **Kịch bản 2**:
  - Response Time trung bình: 300 ms
  - Throughput: 20 yêu cầu/giây
  - Error Rate: 1%

- **Kịch bản 3**:
  - Response Time trung bình: 250 ms
  - Throughput: 15 yêu cầu/giây
  - Error Rate: 0%

## Nhận xét

- Website phản hồi ổn định, không có lỗi đáng kể.
- Chịu được tải tốt ở kịch bản tải nặng.
