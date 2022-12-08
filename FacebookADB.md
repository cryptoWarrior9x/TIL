## QUY TRÌNH QUẢN LÝ FANPAGE

### Các công việc phải làm trong 1 ngày:
- Sáng:
    - Tìm video (trước 9h có đủ 10-12vd để anh check)
    - Edit video
    - Điền link video lên google excel cho các bạn sub online (trước 11h30)
    - Share bài (7h45 - 8h45 - 9h45)
- Chiều
    - Tải video lên driver Theo từng ngày tương ứng
    - Check sub và chạy tool
    - Đăng bài lên page bật kiếm tiền (trong VPS)
    - Đăng bài lên page hệ thống

### 1. Tìm video
Yêu cầu video:
- Video dài dưới 6 phút
- Lượt xem cao
- Mới được tải lên (video càng mới càng hạn chế việc người khác lấy trước mình)
- Cảnh đầu hấp dẫn
Sau khi tìm được video:
- Check trùng video với những bạn làm cùng chủ đề
- Lấy link video cho lên google excel của mình
- Mỗi ngày tìm từ 10-12 video
- Trước 10h phải có video để anh check chất lượng
- Sau khi check, gửi link video vào google excel của bạn sub (Deadline trước 12h trưa)

LỖI THƯỜNG GẶP:
- Video dính nhiều chữ tiếng trung (thường là video về top những cái gì đó)
- Video giọng tự truyện chứ ko phải review
- Video cũ -> chỉ tìm video trong vòng 1 tháng đổ lại

### 2. Edit video
Sau khi chạy tool xong thì trong thư mục “Output” có các file âm thanh (.wav) và file video (.mp4)
Các bước edit:
- Vào camtasia
- Chỉnh khung hình về 1200x1200
- Import media: Tải lên video và âm thanh của video muốn edit
- Lấy độ dài của file âm thanh làm chuẩn (rê chuột vào thanh âm thanh để xem độ dài)
- Chọn thanh video, nhấn chuột phải -> add clip speed -> Điền duration bằng file âm thanh
- Chọn âm thanh nền phù hợp với từng video
- Chỉnh âm thanh nền 25%, âm lượng âm thanh video 150%
- Cắt và che những nơi có tiếng trung trong video (SUB, logo)
- Nếu làm phim thì chèn tiêu đề (Chú ý đổi ngôn ngữ tương ứng với từng quốc gia)
Xuất video:
- Vào file -> Batch production
- Chọn các file camtasia vừa mới edit
- Chọn Only upto 1080 (dòng thứ 3)
- Chọn thư mục lưu (bỏ tích ở Organization the pro...)

LỖI THƯỜNG GẶP:
- Hình ảnh lệch với âm thanh (cái này check những đoạn có âm thanh gốc xem đã chuẩn chưa)
- Chọn nhạc không phù hợp
- Khung hình không đổi về 1200x1200

### 3. Share Bài
Mỗi bạn sẽ có một vài con via được login trên máy tính để quản lý một số page hệ thống.
Page hệ thống thuộc về một nội dung cụ thể (rvcs mexico, rvcs philipine,...)
Hằng ngày vào share với khung giờ sau:
- Hệ thống mexico: Share ở khung giờ (7h45 - 8h45 - 9h45)
- Hệ thống việt nam: Share lúc 9h - 11h - 13h
Cách share:
- Vào page bật kiếm tiền đang làm để chọn video để share. lấy link video
- Mở chrome đang quản lý page hệ thống
- Vào link video vừa chọn.
- Nhấn share -> Share lên Trang (hoặc Tùy chọn khác -> Share lên trang) -> Chọn trang. Sau đó, nhấn share.
### 4. Check sub
Mở từng file aegisub và thêm video vào để check các ý sau:
- Thiếu sub
- Âm thanh gốc đã đúng chưa
- Check mấy câu cuối của sub xem thời gian sub có dài hơn thời gian video hay không?
- QUAN TRỌNG: THÔNG THƯỜNG NHIỀU DÒNG VỀ CƠ BẢN LÀ 1 CÂU NHƯNG KHÔNG ĐƯỢC GHÉP LẠI. NẾU PHÁT HIỆN THÌ CŨNG BÁO CHO SUB SỬA LẠI. ví dụ: dòng thứ 2: "Hôm nay" và dòng thứ 3: "tôi đi chơi". Về ngữ pháp 2 câu này là 1 câu thì phải ghép lại "Hôm nay, tôi đi chơi". Nếu phát hiện không ghép 2 dòng này lại thì phải nói lại sub để sửa.
LỖI THƯỜNG GẶP:
- Sub dài hơn video (check câu sub cuối xem có dài hơn thời gian kết thúc video ko)
- Thiếu sub

