# Nhật ký điều chỉnh và Mapping (TodoList -> Worksheet 01)

File này tóm tắt các thay đổi chính khi "lắp ghép" nội dung từ nháp của bạn vào file nộp chính thức.

## 1. Mapping nội dung

| Hạng mục trong Todolist | Vị trí trong 01-risk-map.md | Thay đổi/Điều chỉnh của AI |
| :--- | :--- | :--- |
| **Track 04** | Section 1 | Giữ nguyên tên và số track. Phần "Lý do chọn" được trau chuốt lại để nhấn mạnh tính thực tiễn. |
| **Scenario** | Section 2 | Gộp các ý về nhập liệu giọng nói/OCR và hậu quả thực tế vào 4 trường chuẩn của worksheet. |
| **8 lỗi sai (Tư duy)** | Section 3 (Candidates) | Chọn lọc 3 lỗi tiêu biểu nhất (Hallucination, Sycophancy, PII Leakage) để đảm bảo tính đa dạng và Severity thực tế. |
| **Failure Deep Dive** | Section 4 | Chọn lỗi **Hallucination (cộng sai tiền)** làm lỗi chính vì nó ảnh hưởng trực tiếp đến cốt lõi của ứng dụng tài chính (sự chính xác). |
| **Harm Map** | Section 5 | Chuyển đổi các ý về "Affected person" và "Hidden harm" sang định dạng bảng, làm rõ rủi ro "Over-reliance" (quá tin vào máy). |

## 2. Các điểm AI đã bổ sung/điều chỉnh quan trọng

- **Layer Mapping (Cực kỳ quan trọng):** Trong `todolist.md` bạn mới liệt kê lớp, tôi đã thực hiện map cụ thể lỗi nào đến từ Layer nào (Layer 1: Input, Layer 2: RAG, Layer 3: Model, v.v.) theo đúng khung lý thuyết 5 lớp của bài học.
- **Bad Behavior vs Expected Behavior:** Chuyển các mô tả chung chung thành các câu "quote" (trích dẫn) cụ thể của AI để đáp ứng tiêu chuẩn "testable" (có thể kiểm thử được).
- **Failure Pattern Sentence:** Xây dựng câu tóm tắt lỗi theo đúng cấu trúc: *“Khi [Context], AI có xu hướng [Bad Behavior] thay vì [Expected Behavior], gây hậu quả cho [Who]”*.
- **Severity Rule:** Phân loại lại mức độ nghiêm trọng (High cho sai lệch tiền bạc, Medium cho rủi ro trải nghiệm).

## 3. Lưu ý cho bạn
- Bạn cần mở file `worksheet/01-risk-map.md` để điền nốt **Họ tên** và **Mã học viên** vào Section 1.
- Các phần Prompt phản biện trong Worksheet đã được giữ nguyên để bạn có thể copy và sử dụng với AI nhằm tối ưu hóa thêm bài làm của mình.
