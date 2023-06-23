# Bài tập lớn số 3 - Nhập môn khoa học dữ liệu - Nhóm 2 - Lớp NMKHDL.1_K3N2_2223

## Thành viên

| Thành viên               | Phân công công việc                       | Mức độ hoàn thành |
| ------------------------ | ----------------------------------------- | ----------------- |
| A42718 - Lê Thảo Quyên   | Thực hiện Bản dịch Tiếng Việt             | 100%              |
| A41316 - Nguyễn Hữu Khoa | Thực hiện ghi chép và chuyển đổi mã nguồn | 100%              |

## Các file báo cáo

1. [Bản dịch Tiếng Việt](chapter8_vi.pdf)

2. File mã nguồn được lưu trong thư mục [src](src/) gồm:
   - [python2](src/python2/): là file mã nguồn gốc được lấy từ sách
   - [python3](src/python3/): là file mã nguồn đã được chuyển đổi cú pháp sang python3
     - [Data_Collection.ipynb](src/python3/Data_Collection.ipynb): Thu thập dữ liệu từ Reddit thông qua API của Reddit, sử dung thư viện PRAW và lưu trữ dữ liệu vào cơ sở dữ liệu bằng SQLite3.
     - [Data_Preparation_n_Analysis.ipynb](src/python3/Data_Preparation_n_Analysis.ipynb): Dữ liệu được chuẩn bị và đưa vào phân tích.
   - [graph](src/python3/graph/): là thư mục chứa các đồ thị được tạo ra từ dữ liệu thu thập được

3. Các thư viện Python sử dụng trong chương này:
   - **NLTK:** Xử lí ngôn ngữ tự nhiên
   - **PRAW:** Cho phép tải bài viết xuống từ Reddit
   - **SQLite3:** Cho phép tạo và lưu trữ data trong cơ sở dữ liệu 
   - **Matplotlib:** Đồ thị hóa dữ liệu

4. **Lưu ý:** Trong phần chuẩn bị dữ liệu, để có thể lấy được dữ liệu từ Reddit bạn cần sử dụng API của Reddit. Tuy nhiên bạn sẽ bị giới hạn 60 request/phút cho mỗi máy khách. Nếu muốn tăng giới hạn lên 600 request/phút bạn cần đăng kí token sử dụng OAuth2, gửi submit cũng như đợi xét duyệt.

## Hướng dẫn chạy chương trình

1. Tạo môi trường ảo bằng lệnh `python3 -m venv venv`
2. Kích hoạt môi trường ảo bằng lệnh `source venv/bin/activate`
3. Tải và cài đặt các thư viện cần thiết bằng lệnh `pip install -r requirements.txt`
4. Tải và cài đặt MySQL
5. Tạo database `reddit` trong MySQL
6. Chạy mã nguồn theo thứ tự:
   -  `Data_Collection.ipynb`
   -  `Data_Preparation_n_Analysis.ipynb` 

## Cập nhật

Theo dõi Repo trên Github tại [đây](https://github.com/kztera/BTL-3-NMKHDL)

> Chương 8: Text mining and text analytics được lấy từ cuốn sách Introducing Data Science: Big Data, Machine Learning, and more, using Python tools của Davy Cielen, Arno D. B. Meysman, Mohamed Ali.