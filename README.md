# reflection_module2
# reflection 29/01/2021
https://github.com/ezreall/reflection_module2/blob/main/reflection.docx

# Reflection 28/01/2021 https://github.com/ezreall/reflection_module2/blob/main/bai4.xmind 
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
