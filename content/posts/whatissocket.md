---
title: "Lập trình socket là gì?"
date: 2025-10-11
description: "Giới thiệu khái niệm socket và cách dùng trong lập trình mạng."
categories: ["Lập trình mạng"]
tags: ["Socket", "Cơ bản"]
---

**Socket** giống như “đường dây” giữa hai chương trình để gửi và nhận dữ liệu.  

Ví dụ:
- Client (máy người dùng) gửi tin nhắn.
- Server nhận tin, xử lý, rồi phản hồi lại.

Trong code, bạn chỉ cần:
```python
import socket
s = socket.socket()
s.connect(('localhost', 8080))
s.send(b"Hello server")
```
thế là đã ping đến máy khác được r đó :D