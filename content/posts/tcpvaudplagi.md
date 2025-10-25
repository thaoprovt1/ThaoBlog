---
title: "TCP và UDP khác nhau như thế nào?"
date: 2025-10-11
description: "So sánh dễ hiểu giữa hai giao thức phổ biến trong lập trình mạng."
categories: ["Lập trình mạng"]
tags: ["TCP", "UDP"]
---

TCP và UDP đều dùng để gửi dữ liệu qua mạng, nhưng cách hoạt động thì khác nhau hoàn toàn.

| TCP | UDP |
|-----|-----|
| Có kết nối (connection) | Không cần kết nối |
| Đảm bảo dữ liệu đến nơi | Không đảm bảo |
| Gửi chậm hơn nhưng an toàn | Gửi nhanh, không cần kiểm tra |
| Dùng trong web, email | Dùng trong game, stream, VoIP |

Tóm lại:  
- Cần **chính xác** → dùng **TCP**  
- Cần **tốc độ** → dùng **UDP**
