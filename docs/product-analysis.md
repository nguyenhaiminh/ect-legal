# ECT Legal — Phân tích sản phẩm & kế hoạch triển khai

## 1. Bài toán

Doanh nghiệp và cá nhân khó trả lời nhanh 4 câu hỏi: văn bản nào điều chỉnh, chữ ký nào đủ tin cậy, hợp đồng điện tử cần lưu chứng cứ gì, và quy định có đang hiệu lực hay không. ECT Legal là lớp tra cứu và giải thích có căn cứ; không phải hệ thống phát hành chữ ký số và không thay thế luật sư.

## 2. Người dùng mục tiêu

| Persona | Nhu cầu | Rủi ro |
|---|---|---|
| HR/pháp chế | HĐLĐ điện tử, quy trình ký, lưu hồ sơ | Dùng văn bản cũ, thiếu chứng cứ |
| Sales/operations | Hợp đồng thương mại, ký từ xa | Sai thẩm quyền, sai phiên bản |
| Kế toán/IT | Chữ ký số, chứng thư, dấu thời gian | Không xác minh trạng thái ký |
| SME/chủ hộ | Hiểu nhanh “có được ký điện tử không” | Nhầm OTP với chữ ký số |

## 3. MVP (đã triển khai)

- Câu hỏi gợi ý theo 4 nhóm.
- Câu trả lời có kết luận, căn cứ, việc nên làm.
- Thư viện văn bản chính thức.
- Checklist 8 điểm trước khi ký.
- Không lưu nội dung câu hỏi trên máy chủ.

## 4. Giai đoạn 2

1. Bộ lọc theo loại văn bản, hiệu lực, lĩnh vực, cơ quan ban hành.
2. Trang chi tiết văn bản: metadata, điều liên quan, văn bản sửa đổi/thay thế.
3. Đồ thị quan hệ văn bản: Luật → Nghị định → Thông tư → hướng dẫn.
4. Import PDF/HTML từ nguồn chính thức, OCR có kiểm soát.
5. RAG có trích dẫn đoạn/điều, bắt buộc trả “không đủ căn cứ” khi không tìm thấy.
6. Nhật ký phiên bản tri thức và quy trình duyệt pháp chế.
7. Module đánh giá hợp đồng tải lên: chỉ phân tích, không tự kết luận thay luật sư.

## 5. KPI

- ≥95% câu trả lời có ít nhất một nguồn chính thức.
- 100% văn bản hiển thị trạng thái hiệu lực.
- Thời gian tìm đúng văn bản đầu tiên <60 giây.
- Tỷ lệ câu trả lời bị đánh dấu “thiếu căn cứ” <5% sau vòng review.

## 6. Không làm trong MVP

- Không tư vấn cá nhân hóa cho tranh chấp đang xét xử.
- Không lưu hoặc xử lý CCCD, chứng thư, hợp đồng thật trên máy chủ.
- Không tự ký, tự phát hành chứng thư hoặc tự xác thực danh tính.
