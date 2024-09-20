## Tạo repsitory (repo)

git init
=> nhánh chính: master

## git int -b main

=> Tạo repo local vs nhánh chính có tên main

## git remote add origin + <url repo>

=> Liên kết repo local vs repo remote

## Không đưa thư mục node_modules lên repo remote

=> node_modules chiếm dung lượng rất lớn
=> node_modules có thể cài lại thông qua câu lệnh : npm i


## file .gitignore quy định những thư mục hay file không được phép đẩy lên repo remote
=> .gitignore nằm ở thư mục root

## git status
=> Kiểm tra sự thay đổi của các file trong dự án


## git add
=> Thêm mỗi file vào trong staging

## git add . 
=> Dùng để thêm tất cả các file ở trong thư mục hiện tại vào trong staging

## git add - A 
=> Dùng để thêm tất cả các file ở trong dự án vào trong staging

## git add <đường dẫn file>
=> Chỉ thêm file cụ thể vào trong staging


## demo git confict