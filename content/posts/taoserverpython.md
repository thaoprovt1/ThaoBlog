---
title: "Cách tạo server đơn giản bằng Python"
date: 2025-10-11
description: "Hướng dẫn ngắn gọn cách viết server cơ bản bằng Python."
categories: ["Thực hành"]
tags: ["Python", "Socket"]
---

Tạo web server đơn giản chỉ vài dòng code thôi:

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