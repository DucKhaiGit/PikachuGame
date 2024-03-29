# BTL_JAVA
Giới thiệu chung về game 
![image](https://user-images.githubusercontent.com/131663358/235855636-e12da8d5-7878-4237-abb8-c67a80508b11.png)


- Giao diện chính của game: là 64 pokemon trong đó có với 16 loại pokemon khác nhau.
- New game: cho phép người chơi có thể bắt đầu một game mới.
- Score: là điểm số mà chúng ta đạt được khi tìm được các cặp hình 
giống nhau .Mỗi cặp hình giống nhau thì ta sẽ thu được 10 điểm 
công vào .
- Time : Chính là thanh thời gian chơi của chúng ta.Khi thanh thời 
gian chạy hết là lúc chúng ta hết thời gian chơi.

b) Mô tả cách chơi.
Để chơi game pikachu cổ điển rất đơn giản bạn chỉ cần sử dụng 
chuột và tìm ra các cặp thú giống nhau để loại bỏ khỏi màn hình 
trò chơi và ghi điểm.
Đồng hồ bấm giờ sẽ chạy khi bạn bắt đầu chơi, hãy tinh mắt và 
nhanh nhẹn để kết thúc trò chơi trước giờ nếu không bạn sẽ bị thua 
đấy.
Bạn chọn các cặp thú sao cho khi trên màn hình không còn hình 
thú nào nữa hết, như vậy bạn đã chiến thắng và chuyển qua màn 
hình chơi khác

- Code thuật toán của game.(Cotroller.java)
![image](https://user-images.githubusercontent.com/131663358/235857278-680cd51d-e875-433a-8a20-130a0ff52648.png)

Ta coi dao diện chính của game là một ma trận.
Ta có 21 hình ảnh khác nhau nên ta sẽ khai báo biến imgCount là 
21 .
Max = 4 là ta khai bao cho số ảnh giống nhau trong ma trận tối 
thiếu là 4
Int arr là để khai bao giá trị ban đầu của mỗi ảnh đều bằng 0.
Sau đó ta dùng ArrayList để lưu các listPoint vào trong Point bằng 
hai vòng lặp for.
![image](https://user-images.githubusercontent.com/131663358/235857470-3fcaf97b-6e47-4429-a9e8-d39a5e1db463.png)

Ta khai báo một biến i đại diện cho số cặp pikachu giống nhau .Ta 
dùng biến index để lấy giá trị ngẫu nhiên của 1 trong 21 ảnh khác 
nhau.Trong vòng lặp if ta có phép so sánh để so sánh số hình 
piakchu giống nhau tối thiểu trong một giao diện game.
 nếu nhỏ hơn max thì ta cộng thêm 2 vào biến 
arr.![image](https://user-images.githubusercontent.com/131663358/235857637-a5060d27-34f2-457a-a53e-ee16fafa2ec2.png)

Vòng lặp for để tạo ra hai cặp pikachu giống nhau trong 1 ma trận để tạo ra một biến mới lưu về kích thước của list.
![image](https://user-images.githubusercontent.com/131663358/235857734-e97e275f-9074-4f41-bbf1-99595641786f.png)

để tạo ra một biến mới lấy giá 
trị ngẫu nhiên trong khoảng từ 0 đến size -1.
lúc nãy sẽ lưu điểm có tọa độ x,y trên ma trận là index (mục đích 
để chọn hình ảnh đã lưu ở trên).
loại bỏ điểm này khỏi listP để tránh 
lần lấy PointIndex sau sẽ trùng số lần trước lưu giá trị.
While để kiểm tra i là số cặp pikachu trung nhau nên ta chỉ cho 
giới hạn chúng chạy tới đó.
dùng để kiếm tra 
hai biến pikachu có giống nhau không.
- Code nhận thông tin về các click chuột trên các button và xử lý 
theo hàm đã xây dựng (ButtonEvent.java).
- Code kiểm tra các cặp giống nhau (PointLine.java).
}
III) HƯỚNG PHÁT TRIỂN GAME.
- Chúng ta có thể thiết kế thuật toán làm sao cho khi ta chọn hai hình 
nhân vật hoạt hình giống nhau thì nó sẽ hiện đường đi của hai hình 
đó.
- Chúng ta có thể mở rộng kích thước chơi của game thành các cỡ
ma trận lớn hơn để thêm độ khó cho game và tăng mức điểm của 
game lên.
