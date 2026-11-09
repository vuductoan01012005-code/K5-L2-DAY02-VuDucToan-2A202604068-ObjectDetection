# Mini guideline — bài làm cá nhân

> Điền nội dung này trước khi bắt đầu gán nhãn. Giữ lại các quyết định sau khi self-QC.

## Định nghĩa lớp

| Lớp     | Định nghĩa của bạn                                                                                                   | Ví dụ/điểm phân biệt                                                                         |
| ------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `car`   | Xe chở người kích thước nhỏ đến trung bình, thường có 4 bánh, dưới khoảng 9 chỗ ngồi.                                | Sedan, hatchback, coupe, SUV cỡ nhỏ. Không gán truck nếu mục đích chính không phải chở hàng. |
| `truck` | Xe tải hoặc phương tiện có khoang/thùng chở hàng riêng biệt hoặc thiết kế chính để vận chuyển hàng hóa.              | Pickup, light truck, cargo truck, container truck. Pickup vẫn được gán truck.                |
| `bus`   | Phương tiện thiết kế để chở nhiều hành khách theo tuyến hoặc vận tải công cộng.                                      | Xe buýt thành phố, xe khách, shuttle bus, coach bus.                                         |
| `van`   | Xe thân hộp, khoang hành khách và khoang hàng liền khối. Kích thước lớn hơn ô tô thông thường nhưng nhỏ hơn xe buýt. | Minivan, cargo van, passenger van. Ưu tiên van khi xe có thân hộp đặc trưng.                 |

## Quy tắc chung

- Box bám sát vật thể nghĩa là:Bounding box phải bao quanh toàn bộ phần nhìn thấy của vật thể, tiếp xúc sát biên ngoài cùng của xe nhưng không chứa nhiều nền không cần thiết.
- Vật thể bị che khuất: Vẫn gán nhãn nếu có thể nhận diện chắc chắn lớp đối tượng. Box bao quanh toàn bộ phần còn nhìn thấy được của vật thể.
- Vật thể bị cắt bởi rìa ảnh: Vẫn gán nhãn nếu có thể xác định loại xe. Box kéo đến mép ảnh và phủ toàn bộ phần xuất hiện trong ảnh.
- Vật thể rất nhỏ/mơ hồ: Không gán nhãn nếu không thể xác định chắc chắn class theo schema. Ưu tiên tính nhất quán hơn là đoán.

## Ghi lại quyết định cho ít nhất ba ca mơ hồ

| Ảnh         | Tình huống | Quyết định cuối | Lý do theo schema |
| ----------- | ---------- | --------------- | ----------------- |
| `drive_...` |            |                 |                   |
| `drive_...` |            |                 |                   |
| `drive_...` |            |                 |                   |
