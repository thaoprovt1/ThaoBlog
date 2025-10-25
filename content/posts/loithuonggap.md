---
title: "Khi lập trình mạng, lỗi hay gặp nhất là gì?"
date: 2025-10-11
description: "Tổng hợp những lỗi sinh viên thường gặp khi học lập trình mạng."
categories: ["Lập trình mạng"]
tags: ["Lỗi", "Debug"]
---

Một vài lỗi “kinh điển” ai học cũng gặp:

- Sai **địa chỉ IP** hoặc **port**.
- Không **đóng kết nối** sau khi gửi xong.
- Quên **encode/decode** khi truyền chuỗi.
- Cố “send” dữ liệu khi server chưa sẵn sàng 😅

Giải pháp:
1. In log từng bước.
2. Dùng Wireshark hoặc netcat để kiểm tra.
3. Bình tĩnh, không hoảng 😤