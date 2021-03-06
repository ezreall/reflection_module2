# reflection_module2
### Bài tập Stack https://github.com/ezreall/Bai_tap_modul2.git
# reflection 4/02/2021
## Stack
Giống như một ngăn xếp <br>
Hoạt động theo nguyên lý Last-In-First-Out(Vào cuối ra trước) <br>
Có thể dùng Mảng hoặc là một linkedList để lưu trữ các phần tử<br>

### Các thao tác cơ bản của Stack
• push(): lưu giữ một phần tử trên ngăn xếp<br>
• pop (): Xoá một phần tử từ ngăn xếp<br>
• peek(): lấy phần tử dữ liệu ở trên cùng của ngăn xếp, mà không xóa phần tử này. <br>
• isEmpty(): Kiểm tra rỗng<br>
• isFull(): kiểm tra xem ngăn xếp đã đầy hay chưa.<br>

## Queue
Chỉ cho phép truy cập vào giá trị ở phía trước hàng đợi và lặp lại theo thứ tự đó, một cách triệt tiêu.<br>
Là một cấu trúc dữ liệu được sử dụng rộng rãi gồm một tập hợp các nút (rếng Anh: node) được liên kết với nhau theo quan hệ cha-con.<br>
Tuân theo phương pháp First-In-First-Out, tức là dữ liệu được nhập vào đầu tiên sẽ được truy cập đầu tiên.<br>
### Các thao tác cơ bản của Queue
• enqueue(): thêm (hay lưu trữ) một phần tử vào trong hàng đợi.<br>
• dequeue(): xóa một phần tử từ hàng đợi. • peek(): lấy phần tử ở đầu hàng đợi, mà không xóa phần tử này<br>
• isEmpty(): Kiểm tra rỗng<br>
• isFull(): kiểm tra xem hàng đợi đã đầy hay chưa.<br>

## Tree
Cấu trúc Tree đơn giản nhất đó là cấu trúc mà ở đó mỗi node chỉ có nhiều nhất là 2 node con, loại này thường được gọi là Cây nhị phân (binary tree)

### Cây nhị phân - Binay Tree
• Là cây rỗng hoặc là cây mà mỗi node có tối đa 2 node con<br>

### Cây nhị phân tìm kiếm - Binay Search Tree
 Phần tử ở node đó lớn hơn các phần tử ở cây con bên trái<br> 
 Nhỏ hơn các phần tử ở cây con bên phải<br>
 
 #### Hoạt động cơ bản trên cây tìm kiếm nhị phân
• Chèn: chèn một phần tử vào trong một cây/ tạo một cây.<br>
• Tìm kiếm: tìm kiếm một phần tử trong một cây.<br>
• Duyệt tiền thứ tự: duyệt một cây theo cách thức duyệt tiền thứ tự<br>
• Duyệt trung thứ tự: duyệt một cây theo cách thức duyệt trung thứ tự<br>
• Duyệt hậu thứ tự: duyệt một cây theo cách thức duyệt hậu thứ tự<br>
# reflection 3/02/2021
### ArrayList : 
là dùng một mảng động (như mảng thường nhưng có thể thay đổi kích thước và các phương thức thêm) để lưu trữ phần tử.<br>
### LinkedList : 
Sử dụng danh sách liên kết để lưu trữ phần tử. Mỗi phần thử có thể được gọi là 1 node trong danh sách.<br>


# Chúng khác nhau ở những đặc điểm sau:

1- Cách lưu trữ phần tử: Định nghĩa đã nêu rõ rồi đúng không nào<br>
2- ArrayList thêm và xóa phần tử chậm hơn LinkedList: Điều này khá dễ hiểu vì LinkedList chỉ cần thay đổi luồng trỏ của các node trong danh sách nên độ phức tạp là O(1) còn ArrayList phải tăng/lùi tất cả những vị trí sau vị trí muốn thêm/xóa nên độ phức tạp là O(n).<br>
3- ArrayList truy xuất phần tử nhanh hơn LinkedList: ArrayList muốn truy xuất đến phân tử thứ mấy trong danh sách thì chỉ cần gọi vị trí đó ra là được nên mất O(1) phức tạp, còn LinkedList thì phải duyệt qua các phần tử trước đó thì mới truy xuất được đến phần tử cần lấy nên độ phức tạp là O(n)<br>
4- ArrayList chỉ có thể hoạt động như 1 list thông thường, còn LinkedList có thể hoạt động như ArrayList, stack, queue. (stack và queue mình sẽ nói đến ở bài blog khác nhé)<br>
5- ArrayList yêu cầu ít bộ nhớ hơn LinkedList: Vì ngoài lưu trữ giá trị thì các node trong LinkedList còn phải chứa các tham chiếu đến phần tử trước, sau của nó nữa.


