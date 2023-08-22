# git_tutorial
create a new repository on the command line
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/hungnp196/fast_html.git
git push -u origin main
or push an existing repository from the command line
git remote add origin https://github.com/hungnp196/fast_html.git
git branch -M main
git push -u origin main

#     HƯỚNG DẪN CƠ BẢN SỬ DỤNG GIT           #

### CÀI ĐẶT ###
	
	- Có thể sử dụng 2 phiên bản là CLI và GUI để dùng
	link tải : 
		https://git-scm.com/downloads  (CLI)
		https://git-scm.com/downloads/guis  (GUI)

### SỬ DỤNG ###

	1 trong 2 trang Git cơ bản nhất là Bitbucket.org và Github.com
		Bitbucket.org cho phép tạo Repository Private và Public free
		Github.com chỉ cho phép tạo Repository Private nếu trả phí và free cho Public

	1. Tạo mới Repository
		Cả Bitbucket và Github đều có giao diện tạo mới gần giống nhau, chỉ cần điền tên là đủ, Bitbucket thì có thể chuyển đổi dạng Public/Private tùy ý.

### CÁC LỆNH CƠ BẢN ###
	2. Clone
		Bitbucket : lệnh clone có dạng sau khi vào repository: 

			git clone https://lamtacvu@bitbucket.org/lamtacvu/git_tutorial_all.git
			hoặc : 
			git clone git@bitbucket.org:lamtacvu/git_tutorial_all.git

		Github : link clone có dạng sau khi click vào nút "Clone or download"
			https://github.com/markwan314/repos-test-12.git
			hoặc
			git@github.com:markwan314/repos-test-12.git

		- Tạo mới 1 thư mục trên máy và vào thư mục đó
		- Click chuột phải chọn Gitbash here
		- Đối với lệnh clone của Bitbucket thì chỉ việc paste vào CLI còn Github thì phải gõ
			git clone <link repository>
		- enter

	3. commit

		Sau khi code xong 1 đoạn hoặc thay đổi cần phải commit để lưu thay đổi
		lệnh : 
				git commit -m "<tin nhắn sửa đổi>"
		- chú ý tin nhắn sửa đổi phải rõ ràng nêu ra được mình sửa những gì hay hoàn thiện phần nào
	4. pull

		Khi mà có nhiều người làm trên cùng 1 repository thì luôn cần phải update phiên bản làm việc trên máy của mình  
		lệnh : 
				git pull

	5. push
		Đẩy code lên Git với
		lệnh : 
				git push
		- chú ý : nếu như branch chưa có thì phải thêm -u origin master đằng sau
				nếu master muốn push lên các branch khác thì phải thêm tên branch đằng sau 
				ví dụ : git push <tên branch>

	6. add

		Khi mình thêm file mới vào git thì cần phải chạy để nhận biết việc thêm mới hoặc xóa
		lệnh : 

				git add .
			hoặc:
				git add <tên file>
	7. remote
		Khi muốn thay remote link cho repository
		lệnh :
				git remote set-url origin <link tới url repository>
	8. status
		Khi muốn xem các file nào vừa mới thay đổi trong repo
		lệnh: 
				git status
	9. diff
		Khi muốn so sánh code giữa các phiên bản hoặc giữa các file hoặc giữa các branch
		lệnh : 
				git diff
				git diff HEAD ./path/to/file
				git diff <tên branch>..<tên branch>
				git diff <tên commit> <tên commit>
	10. checkout
		Khi muốn khóa branch sử dụng mà không cho phép ai sử dụng nữa hoặc tạo branch mới
		lệnh: 
				git checkout <tên branch>

### TẠO PULL REQUEST ###
	Khi muốn master xem code của mình và ghép vào nhánh chính thì cần phải tạo pull request 
	Trình tự :
		- Sau khi commit và push lên branch của mình xong thì cần phải lên trang Github hoặc Bitbucket tạo pull request ở mục pull request
		- Ấn tạo mới và điền các thông tin yêu cầu là ghép code từ branch nào sang branch nào, tên tiêu đề 
		- Sau đó đợi master xét duyệt.


### TRÌNH TỰ LÀM VIỆC ###

	1. CLONE
	2. PULL
	3. CHECKOUT
	4. <update code>
	5. ADD
	6. COMMIT
	7. PUSH
	8. PULL request
	9. quay lại bước 2
