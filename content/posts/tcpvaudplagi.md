---
title: "TCP và UDP khác nhau như thế nào?"
date: 2025-10-11
description: "So sánh dễ hiểu giữa hai giao thức phổ biến trong lập trình mạng."
categories: ["Lập trình mạng"]
tags: ["TCP", "UDP"]
featured: true
---
<a id="TCP"></a>

#### Giao thức TCP (Tranmission Control Protocol) là gì?
![Google | TCP là gì?](images/whatistcp.png)
TCP là một giao thức mạng được dùng trong việc truyền gửi dữ liệu từ một mạng này đến một mạng khác. Một giao thức trong phạm vi mạng bao gồm những quy tắc và thứ tự quản lý quá trình truyền dữ liệu sao cho người dùng trên toàn cầu dù ở đâu, trên nền tảng gì, phần mềm nào cũng đều được phép thao tác theo cùng một phương thức tương tự nhau thì được gọi là TCP.
> Cùng một phương thức giao tiếp = TCP

Thường thì TCP sẽ liên kết với giao thức Internet (Internet Protocal hay IP) tạo thành một cặp gọi là TCP/IP. Thuật ngữ này hay xuất hiện ở mục network setting trên máy tính hay các thiết bị di động cá nhân (Network Settings). IP có nhiệm vụ gán địa chỉ thực hiện đưa những gói tin từ nguồn đến đích, còn TCP xác thực tính tin cậy của truyền dẫn.
![Network settings](images/networksettings.png)

#### Giao thức UDP (User Datagram Protocol) là gì?
UDP được định nghĩa là giao thức dữ liệu người dùng, đây là giao thức giao tiếp thay thế cho giao thức mạng truyền dữ liệu [TCP](#TCP), UDP được áp dụng vào việc tùy chỉnh, cài đặt những kết nối có độ trễ thấp và không chịu lỗi giữa các ứng dụng ở môi trường internet.
>![UDP | source: https://vietnix.vn/udp-va-tcp](images/giao-thuc-udp.png)

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
