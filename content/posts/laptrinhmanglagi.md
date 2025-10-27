---
title: "Lập trình mạng là gì?"
date: 2025-10-23
description: "Giải thích khái niệm lập trình mạng một cách dễ hiểu cho sinh viên công nghệ."
categories: ["Lập trình mạng"]
tags: ["Networking", "Cơ bản"]
featured: true
---

Nghe “lập trình mạng” thì nhiều người sẽ nghĩ ngay tới hacker, ddos, server game hay mấy dòng lệnh đen thui gì gì đó trên màn hình.
Nhưng thật ra **lập trình mạng** chỉ đơn giản là việc lập trình có liên quan đến **giao tiếp giữa các máy tính qua mạng** và việc lựa chọn ngôn ngữ lập trình phù hợp với bản thân.

Đối với mạng, có 4 loại mạng cơ bản là: LAN, MAN, WAN, PAN. 
![Ảnh mạng](images/manglagi.png)

- **Mạng LAN (Local Area Network)**

Mạng LAN là mạng cục bộ nên có đường truyền ngắn. Với giao thức TCP/IP, mạng LAN chủ yếu được sử dụng tại nơi diện tích nhỏ như: văn phòng, tòa nhà, trường học.

Tất cả máy tính kết nối mạng LAN đều được sử dụng để kết nối vào máy chủ sau đó chờ quyền truy cập để thực hiện lệnh in trên máy in. 

- **Mạng MAN (Metropolitan Area Network)**

Khác với mạng LAN, mạng đô thị MAN có phạm vị kết nối rộng hơn, hình thành nhờ sự kết nối nhiều mạng LAN với nhau. 

Đây là mô hình rộng cung cấp "dịch vụ giá trị gia tăng"; trên một đường truyền tốc độ nhanh để kết nối và mở rộng triển khai các doanh nghiệp với nhau. 

- **Mạng WAN (Wide Area Network)**

Mạng diện rộng WAN là sự kết hợp giữa mạng LAN và mạng MAN với việc sử dụng đường dây cáp quang hay thuê bao hoặc thông qua đường truyền vệ tinh. 

Phạm vi hoạt động của mạng rộng lớn hơn, bao gồm cả một quốc gia, khu vực địa lý hay thậm chí ở toàn cầu. 

- **Mạng PAN (Personal Area Network)**

Mạng PAN có khả năng phát tín hiệu kết nối trong một diện tích nhỏ để truyền dữ liệu thông qua mạng trực tuyến. 

Cá nhân có thể sử dụng mạng PAN giữa các thiết bị với nhau như di động. máy tính. để liên lạc thuận lợi hơn hoặc kết nối với các mạng cao cấp hơn.

#### **Lập trình mạng là gì?**
Lập trình mạng nói một cách dễ hiểu là công việc của người sẽ phát triển ứng dụng tại hệ thống doanh nghiệp từ việc lập sổ sách nhân sự, quản lý tiền cho đến việc sáng tạo các trò chơi, điều khiển để tăng sức hấp dẫn thu hút khách hàng hơn.

Công thức để xây dựng lập trình mạng như sau: 

>- *Lập trình mạng = Kiến thức mạng + Mô hình lập trình mạng + Ngôn ngữ lập trình mạng*

Theo công thức này thì sẽ rất dễ nhận thấy ba vấn đề chính cần quan tâm là kiến thức mạng truyền thông, mô hình lập trình và ngôn ngữ lập trình. 

Về kiến thức mạng truyền thông thì đây là kiến thức chung về mạng di động: mạng Bluetooth, hệ thống GPS, mạng Sensor… mà người làm quản trị cần nắm vững cách sử dụng để khai thác. 

Mô hình lập trình là kiến thức về tất cả các cách xây dựng hệ thống mạng, kiến thức về cơ sở dữ liệu, mô hình xây dựng các chương trình ứng dụng mạng. 

- **Ví dụ về một số ít ngôn ngữ lập trình được ưa chuộng bởi các Dev:**
- **C/C++** → Dùng để viết các ứng dụng mạng ở cấp độ thấp (low-level) thân thuộc và cổ điển, ví dụ như client–server, proxy, hoặc thậm chí là giao thức mạng riêng (chi tiết thì bạn có thể tra wiki hoặc hỏi AI nhé tại vì mình cũng tham khảo thông tin từ mạng là chính 🐴).

