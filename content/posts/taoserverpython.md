---
title: "Cách tạo server đơn giản bằng Python"
date: 2025-10-11
description: "Hướng dẫn ngắn gọn cách viết server cơ bản bằng Python."
categories: ["Thực hành"]
tags: ["Python", "Socket"]
---

Bạn cần chia sẻ nhanh các file trong mạng nội bộ? Hay bạn là một lập trình viên web cần một cách siêu tốc để kiểm thử giao diện HTML, CSS, JavaScript của mình? Đừng vội nghĩ đến những thiết lập phức tạp hay những chương trình lớn. Với Python được cài đặt sẵn trên máy, bạn có thể khởi tạo một máy chủ web (web server) chỉ trong vài phút ngắn ngủi!.  
Hãy cùng khám phá module http.server có sẵn của Python nhé!

**Server này làm được gì?**  
Server đơn giản này chủ yếu dùng để phục vụ các file tĩnh. Điều này có nghĩa là bạn có thể:
- Truy cập và tải xuống bất kỳ file nào trong thư mục mà server được khởi chạy.
- Xem trước các trang web (HTML, CSS, JS) trực tiếp trên trình duyệt.
- Chia sẻ tài liệu, hình ảnh cho các máy tính khác trong cùng một mạng LAN.
```python
import socket

server = socket.socket()
server.bind(('localhost', 8080))
server.listen(1)

print("Server đang chạy...")
conn, addr = server.accept()
print(f"Kết nối từ {addr}")

data = conn.recv(1024)
print("Nhận:", data.decode())
conn.send(b"Hello client!")
conn.close()

```
Chạy xong, mở terminal khác gửi telnet localhost 8080 là thấy nó phản hồi liền !