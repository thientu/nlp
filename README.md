# Thông tin sinh viên:
- Họ và tên: Trần Thiên Tứ
- MSSV: 1412633
- Source code được lưu trên tài khoản c9.io của em tại: https://ide.c9.io/thientu/natural-language-processing

**Lưu ý:** có thể đổi đuôi tệp này từ .txt sang .md rồi mở bằng markdown trên github để dễ nhìn hơn
#### Trong bài tập có sử dụng một số corpus của nltk nên nếu chạy lỗi do thiếu corpus thì có thể download bằng cách: *nltk.download()* rồi làm theo hướng dẫn.
Do nhiều corpus cần tải trong tất cả cả bài tập nên em không nhớ hết tên các corpus mà em đã tải.
#### Một số vấn đề em gặp phải khi làm bài tập: *Có ích cho những bạn khác đọc sách và thử code*
1. Các hàm sách in bị sai:
  - **nltk.edit_dist** trang 424: hàm đúng là **nltk.edit_distance**
  - **nltk.ibigrams()** trang 429, in dư chữ i: hàm đúng là **nltk.bigrams()** 
2. Do phiên bản nltk em dùng là *3.2.1*, còn phiên bản trong sách là *2.0.4* nên có một số thay đổi:
  - Hàm **nltk.clean_html()** không dùng được. Thay vào đó em dùng **BeautifulSoup** với hàm **get_text()**
  - **ElementTree** trong phiên bản 3.2.1 không còn nên em dùng **ElementTree** của module **xml**
  - Để cài BeautifulSoup có thể tham khảo trên trang chủ của BeautifulSoup nếu gặp vấn đề khi cài bằng lệnh sau: **pip install beautifulsoup4**

# Chi tiết các bài tập:

**Bài 1**

Bỏ dấu comment (#) để coi kết quả. *Có thể xem ở bài 2*

**Bài 3**

Sửa tập *legal_pos* (tập các từ loại hợp lệ) và file *dic.html* để kiểm tra kết quả

**Bài 4**

Sử dụng luôn rotokas dic để tìm số lượng pos nhỏ hơn 10

**Bài 5**

Xóa dấu comment rồi chạy code để xem kết quả. Hàm này chèn \cv ngay sau \lx.

**Bài 6**

Tương tự bài 5. Khác ở chỗ tính toán số lượng âm tiết. Hàm này dùng dictionary trong corpus của nltk để tính.
Các từ so khớp được trong từ điển sẽ cho kết quả đúng.
Tuy nhiên, rotokas.dic không phải tiếng anh nên kết quả không tính được số âm tiết do không trùng với từ điển tiếng anh.
Có thể thay rotoks.dic bằng tiếng anh để có kết quả chính xác.

**Bài 7**

Trong bài này mặc định dùng rotokas.dic nên biến *word* mặc định là *kaa*.
Có thể thay thế *word* thành một từ trong rotokas.dic để xem kết quả.
Hoặc thay thế rotokas.dic bởi từ điển khác và thay thể *word* cho phù hợp.

**Bài 8**

Bài này mặc định là lấy ra 10 cặp trường liên tục nhau nhiều nhất.
Có thể thay đổi 10 thành số tùy ý ở cuối dòng top10=....

**Bài 9**

Thay đổi file ex9.csv để xem kết quả khác.

**Bài 10**

Thay từ *music* ở dòng cuối để xem các kết quả cho các từ khác.

**Bài 11**

Sửa dòng cuối cùng nếu muốn xem các kết quả khác.

**Bài 12**

Bài này demo bằng cây của của tác phẩm merchant of venice của shakespears.
Có thể thay bằng cây khác để kiểm tra.
Kết quả chạy được lưu trong file ex12.txt

**Bài 13**

Thay đổi nội dung file comparative_wordlist.csv để xem các kết quả mong muốn.

**Bài 14**

Thay đổi nội dụng file ex14.csv rồi theo dõi kết quả trong file ex14.out.
