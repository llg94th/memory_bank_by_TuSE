[memory-bank-instructions](rule/memory-bank-instructions_vi.md)
# Cách sử dụng Memory Bank và Modes để làm việc nhanh hơn
## Nguyên tắc hoạt động
### Memory Bank:

Memory Bank là một tập hợp các tài nguyên cần thiết để tự động hoàn thành các tác vụ cho một dự án. Nó bao gồm các tài nguyên liên quan đến công cụ, hệ thống, lớp và thuật ngữ cơ bản. Nó được sử dụng để giải quyết các vấn đề liên quan đến các tác vụ thông thường và khó khăn trong việc hoàn thành dự án.

### Modes:

Modes là một tập hợp các câu hỏi và mục tiêu cho một dự án. Nó bao gồm các câu hỏi và mục tiêu liên quan đến các tác vụ thông thường và khó khăn trong việc hoàn thành dự án. Nó được sử dụng để giải quyết các vấn đề liên quan đến các tác vụ thông thường và khó khăn trong việc hoàn thành dự án.

## Cách thiết lập:
### Cursor: Modes tùy chỉnh 
    - https://docs.cursor.com/en/agent/modes#agent
### VS Code: Chat Modes tùy chỉnh
    - https://code.visualstudio.com/docs/copilot/customization/overview
### Quy tắc tùy chỉnh
    Sử dụng memory-bank-instructions.md để tạo quy tắc tùy chỉnh.
    
## Cách sử dụng Memory Bank:
### Làm việc với Memory Bank
#### Quy trình cốt lõi
Khởi tạo Memory Bank
Bước khởi tạo rất quan trọng vì nó tạo nền tảng cho tất cả các tương tác trong tương lai với dự án của bạn. Khi bạn yêu cầu khởi tạo với lệnh initialize memory bank, XYZ Code sẽ:

1. Thực hiện phân tích toàn diện dự án của bạn, bao gồm:
    - Tất cả các tệp mã nguồn và mối quan hệ của chúng
    - Các tệp cấu hình và thiết lập hệ thống build
    - Cấu trúc và mô hình tổ chức dự án
    - Tài liệu và chú thích
    - Các phụ thuộc và tích hợp bên ngoài
    - Các framework và mô hình kiểm thử
2. Tạo các tệp memory bank toàn diện trong thư mục ./memory-bank
3. Cung cấp bản tóm tắt chi tiết về những gì nó đã hiểu về dự án của bạn
4. Yêu cầu bạn xác minh tính chính xác của các tệp đã tạo

***Quan trọng***:

Hãy dành thời gian để xem xét và sửa chữa cẩn thận các tệp đã tạo sau khi khởi tạo. Bất kỳ hiểu lầm hoặc thiếu thông tin nào ở giai đoạn này sẽ ảnh hưởng đến tất cả các tương tác trong tương lai. Việc khởi tạo kỹ lưỡng cải thiện đáng kể hiệu quả của XYZ Code, trong khi khởi tạo vội vàng hoặc không đầy đủ sẽ vĩnh viễn hạn chế khả năng hỗ trợ bạn một cách hiệu quả.

#### Cập nhật Memory Bank
Memory Bank được cập nhật khi:

1. XYZ Code phát hiện các mẫu dự án mới
2. Sau khi thực hiện các thay đổi quan trọng
3. Khi bạn yêu cầu rõ ràng với update memory bank
4. Khi ngữ cảnh cần làm rõ

Để thực hiện cập nhật Memory Bank, XYZ Code sẽ:

1. Xem xét TẤT CẢ các tệp dự án
2. Ghi lại trạng thái hiện tại
3. Ghi lại các hiểu biết sâu sắc và mẫu
4. Cập nhật tất cả các tệp memory bank khi cần thiết

Bạn có thể hướng dẫn XYZ Code tập trung vào các nguồn thông tin cụ thể bằng cách sử dụng các lệnh như update memory bank using information from @/Makefile.

#### Thực thi tác vụ thường xuyên
Khi bắt đầu mỗi tác vụ, XYZ Code:

1. Đọc TẤT CẢ các tệp memory bank
2. Bao gồm [Memory Bank: Active] ở đầu phản hồi của nó
3. Cung cấp bản tóm tắt ngắn gọn về hiểu biết của nó về dự án của bạn
4. Tiến hành với tác vụ được yêu cầu

Khi kết thúc một tác vụ, XYZ Code có thể đề xuất cập nhật memory bank nếu có những thay đổi quan trọng được thực hiện, sử dụng cụm từ: "Bạn có muốn tôi cập nhật memory bank để phản ánh những thay đổi này không?"

#### Quy trình thêm tác vụ
Khi bạn hoàn thành một tác vụ lặp đi lặp lại theo một mẫu tương tự mỗi lần, bạn có thể ghi lại nó để tham khảo trong tương lai. Điều này đặc biệt hữu ích cho các tác vụ như thêm tính năng theo các mẫu hiện có

Để ghi lại một tác vụ, sử dụng lệnh add task hoặc store this as a task. XYZ Code sẽ:

1. Tạo hoặc cập nhật tệp tasks.md trong thư mục memory bank
2. Ghi lại tác vụ sử dụng ngữ cảnh hiện tại:
    - Tên và mô tả tác vụ
    - Danh sách các tệp cần được sửa đổi
    - Quy trình từng bước
    - Các cân nhắc quan trọng
    - Ví dụ triển khai

Khi bắt đầu một tác vụ mới, XYZ Code sẽ kiểm tra xem nó có khớp với bất kỳ tác vụ đã ghi lại nào không và tuân theo quy trình đã thiết lập để đảm bảo không bỏ sót bước nào.

#### Các lệnh chính

- initialize memory bank - Sử dụng khi bắt đầu một dự án mới
- update memory bank - Khởi tạo việc phân tích lại toàn diện tài liệu ngữ cảnh cho tác vụ hiện tại. Thận trọng: Điều này tốn nhiều tài nguyên và không được khuyến nghị cho các mô hình "nhẹ" do có thể giảm hiệu quả. Có thể được sử dụng nhiều lần, kết hợp tốt với các hướng dẫn cụ thể, ví dụ: update memory bank using information from @/Makefile
- add task hoặc store this as a task - Ghi lại một tác vụ lặp đi lặp lại để tham khảo trong tương lai

#### Chỉ báo trạng thái
XYZ Code sử dụng các chỉ báo trạng thái để truyền đạt rõ ràng trạng thái Memory Bank:

- [Memory Bank: Active] - Chỉ ra rằng các tệp Memory Bank đã được đọc thành công và đang được sử dụng
- [Memory Bank: Missing] - Chỉ ra rằng không thể tìm thấy các tệp Memory Bank hoặc chúng trống rỗng
Các chỉ báo này xuất hiện ở đầu phản hồi của XYZ Code, cung cấp xác nhận ngay lập tức về trạng thái Memory Bank.

#### Cập nhật tài liệu
Cập nhật Memory Bank nên tự động xảy ra khi:

- Bạn phát hiện các mẫu mới trong dự án của mình
- Sau khi thực hiện các thay đổi quan trọng
- Khi bạn yêu cầu rõ ràng với update memory bank
- Khi bạn cảm thấy ngữ cảnh cần làm rõ
