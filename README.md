##tuan2
mysql  -u laptrinh -p123456;
show databases;
== sau moi cau lenh phai co dau phay;
xoa bo du lieu:     drop database "ten can xoa trong show databases";
create database "ten mysql can khoi phuc";
----- drop ><create---- xóa và khôi phục


THIET KE CO SO DU LIEU;
hệ quản trị cơ sở dữ liệu nó tạo ra thành những bảng (table);: sao cho dữ liệu của các bảng này được liên kết với nhau.
sao cho khi thay đổi kiểu dữ liệu ở bảng này thay đổi thì dữ liệu bảng kia cũng bị thay đổi.
- có các kiểu dữ liệu khác nhau: vd int, auto..
	UNSIGNED: không bị âm
	zerofill: thêm số 0 vào cho nó cân bằng
	Unique: các thông tin phải khác biệt với các thông tin đã có
	not null: ô bắt buộc phải điền
	đặt khóa chính,
=============================
<div>
<ul> <b>các lệnh trong bảng ghi câu lệnh: </b>
  <li>. không nên dùng tài khoản và mật khẩu mặc định của mysql làm (tạo bảng và sử lí vì
        tất cả các tables có thể bị sử dụng không lấy lại được, chỉnh sửa lại nhiều, hoạc dữ liệu không được bảo vệ);
-      mặc định: mysql -u root -p (thuong o day khong co pass nen bam enter:)
	    + đầu tiên cần tạo 1 database:  create database tên;
	    + Sau khi vào cần tạo một tài khoản mới để bảo vệ dữ liệu thông tin của một bảng nào đó.
    	cách tạo: grant all privileges on tên.* to  tendangnhap@localhost identifid by 'password'
      ==> show databases; lên xem các dữ liệu trên các bảng:
      sau bước này ta đã có 1 kho để lưu trữ dữ liệu

  <li>. cách tạo bảng trong mysql
      THIET KE CO SO DU LIEU; 
      làm trên phpmyadmin;
      b1: đăng nhập vào table
      >show databases;
      >use tên; vào tên bảng
      >show tables; hiển thị trong bảng đó 
      > show create table tenbangcanmo;
      để chỉnh sửa : create table 'tên' ... có trong phpmyadmin
  <li>. xử xí nhập và truy xuất dữ liệu.
      insert into bảng(các giá trị cần thêm)
         value = giá trị;
     select * from tên bảng
  </div>