# reflection 2/02/2021

# Các đặc điểm của clean code:
• Đơn giản<br>• Trực tiếp <br>• Dễ đọc<br>• Dễ cải tiến<br> • Có unit test và acceptance test<br>• Các định danh đều thể hiện rõ nghĩa<br>• Có ít sự phụ thuộc<br>• Không có mã bị trùng lặp (duplicate)<br>• Thể hiện được ý tưởng của thiết kế<br>
## Mã nguồn nhằm mục đích chính:
<br>• Mã nguồn dễ duy trì hơn
<br>• Mã nguồn dễ mở rộng hơn
## Các cách thực hành clean code.
Áp dụng coding conventions trong việc đặt tên (biến, hàm, class), số lượng (dòng trong một hàm, số kí tự trong một dòng, số hàm trong một class,..)sử dụng comment, thực hiện xuống dòng..<br>
Sử dụng nguyên lý SOLID.<br>
Sử dụng Seperation of Concern và các mô hình phổ biến như MVC, MVVM để phân tách code thành nhiều thành phần nhỏ, dễ quản lý.
Áp dụng design pattern để giải quyết các vấn đề trong code.
## SOLID
Hiểu một cách đơn giản SOLID là 5 nguyên lý giúp lập trình viên phát triền phần mềm với kiến trúc tốt<br>
S đại diện cho SRP (Single responsibility principle<br>
O đại diện cho OCP (Open closed principle)<br>
L đại diện cho LSP (Liskov substitution principle)<br>
I đại diện cho ISP ( Interface segregation principle)<br>
D đại diện cho DIP ( Dependency inversion principle)<br>

## Refactoring.
Là việc thay đổi cấu trúc bên trong mà không làm thay đổi hành vi với bên ngoài hệ thống<br>
Refactoring có thể thực hiện ở nhiều mức độ<br>
Hệ thống -> Chức năng -> File/Class -> Method/Functions<br>
Tùy theo những mức độ này thì "cấu trúc bên trong" "hành vi bên ngoài" "hệ thống" sẽ được hiểu khác nhau.Ví dụ khi refactoring 1 class thì cấu trúc bên trong là properties, method của class đó hành vi bên ngoài là các nhiệm vụ mà class đó thực hiện.Như vậy refactoring khi đó là viết lại properties, method sao cho không làm thay đổi các nhiệm vụ của class đó
# Tại sao phải refactoring code
Refactoring không hề làm hệ thống chạy nhanh hơn, bảo mật hơn tuy nhiên nó sẽ giúp source code dễ tiếp cận, dễ đọc, dễ hiểu từ đó giúp ích rất nhiều cho quá trình bảo trì, mở rộng hệ thống.
# Khi nào thì thực hiện refactoring
Bất cứ khi nào bạn muốn đoạn code của mình "tốt hơn" thì đều có thể thực hiện refactoring. Tuy nhiên một số giai đoạn dưới đây được cho là thích hợp hơn để làm refactoring
# reflection 1/02/2021
https://github.com/ezreall/reflection_module2/blob/main/Abstract%20va%CC%80%20interface.docx
# reflection 29/01/2021
https://github.com/ezreall/reflection_module2/blob/main/reflection.docx

# Reflection 28/01/2021
https://github.com/ezreall/reflection_module2/blob/main/bai4.xmind 
# Reflection 27/01/2021

Từ khoá class được sử dụng để khai báo lớp

Từ khoá new được sử dụng để khởi tạo đối tượng

Phương thức khởi tạo (constructor) là phương thức giúp khởi tạo các đốitượng

Các phương thức cho phép thay đổi giá trị của thuộc tính được gọi là setter, các phương thức cho phép lấy về giá trị của thuộc tính được gọi là getter

Access modifier là các từ khoá được sử dụng để quy định mức độ truy cập đến lớp và các thành phần của lớp

Các mức truy cập:

public: có thể truy cập từ bất cứ đâu

private: các phương thức và thuộc tính chỉ được phép truy xuất trong cùng một lớp

protected: các phương thức và thuộc tính được phép truy xuất trong cùng một lớp và ở các lớp con (kế thừa)

Từ khoá this được sử dụng để đại diện cho đối tượng hiện tại

Hàm tạo (constructor)

//• Dùng để tạo và khởi tạo các trạng thái ban đầu của đối tượng

//• Mặc định sẽ có một Hàm tạo không có đối số được thêm vào cho lớp.

//Có thể lựa chọn sử dụng các constructor khác nhau bằng cách truyền vào tham số khác nhau

__construct() vs __destruct()

// Để can thiệp vào quá trình khởi tạo đối tượng, chúng ta sử dụng hàm __construct()

//• Để can thiệp vào quá trình huỷ đối tượng, chúng ta sử dụng hàm __destruct()



# Reflection 26/01/2021

## include(),require() và require_once()
	Theo em hiểu thì các hàm include(), require() và require_once() đều được dùng để nhập vào mã lệnh có trong một tập tin khác
	Nên sử dụng require khi ứng dụng yêu cần phải nhập vào một tập tin mang tính chất bắt buộc. Nếu tập tin này không tồn tại PHP sẽ chấm dứt hoạt động của chương trình đang chạy và hiển thị lỗi E_COMPILE_ERROR.

	Sử dụng require_once khi file nhập vào là bắt buộc phải có và tập tin này chỉ nên được nhập vào một lần đầu tiên, nếu file này tiếp tục được nhập vào sau đó (sử dụng một trong ba hàm require, include hay require_once PHP sẽ bỏ qua việc nhập vào.
	
	Sử dụng include khi bạn muốn nhập vào tập tin không mang tính chất bắt buộc, có cũng được không có cũng không sao
	
## Duyệt mảng liên kết
	Cách phổ biến nhất là dùng lệnh foreach, có hai trường hợp mỗi lần lặp trích xuất ra giá trị phần tử và trích xuất cả giá trị và chỉ số index

	
	foreach ($bienmang as $value) {
    	var_dump($value);
	}

	// vòng lặp, lấy  giá trị  và chỉ số từng phần tử
	foreach ($bienmang as $key => $value) {
    	var_dump($key, $value);
	}

	Ví dụ:

	<?php
  	 	 $names = ["Nguyen", "Huy", "Thang"];
   		 foreach ($names as $k => $name)
  	  {
   		echo "chỉ số $k; giá trị $name", PHP_EOL;
 	   }
  	  /*
        chỉ số 0; giá trị Nguyen
        chỉ số 1; giá trị Huy
        chỉ số 2; giá trị Thang
  	  */
  	  foreach ($names as $name)
  	  {
   	     echo "$name ";
  	  }
  	 
  	  
 ## Tìm hiểu các chế độ debug
Debug là quá trình tìm kiếm ra lỗi hay nguyên nhân gây ra lỗi (bug ở đâu) để có hướng sửa lỗi (fix bug). 

Programmers chính là các công cụ sinh ra Bugs nhiều nhất vì họ lập trình. Và chính vì vậy, công cụ tốt nhất để gỡ bỏ bớt Bugs cũng chính là các Programmers

Production mode enable tất cả các tối ưu trong webpack. Bao gồm minified code, scope hoisting, tree-shaking và nhiều nữa

Warning Errors
Đây là lỗi cảnh báo và không dừng việc thực thi chương trình. Lý do chính cho các lỗi cảnh báo là bao gồm một file nào đó bị thiếu hoặc sử dụng tham số không chính xác trong một chức năng.
Developement mode chủ yếu tối ưu hóa tốc độ và không minified code để bạn dễ dàng làm việc

Trong PHP có nhiều loại lỗi khác nhau trong PHP nhưng về cơ bản nó chứa bốn loại lỗi chính sau đây và cùng mình tìm hiểu từng loại nhé.

Parse error or Syntax Error
Fatal Error
Warning Errors
Notice Error

Parse error or Syntax Error

Lỗi phân tích cú pháp hoặc lỗi cú pháp là loại lỗi được lập trình viên thực hiện trong code của chương trình, lỗi cú pháp được phát hiện ra khi chương trình thực hiện biên dịch code. Sau khi sửa lỗi cú pháp thì sẽ biên dịch code và thực thi nó. Lỗi phân tích cú pháp có thể được gây ra bởi các sai sót như bị thiếu dấu ngoặc kép, thiếu dấu ngoặc đơn, thiếu dấu ngoặc nhọn, thiếu dấu chấm phảy, ..v.v

Fatal Error

Đây là loại lỗi khi biên dịch code PHP và hiểu những gì mình viết, tuy nhiên nó nhận ra trong đó có một hàm không được khai báo. Điều này có nghĩa là hàm được gọi nhưng hàm đó lại không được định nghĩa. Và dừng thực thi chương trình

Warning Errors

Đây là lỗi cảnh báo và không dừng việc thực thi chương trình. Lý do chính cho các lỗi cảnh báo là bao gồm một file nào đó bị thiếu hoặc sử dụng tham số không chính xác trong một chức năng.

Notice Error

Đây là một lỗi giống như Warning Errors, tức là những lỗi nhỏ, không nghiêm trọng mà PHP gặp phải khi thực thi tập lệnh - ví dụ: truy cập vào một biến chưa được xác định. Theo mặc định, các lỗi như vậy hoàn toàn không được hiển thị cho người dùng - mặc dù hành vi mặc định có thể được thay đổi.
