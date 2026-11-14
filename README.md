# 🎮 Tetris – Giới thiệu và hướng dẫn chơi game

> Trò chơi xếp gạch kinh điển: luật chơi đơn giản, nhưng chơi giỏi thì không đơn giản chút nào.

## 📑 Mục lục

- [1. Giới thiệu tổng quan](#1-giới-thiệu-tổng-quan)
- [2. Hướng dẫn chơi](#2-hướng-dẫn-chơi)
- [3. Các chức năng chính của game](#3-các-chức-năng-chính-của-game)
- [4. Kết luận](#4-kết-luận)

---

## 1. Giới thiệu tổng quan

### 1.1. Tetris là game như thế nào?

Bạn đã bao giờ thử sắp xếp những khối hình liên tục rơi xuống màn hình sao cho không để lại bất kỳ khoảng trống nào? Tưởng chừng đơn giản, nhưng chỉ một vài quyết định thiếu tính toán cũng có thể khiến các khối hình nhanh chóng chất đống. Đó chính là thử thách mà Tetris mang đến cho người chơi.

**Tetris** (còn gọi là trò chơi xếp gạch, xếp hình) là một trong những trò chơi điện tử kinh điển và có sức ảnh hưởng lớn nhất trong lịch sử ngành game. Đây là game thuộc thể loại giải đố (puzzle), trong đó người chơi điều khiển các khối hình học rơi từ trên xuống, xoay và di chuyển chúng sao cho xếp thành những hàng ngang kín. Mỗi hàng hoàn chỉnh sẽ biến mất và mang về điểm số cho người chơi.

Không có cốt truyện phức tạp hay hệ thống nhân vật cầu kỳ, Tetris thu hút người chơi bằng những thao tác đơn giản nhưng đòi hỏi khả năng quan sát, tư duy logic và phản xạ nhanh. Mỗi khối hình xuất hiện đều đặt ra một lựa chọn mới: nên đặt ở đâu, xoay theo hướng nào và làm thế nào để chuẩn bị cho những khối tiếp theo. Vì vậy, ai cũng có thể làm quen với trò chơi chỉ sau vài phút, nhưng để đạt điểm số cao thì cần thời gian luyện tập.

### 1.2. Vì sao Tetris hấp dẫn?

- **Dễ học, khó thành thạo:** luật chơi chỉ gói gọn trong vài dòng, nhưng chiến thuật thì gần như vô tận.
- **Ván chơi ngắn, chơi ở đâu cũng được:** một ván có thể chỉ kéo dài vài phút, phù hợp để giải trí lúc rảnh rỗi.
- **Luôn có mục tiêu để phá kỷ lục:** càng chơi lâu, tốc độ rơi càng nhanh, khiến mỗi ván đều có cảm giác "thêm một lượt nữa".
- **Rèn luyện tư duy:** game giúp cải thiện khả năng quan sát, tính toán không gian và ra quyết định nhanh.
- **Phù hợp mọi lứa tuổi:** không có yếu tố bạo lực hay nội dung phức tạp, trẻ em và người lớn đều có thể chơi.


## 2. Hướng dẫn chơi

### 2.1. Mục tiêu của trò chơi

Nhiệm vụ của bạn rất đơn giản: sắp xếp các khối hình đang rơi xuống để lấp đầy các hàng ngang bên dưới. Khi một hàng được lấp kín, hàng đó tự động biến mất và bạn nhận được điểm. Hãy cố gắng xóa càng nhiều hàng càng tốt và duy trì ván chơi lâu nhất có thể.

Trò chơi kết thúc (**Game Over**) khi các khối hình chất chồng lên đến giới hạn phía trên, khiến khối mới không còn chỗ để xuất hiện.

### 2.2. Các loại khối hình

Tetris truyền thống có bảy loại khối hình cơ bản, gọi là **Tetromino**. Mỗi khối được ghép từ bốn ô vuông nhỏ và thường có màu sắc riêng để người chơi dễ nhận biết.

```text
 I      O     T      S      Z      J      L
████    ██    ███     ██    ██     █      ███
        ██     █     ██      ██    ███      █
```

| Khối | Hình dạng | Đặc điểm |
|:----:|-----------|----------|
| 🟦 **I** | Đường thẳng 4 ô | Đặt ngang hoặc dọc. Là khối quan trọng nhất để xóa 4 hàng cùng lúc. |
| 🟨 **O** | Hình vuông 2×2 | Không thay đổi hình dạng khi xoay. Phù hợp với chỗ trống rộng 2 ô. |
| 🟪 **T** | Hình chữ T | Xoay được theo 4 hướng, rất linh hoạt để lấp các khoảng trống. |
| 🟩 **S** | Hình chữ S | Thích hợp với những khu vực có bề mặt lệch bậc. |
| 🟥 **Z** | Hình chữ Z | Đối xứng với khối S, cũng dùng cho các chỗ lệch bậc. |
| 🔷 **J** | Hình chữ J | Đối xứng ngược với khối L, hay dùng để lấp góc hoặc chỗ lõm. |
| 🟧 **L** | Hình chữ L | Đối xứng ngược với khối J, hay dùng để lấp góc hoặc chỗ lõm. |

*Màu sắc có thể khác nhau tùy phiên bản.* Việc ghi nhớ hình dạng và cách xoay của từng khối sẽ giúp bạn chọn vị trí đặt nhanh và chính xác hơn.

### 2.3. Luật chơi cơ bản

- **Khối hình rơi từ phía trên:** các khối Tetromino lần lượt xuất hiện ở đầu khu vực chơi và rơi dần xuống theo thời gian.
- **Người chơi điều khiển khối đang rơi:** có thể di chuyển sang trái, sang phải, xoay khối hoặc cho khối rơi nhanh hơn để tìm vị trí thích hợp.
- **Lấp kín hàng ngang để ghi điểm:** khi một hàng đầy, hàng đó biến mất và các khối phía trên dịch xuống. Xóa nhiều hàng cùng lúc sẽ được nhiều điểm hơn.
- **Không để khối chạm giới hạn phía trên:** nếu các khối chồng quá cao và khối mới không còn chỗ xuất hiện, trò chơi kết thúc.

### 2.4. Hướng dẫn điều khiển

Trên máy tính, người chơi điều khiển bằng bàn phím. Trên điện thoại, các thao tác tương ứng là chạm hoặc vuốt trên màn hình: chạm để xoay khối, vuốt trái/phải để di chuyển và vuốt xuống để khối rơi nhanh hơn.

| Phím điều khiển | Chức năng |
|:---------------:|-----------|
| `←` | Di chuyển khối sang trái |
| `→` | Di chuyển khối sang phải |
| `↑` | Xoay khối |
| `↓` | Tăng tốc độ rơi của khối (soft drop) |
| `Space` | Thả khối rơi ngay xuống vị trí thấp nhất (hard drop) |
| `C` | Giữ lại khối hiện tại để dùng sau (Hold), nếu phiên bản hỗ trợ |
| `P` | Tạm dừng hoặc tiếp tục trò chơi, nếu phiên bản hỗ trợ |

### 2.5. Cách tính điểm và cấp độ

Điểm số phụ thuộc vào số hàng xóa được cùng lúc: xóa càng nhiều hàng một lượt, điểm thưởng càng cao. Con số dưới đây là điểm cơ bản theo cách tính của các phiên bản kinh điển (sẽ được nhân với hệ số theo cấp độ hiện tại), mỗi phiên bản có thể điều chỉnh khác đi.

| Số hàng xóa cùng lúc | Tên gọi thường dùng | Điểm cơ bản (tham khảo) |
|:--------------------:|:-------------------:|:-----------------------:|
| 1 hàng | Single | 40 |
| 2 hàng | Double | 100 |
| 3 hàng | Triple | 300 |
| 4 hàng | **Tetris** | 1200 |

Bên cạnh đó, cứ sau một số hàng nhất định (thường là 10 hàng), trò chơi sẽ lên một cấp độ (**Level**) mới. Cấp độ càng cao, khối rơi càng nhanh, thử thách càng lớn nhưng điểm thưởng cũng càng nhiều.

### 2.6. Quy trình bắt đầu một ván chơi

1. **Bắt đầu:** truy cập trò chơi và nhấn nút Start/Bắt đầu để khởi động.
2. **Quan sát:** xác định vị trí của khối hình đang xuất hiện, đồng thời xem trước khối tiếp theo.
3. **Điều khiển:** dùng các phím điều khiển để di chuyển hoặc xoay khối đến vị trí mong muốn.
4. **Thả khối:** chờ khối rơi xuống hoặc nhấn phím `Space` để thả khối nhanh hơn.
5. **Ghi điểm:** tiếp tục sắp xếp để hoàn thành các hàng ngang và tích lũy điểm số.
6. **Kiểm soát chiều cao:** theo dõi chiều cao của các khối đã xếp để tránh chạm giới hạn phía trên.

### 2.7. Một số mẹo chơi cơ bản

> 💡 **Mẹo nhanh:** chừa một cột trống thẳng đứng sát mép khu vực chơi để chờ khối I, rồi xóa bốn hàng cùng lúc.

- **Giữ bề mặt tương đối bằng phẳng:** hạn chế tạo ra những khoảng trống sâu hoặc chênh lệch quá lớn vì chúng gây khó khăn cho các khối tiếp theo.
- **Quan sát khối tiếp theo:** đừng chỉ tập trung vào khối đang rơi, hãy dự đoán khối sắp xuất hiện để chủ động sắp xếp.
- **Tránh tạo lỗ hổng bị che khuất:** những khoảng trống nằm dưới các khối khác có thể khiến bạn mất nhiều lượt để xử lý.
- **Sử dụng Hold hợp lý:** nếu có hỗ trợ, hãy giữ lại khối chưa phù hợp để dùng vào thời điểm thích hợp hơn.
- **Tận dụng khối I:** dành khối I cho những lúc có thể xóa nhiều hàng cùng lúc để ghi điểm cao.

---

## 3. Các chức năng chính của game

Dựa trên các phiên bản Tetris phổ biến, có thể chia các chức năng của game thành hai nhóm: **chức năng cơ bản** (bắt buộc phải có để game chơi được) và **chức năng nâng cao** (giúp game phong phú, hấp dẫn hơn).

### 3.1. Chức năng cơ bản

| Chức năng | Mô tả |
|-----------|-------|
| **Màn hình chính (Menu)** | Gồm các lựa chọn như Bắt đầu chơi, Hướng dẫn, Cài đặt và Thoát game. |
| **Khu vực chơi** | Một lưới hình chữ nhật (thường rộng 10 cột, cao 20 hàng) nơi các khối rơi và được xếp chồng lên nhau. |
| **Tạo khối ngẫu nhiên** | Liên tục sinh ra các khối trong bảy loại Tetromino để người chơi xử lý. |
| **Điều khiển khối** | Di chuyển trái/phải, xoay khối, tăng tốc rơi và thả rơi ngay xuống đáy. |
| **Xóa hàng và tính điểm** | Tự động phát hiện hàng đã đầy, xóa hàng đó, dồn các khối phía trên xuống và cộng điểm. |
| **Tăng cấp độ** | Cấp độ tăng theo số hàng đã xóa, đồng thời tốc độ rơi của khối nhanh dần. |
| **Bảng thông tin** | Hiển thị điểm hiện tại, cấp độ, số hàng đã xóa và khối sẽ xuất hiện tiếp theo (Next). |
| **Tạm dừng / tiếp tục** | Cho phép dừng ván chơi bất cứ lúc nào và quay lại chơi tiếp. |
| **Kết thúc và chơi lại** | Thông báo Game Over khi khối chạm giới hạn trên, hiển thị điểm đạt được và cho phép bắt đầu ván mới. |

### 3.2. Chức năng nâng cao

| Chức năng | Mô tả |
|-----------|-------|
| **Giữ khối (Hold)** | Cất khối hiện tại sang một ô riêng để dùng sau, hoặc đổi với khối đang được giữ. |
| **Khối bóng (Ghost piece)** | Hiển thị mờ vị trí khối sẽ rơi xuống, giúp người chơi đặt khối chính xác hơn. |
| **Xem trước nhiều khối** | Cho xem 3–5 khối tiếp theo thay vì chỉ một khối để lên kế hoạch xa hơn. |
| **Bảng điểm cao** | Lưu lại các điểm số tốt nhất để người chơi so sánh và phá kỷ lục của chính mình. |
| **Âm thanh và nhạc nền** | Nhạc nền, hiệu ứng khi xoay khối, xóa hàng và kết thúc ván; có thể bật/tắt trong phần cài đặt. |
| **Cài đặt tùy chỉnh** | Điều chỉnh âm lượng, đổi phím điều khiển, chọn giao diện hoặc màu sắc khối. |
| **Hiệu ứng hình ảnh** | Hiệu ứng khi xóa hàng, hiển thị combo hoặc cấp độ mới để tăng cảm giác sảng khoái. |
| **Nhiều chế độ chơi** | Ví dụ: **Marathon** (chơi đến khi thua), **Sprint** (xóa 40 hàng nhanh nhất có thể), **Ultra** (ghi điểm cao nhất trong thời gian giới hạn). |

---