- **Python** → dễ học, với nhiều thư viện hỗ trợ như socket, asyncio, requests, flask, vân vân và mây mây. Thường dùng để viết server nhanh, test API, hoặc phân tích dữ liệu mạng (cái này dễ dùng, thân thiện cho người mới học lập trình).

- Và với **Java** ta có thể: - Viết **chat app** giữa hai máy - Tạo **web server** nhỏ dùng socket - Làm **ứng dụng client-server** kiểu gửi file...  
Java nổi tiếng là một ngôn ngữ mạnh mẽ và ổn định, rất phù hợp cho các ứng dụng mạng lớn.
Nếu bạn muốn làm việc với mô hình client-server hoặc các kết nối TCP/IP, Java cung cấp sẵn các thư viện như java.net để xử lý.  
Ngoài ra, nếu chuyển sang JavaScript (khi chạy bằng Node.js) còn cho phép ta thực hiện các tác vụ mạng ở mức gần như là “thời gian thực” (real-time) với độ trễ cực thấp, nhờ vào cơ chế bất đồng bộ (asynchronous) và event loop — thứ giúp chương trình không bị “đơ” khi chờ dữ liệu phản hồi.

- Ngoài ra còn có một số ngôn ngữ lập trình khác như: .NET, Delphi,...

Có thể nói, mỗi ngôn ngữ lập trình đều có sự đặc biệt và đặc điểm riêng của chúng, nhưng để thực sự hiểu thì vẫn phải có sự rèn giũa lâu dài và cố gắn không ngừng nghỉ.
>Nói ngắn gọn: **Lập trình mạng = Giao tiếp qua Internet bằng code**. Với mỗi ngôn ngữ lập trình là một sự giao tiếp đặc biệt riêng với máy.

* **Ta có ví dụ TCP Socket đơn giản sau (chạy bằng Netbeans):**
![Ảnh minh họa](images/tcpsockettest.png)

**Code:**
```Java
//Server.js
public class Server {
    public static void main(String[] args) {
        try {
            ServerSocket server = new ServerSocket(5000);
            System.out.println("✅ Server đang chạy ở cổng 5000...");

            Socket socket = server.accept();
            System.out.println("🟢 Client đã kết nối: " + socket.getInetAddress());

            BufferedReader input = new BufferedReader(new InputStreamReader(socket.getInputStream()));
            PrintWriter output = new PrintWriter(socket.getOutputStream(), true);
            BufferedReader keyboard = new BufferedReader(new InputStreamReader(System.in));

            String message;
            while (true) {
                // Nhận tin nhắn từ client
                if ((message = input.readLine()) != null) {
                    System.out.println("💭 Client: " + message);
                }

                // Gửi tin nhắn từ bàn phím
                System.out.print("Bạn: ");
                String send = keyboard.readLine();
                output.println(send);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```
```Java
//Client.js
public class Client {
    public static void main(String[] args) {
        try {
            // Đổi IP (127.0.0.1) này thành IP của máy "Server" trong mạng LAN
            Socket socket = new Socket("127.0.0.1", 5000); 
            System.out.println("✅ Đã kết nối tới server!");

            BufferedReader input = new BufferedReader(new InputStreamReader(socket.getInputStream()));
            PrintWriter output = new PrintWriter(socket.getOutputStream(), true);
            BufferedReader keyboard = new BufferedReader(new InputStreamReader(System.in));

            String message;
            while (true) {
                // Gửi tin nhắn
                System.out.print("Bạn: ");
                String send = keyboard.readLine();
                output.println(send);

                // Nhận tin nhắn từ server
                if ((message = input.readLine()) != null) {
                    System.out.println("💭 Server: " + message);
                }
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```
Và đó, chính là "Lập trình mạng máy tính", một cách để các "máy" giao tiếp với nhau! 
> Lưu ý: Code trên chỉ là code nhỏ để làm mẫu, không có tính thực dụng, không nên dùng trong các công việc quan trọng.

💡 Bài viết khác nên xem: [Học lập trình mạng cần ngôn ngữ gì?](/ThaoBlog/posts/ngonngucanthiet).