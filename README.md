# Chuyển File An Toàn

Ứng dụng web giúp ký số và xác minh chữ ký số cho file bằng RSA, giao diện hiện đại, dễ sử dụng.

## Tính năng

- **Tạo cặp khóa RSA**: Tạo và tải về private key & public key (dạng `.pem`).
- **Ký file**: Ký số file bất kỳ bằng private key, tải về file chữ ký `.sig`.
- **Xác minh chữ ký**: Kiểm tra tính toàn vẹn file với public key và file chữ ký.

## Hướng dẫn cài đặt

1. **Clone dự án**
    ```sh
    git clone <link-repo>
    cd secure_file_transfer
    ```

2. **Cài đặt thư viện**
    ```sh
    pip install -r requirements.txt
    ```

3. **Chạy ứng dụng**
    ```sh
    python app.py
    ```

4. **Truy cập**
    - Mở trình duyệt và vào địa chỉ: [http://127.0.0.1:5000](http://127.0.0.1:5000)

## Hướng dẫn sử dụng

- **Tạo cặp khóa RSA**  
  Nhấn nút **Tạo & tải về cặp khóa RSA** để tải về file zip chứa private key và public key.

- **Ký file**  
  Chọn file cần ký, nhấn **Ký file** để tải về file chữ ký `.sig`.

- **Xác minh chữ ký**  
  Chọn file gốc, file chữ ký `.sig` và public key `.pem`, nhấn **Xác minh chữ ký** để kiểm tra kết quả.

## Cấu trúc thư mục

```
secure_file_transfer/
│
├── app.py
├── requirements.txt
├── keys/
├── uploads/
└── templates/
    ├── index.html
    ├── sign.html
    ├── verify.html
    └── result.html
```

## Công nghệ sử dụng

- Python 3
- Flask
- cryptography
- Bootstrap 4, Animate.css, FontAwesome

---

**Tác giả:**  
- [Dương Huy Hoàng - CNTT 17-07]
![image](https://github.com/user-attachments/assets/35deea3d-f5aa-4515-a36f-08324b6f88d3)
