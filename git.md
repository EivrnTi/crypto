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


## file .git ignore quy định những thư mục hay file không được phép đẩy lên repo remote
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
## working dictionary (file màu đỏ)

## staging (file màu xanh)
=> Lúc này file đã sẵn sàng để đưa lên repo remote

## config git (chỉ chzy5 duy nhất 1 lần)
## git config --global user.name "Your Name"
## git config --global user.email "you@example.com"

## git commit -m "message"
=> Dùng để gắn message vào trong những file đang ở staging được phép đưa lên repo remote
=> Mỗi commit có một mã sha (id)

## git log
=> Kiểm tra lịch sử commit

## git push -u origin <tên nhánh>
=> Đưa code lên repo remote
=> Từ lần push code thứ 2 : git push

## git reset
=> Đưa file từ stagin về lại working

## git restore -S .
=> Đưa tất cả các file đang ở staging về working

## git restore -S <url file>
=> Chỉ đưa duy nhất file về working

## git checkout
=> 1. Đưa 1 cái file đang được chỉnh sửa về trạng thái trước đó

## git checkout -b <tên nhánh>
=> tương đương với 2 lệnh git branch + git switch

## git checkout <tên nhánh>
=> tương đương với lệnh git switch
=> Dùng d963 chuyển qua <tên nhánh>

## branch

// => dev => kiểm tra thử QA và DEV (dev)

// => staging => QA kiểm thử lần 1 (staging)

// production => end user (main/release)

## git branch <tên nhánh>
=> tạo ra 1 nhánh mới
=> nhánh mới sẽ chứa toàn bộ code của nhánh đang đứng

## git branch -a or git branch
=> Liệt kê tất cả các branch đang có ở trong repo

## git switch <tên nhánh>
=> Chuyển qua nhánh <tên nhánh>

## git pull or git pull --no-ff
=> pull code ở repo remote về local


## git clone <url repo>
=> Dùng để clone source code của 1 repo bất kỳ

## git merge <tên branch>
=> merge <branch> vào branch hiện tại
+ TH1: merge thành công nếu không có bất kỳ xung đột (conflict)
+ TH2: bị xung đột => giải quyết conflict => git add => git commit
=> Nếu mege code mà bị conflict => có thể hủy git merge thông qua lệnh: git merge -abort