### 5. Chạy tool
Tải video và file sub về lưu ý những quy tắc sau:
- Tên không dấu
- Dấu cách đổi thành dấu "_"
- File sub có thêm hậu tố "-vi-vi"
- File video trùng tên với file sub nhưng không có "-vi-vi"
Các bước thực hiện:
- Tải hết file video và sub vào folder "Input"
- Đặt lại tên theo đúng quy tắc trên
- Đổi file .ass sang .srt bằng web https://sorz.github.io/asstosrt-wasm/
- Mở Pycharm (Phần mềm có biểu tượng PC) lên
- Điền vào video_list tên video và các ngôn ngữ muốn chạy. Ví dụ: 
	video_list = {
    	'rvcs_cuoc_duoi_bat_cua_chu_soc': ['es-mx', 'tl-tl', 'id-id', 'vi-vi'],
    	'rvcs_dan_nha_giau_dubai': ['es-mx', 'tl-tl', 'id-id', 'vi-vi'],
    }
- Nhấn chuột phải --> chọn Run "Main"

LỖI THƯỜNG GẶP:
- Điền sai tên ở video list
- Không đổi file ass sang srt
- Tên video không trùng với tên file sub (không tính đuôi -vi-vi)

### 6. Đăng bài lên page bật kiếm tiền
- Vào "Team Adb Offline" để xem những video nào muốn đăng
- Vào driver nơi lưu trữ những video đó và lấy link driver
- Vào vps đang quản lý
- Vào chrome "Tai video" và vào link vừa lấy ở bước trên để tải video.
- Sau khi tải xong,
- Chọn chrome của page muốn đăng
- Vào Studio sáng tạo (Thường lưu ở bookmask)
- Chọn page muốn đăng
- Vào phần "Đã đăng" hoặc "Published"
- Chọn "Create new" -> "Multiple video"
- Chọn tải lên video
- Chọn tất cả video muốn đăng
- Điền vào các mục sau:
	+ Tiêu đề
	+ Mô tả
	+ Thẻ Tag
	+ Ngôn ngữ: (Mexico - spanish; Việt nam - vietnamese; Philipine - Filipino; Indonesia - indonesia; Ấn Độ - hindi)
	+ Hình thu nhỏ: Chọn hình ấn tượng.
	+ Lên lịch đăng
		* Mexico: 6h 9h 12h 19h cùng ngày
		* Việt nam: 
- Chọn "Save change"
- Sau khi save change xong, vào lại "Pre-Published" để check lại xem video đã lên lịch chưa, thời gian lên lịch chuẩn chưa
- Ok hết rồi thì vào folder "Download" để xóa hết video vừa mới đăng để tránh nhầm lẫn và giảm bộ nhớ cho vps

LỖI THƯỜNG GẶP:
- QUÊN KHÔNG CHỌN NGÔN NGỮ
- Lên lịch sai giờ hoặc đôi lúc facebook bị lỗi (Cái này thì phải vào Pre-Published để kiểm tra sau mỗi khi lên lịch)
