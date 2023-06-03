Lập trình hướng đối tượng (OOP - Object Oriented Programming) là một phương pháp lập trình được sử dụng rộng rãi, trong đó bạn tập trung vào các "đối tượng" để thực hiện các công việc.

Khởi động trước khi tìm hiểu

Trong Python, đối tượng là một thực thể mà bạn có thể áp dụng các hành động (phương thức) và lưu trữ dữ liệu (thuộc tính). Đối tượng được tạo từ một "lớp" (class), có thể coi như là một khuôn mẫu, mô tả các hành động và dữ liệu mà đối tượng của nó có thể làm.

Để minh họa cho OOP, hãy tưởng tượng một lớp tên là "Dog". "Dog" ở đây là một lớp.

class Dog:
    def __init__(self, name, age):
    
        self.name = name
        self.age = age

    def bark(self):
        print("Woof!")

Trong đó:

__init__ là một phương thức đặc biệt được gọi là "hàm khởi tạo" dùng để khởi tạo đối tượng. Khi bạn tạo một đối tượng mới từ lớp, Python sẽ tự động gọi phương thức này.
self là một tham chiếu đến đối tượng hiện tại, và được sử dụng để truy cập các thuộc tính của đối tượng.
name và age là thuộc tính của lớp Dog. Chúng lưu trữ dữ liệu liên quan đến đối tượng.
bark là một phương thức của lớp Dog. Phương thức là một hàm được định nghĩa trong lớp và có thể thực hiện các hành động liên quan đến đối tượng.
Giờ, bạn có thể tạo ra một đối tượng "Dog" như sau:

my_dog = Dog("Fido", 3)
Ở đây, my_dog là một đối tượng của lớp "Dog". Bạn có thể truy cập các thuộc tính của nó và gọi các phương thức như sau:

print(my_dog.name) # In ra: Fido
print(my_dog.age)  # In ra: 3
my_dog.bark()      # In ra: Woof!

Tham khảo thêm

![Sơ đồ hình dung OOP](https://pynative.com/wp-content/uploads/2021/08/class_and_objects.jpg)

Trên đây là một ví dụ đơn giản về lập trình hướng đối tượng trong Python. Có rất nhiều khái niệm phức tạp hơn như tính kế thừa, đa hình, đóng gói, v.v., nhưng hy vọng rằng ví dụ trên đã giúp bạn hiểu cơ bản về cách lập trình hướng đối tượng hoạt động trong Python.
Trong Python, Danh sách (List), Tuple, Từ điển (Dictionary) và các lớp tùy chỉnh (đối tượng) đều là các loại cấu trúc dữ liệu quan trọng. Dưới đây là mối liên hệ giữa chúng:

Danh sách (List) và Tuple: Danh sách và Tuple đều là các cấu trúc dữ liệu có thứ tự, tức là các phần tử được đánh dấu vị trí bằng chỉ số. Sự khác biệt chính là danh sách có thể thay đổi (mutable), trong khi Tuple không thể thay đổi (immutable).

Danh sách (List), Tuple và Từ điển (Dictionary): Tất cả đều có thể chứa nhiều phần tử. Nhưng khi cần truy cập các phần tử, danh sách và tuple sử dụng chỉ số (index), trong khi từ điển sử dụng khóa (key). Từ điển còn có thể được hiểu như là một tập hợp các cặp khóa - giá trị, trong khi danh sách và tuple chỉ chứa các giá trị đơn lẻ.

Các đối tượng và cấu trúc dữ liệu khác: Các đối tượng trong Python được tạo từ các lớp (classes), và chúng có thể chứa các thuộc tính và phương thức. Các thuộc tính có thể là bất kỳ loại dữ liệu nào, bao gồm danh sách, tuple và từ điển. Điều này tạo nên mối liên hệ chính giữa các đối tượng và các cấu trúc dữ liệu khác.

Ví dụ, bạn có thể tạo một lớp "Person" với thuộc tính "name" là một chuỗi (string), "age" là một số nguyên (integer), và "friends" là một danh sách chứa các đối tượng khác của lớp "Person".

Tóm lại, mỗi loại cấu trúc dữ liệu này có những đặc điểm riêng, nhưng cũng có mối liên hệ chặt chẽ với nhau thông qua cách chúng được sử dụng để lưu trữ và quản lý dữ liệu trong Python.
