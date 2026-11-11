# EduSubmit – Bài 1

Yêu cầu .NET 10 SDK. Hai project độc lập, giao tiếp qua HTTP/JSON.
Mở terminal tại thư mục có `EduSubmit.slnx`.

```powershell
dotnet build
# Terminal 1
dotnet run --project src/Submission.Api --urls http://localhost:5000
# Terminal 2
dotnet run --project src/Submission.Client -- http://localhost:5000
```

Mở `requests.http` bằng REST Client. Chạy request `createSubmission` trước request
đọc lại để lấy ID tự động. API lưu dữ liệu trong RAM: khởi động lại sẽ mất các lượt nộp.
Client chạy lại sẽ tạo GUID mới. Đổi cổng bằng tham số dòng lệnh và biến `@api`.

Đã điền thông tin Lê Hải Anh, DTC245200851, CNTT K23E và repository thật. Trước khi nộp, kiểm tra thông tin
trong `docs/bai1.md`, bổ sung ảnh theo `docs/CHUP-ANH.md`.
Code được hỗ trợ viết bằng Codex; cần tự đọc, chạy lại và thực hành debug theo đề.

Repository đã được tạo và kết nối: https://github.com/dtc245200851/BAI1_PTUDPT.
Sau khi hoàn thiện ảnh và nhật ký, chạy tại thư mục này:

```powershell
git add .
git commit -m "Bai 1: API, Client, mo rong va nhat ky thuc hanh"
git tag bai1
git push -u origin main --tags
```

Chỉ gắn tag sau khi đã bổ sung ảnh để tag chứa đầy đủ bài nộp.


## Bài 2 — Catalog API

Mã nguồn, client, request kiểm tra và hướng dẫn chạy: [Bai2_/CataLogApi](Bai2_/CataLogApi/README.md). Tag: `bai2`.
