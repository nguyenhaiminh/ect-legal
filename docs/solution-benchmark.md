# ECT Legal — Tham khảo giải pháp thị trường

Các điểm dưới đây là năng lực được nhà cung cấp công bố, dùng để tham khảo product discovery; không phải xác nhận độc lập về tuân thủ.

| Nhà cung cấp | Năng lực đáng tham khảo | Bài học cho ECT Legal | Nguồn |
|---|---|---|---|
| VNPT eContract | Tạo/ký hàng loạt, tra cứu dữ liệu nhân sự, kết nối nền tảng HĐLĐ điện tử | Cần mô hình trạng thái hợp đồng và batch workflow | [VNPT](https://vnpt.vn/doanh-nghiep/tu-van/giai-phap-hop-dong-dien-tu-vnpt-econtract-an-toan-nhanh-chong-tin-cay) |
| Viettel vContract | USB Token, Cloud CA, Mobile CA, OTP/eKYC/ký ảnh, gửi email/SMS | Cần giải thích rõ “phương thức xác thực” khác “chữ ký số” | [Viettel](https://shop.viettel.vn/v-contract) |
| MISA eSign | Hỗ trợ USB Token và chữ ký số từ xa | Cần trang kiểm tra chứng thư/trạng thái ký dễ hiểu | [MISA](https://esign.misa.vn/4499/cach-ky-hop-dong-bang-chu-ky-so) |
| EFY-eCONTRACT | Ký số/OTP, CeCA, tích hợp ERP/HRM/CRM, phân quyền, lưu trữ | Cần audit trail, phân quyền và bản chứng thực; tách marketing claim khỏi căn cứ luật | [EFY](https://efy.com.vn/page/san-pham) |
| DocuSign | Tamper seal, audit trail đầy đủ, certificate of completion, xác thực danh tính và báo cáo | ECT Legal cần hiển thị “ai ký, ký lúc nào, bằng cách nào, nội dung nào” như một chuỗi chứng cứ | [DocuSign features](https://www.docusign.com/products/electronic-signature/features) |
| Adobe Acrobat Sign | Activity/audit report, template, bulk send, reminder, lưu agreement và audit trail | Nên tổ chức thư viện theo văn bản/phiên bản/sự kiện; về sau có thể thêm timeline chứng cứ | [Adobe Sign features](https://www.adobe.com/acrobat/business/features.html) |

## Cạnh tranh định vị

- Nhà cung cấp giải pháp tập trung vào **phát hành, ký, lưu trữ và chứng thực**.
- ECT Legal tập trung vào **lớp hiểu pháp lý độc lập**, liên kết đúng văn bản, điều khoản và trạng thái hiệu lực.
- Có thể tích hợp sau này nhưng không nên phụ thuộc một nhà cung cấp chữ ký số.

## Pattern UX rút ra

1. **Status-first:** mọi hồ sơ nên có trạng thái rõ (nháp, chờ ký, đã ký, từ chối, hết hạn), không để người dùng tự đoán.
2. **Audit-first:** lịch sử hành động, người thực hiện, thời gian và phương thức xác thực phải là đối tượng có thể tải xuống.
3. **Template-first:** mẫu hợp đồng và câu hỏi pháp lý lặp lại nên tái sử dụng được.
4. **Role-first:** HR, pháp chế, người ký và quản trị viên cần các màn hình khác nhau.
5. **Evidence-first:** với ECT Legal, mỗi kết luận phải dẫn tới điều luật và nguồn; không bắt chước kiểu “AI trả lời chung chung”.
