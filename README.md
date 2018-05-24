# php_web_api
step 1 : clone source code </br>
  - clone source code về máy,đặt tại thư mục root của xamp. </br>
step 2 :  SETUP THE DATABASE </br>
  - sử dụng phpmyadmin, tạo database 'web_Api' </br>
  - sau đó chọn tệp users.sql import vào database 'web_Api'.  </br>
  - hoặc có thể chạy trực tiếp lệnh sql trong file users.sql ; </br>
step 3 : config môi trường </br>
  -mở file data_config.php </br>
  -sửa lại username và password của mysql cho chuẩn </br>
    [đoạn code sau : </br>
      private $host = "localhost"; </br>
      private $db_name = "web_Api"; </br>
      private $username = "root"; </br>
      private $password = " "; </br>
    ] </br>
step 4: chạy thử </br>
  - chạy xamp và start apache và mysql lên </br>
  - truy cập các linh sau trên trình duyệt để kiểm tra kết quả lấy thông tin người sử dụng.  </br>
    http://localhost/list.php </br>
    http://localhost/view.php?id=1 </br>
    chú ý : sửa localhost thành ServerName của bạn  </br>
  - sử dụng postman hoặc 1 tool nào đó ..... gửi 1 post request tới link sau để thực hiện new a recode </br>
    http://localhost/create.php với data là : </br>
      [ </br>
      "email" => "an12@gmail.com", </br>
      "name" => "an", </br>
      "address" => "ha noi", </br>
      "tel" => "0123743984" </br>
      ]
  - sử dụng postman hoặc 1 tool nào đó ..... gửi 1 post request tới link sau để thực hiện update: </br>
    http://localhost/update.php?id=1 với data là : </br>
      [ </br>
      "name" => "an", </br>
      "address" => "ha noi", </br>
      "tel" => "0123743984" </br>
      ]




