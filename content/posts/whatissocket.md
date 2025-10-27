---
title: "Lập trình socket là gì?"
date: 2025-10-11
description: "Giới thiệu khái niệm socket và cách dùng trong lập trình mạng."
categories: ["Lập trình mạng"]
tags: ["Socket", "Cơ bản"]
---


Trong hệ thống mạng máy tính tồn tại những mô hình tham chiếu có kiến trúc phần tầng (OSI, TCP/IP…) nhằm hỗ trợ chức năng trao đôi thông tin giữa các ứng dụng ở nhiều máy tính khác nhau. Trong đó **Socket** giống như “đường dây” giữa hai chương trình để gửi và nhận dữ liệu.  
![Ảnh minh họa](images/socket_tcp_ip.jpg)

Dữ liệu bên gửi sẽ được đóng gói (Encapsulation) từ tầng trên đến tầng cuối là tầng vật lí (Physical Layer), sau đó nhờ tầng vật lí này chuyển dữ liệu đến tầng vật lí máy bên nhận, bên nhận tiến hành giải mã (decapsulation) gói dữ kiện từ tầng dưới lên tầng trên cùng, là tầng ứng dụng (application layer).

Để đóng gói (Encapsulation) thông thường, người ta sẽ khai báo các biến là riêng tư (private), chủ yếu để hạn chế truy cập dữ liệu từ ngoài lớp (class). Rồi cung cấp các phương thức getter và setter (phương thức trung gian) cho phép truy cập dữ liệu. Với việc triển khai xác thực dữ liệu, người ta sẽ đảm tính toàn vẹn của dữ liệu bằng cách xác thực trước khi gán dữ liệu vào các thuộc tính của đối tượng (Object).  

Ví dụ:
- Client (máy người dùng) gửi tin nhắn (đã được đóng gói).
- Server nhận tin, xử lý (giải mã), rồi phản hồi lại.

Bạn muốn xem code mẫu? [Ấn vào đây!](/ThaoBlog/posts/laptrinhmanglagi).

![Tiếp tục với câu hỏi tiếp theo](images/question_mark.jpg)
#### **Vậy thì tại sao lại phải đóng gói dữ liệu?**
- Việc ẩn dữ liệu để tránh bị rò rỉ là một việc hết sức quan trọng, chỉ với việc một chút thông tin cực nhỏ bị rò rỉ, có thể bị kẻ xấu lợi dụng để truy cập trái phép và gây ra thiệt hại nghiêm trọng. Vì thế việc bảo vệ này nhằm đảm bảo tính toàn vẹn của dữ liệu và giúp ta tránh được những hậu quả không mong muốn.
- Nếu bạn bỏ qua bộ điều chỉnh quyền truy cập (riêng tư, được bảo vệ hoặc công khai), Java sẽ áp dụng bộ điều chỉnh quyền truy cập mặc định.
```Java
//Phương thức Mặc định
class MyClass {
     int myVariable; //Khai báo biến theo mặc định
    
     void myMethod() {
         System.out.println("This is a default method");
     } 
}
```

- Từ khóa "private" khai báo các biến chỉ có thể truy cập được trong lớp (class) được khai báo. Các lớp khác trong cùng chương trình không thể truy cập các phương thức hoặc biến dữ liệu private này. Các lớp và giao diện không thể là private.
```Java
class Shape {
     protected double area; // Protected area

     public Shape(double area) {
         this.area = area;
     }

     public double getArea() {
         return area;
     }
 }

class Circle extends Shape {
     private double radius;

     public Circle(double radius) {
         super(Math.PI * radius * radius); // Calling parent constructor
         this.radius = radius;
     } 
}
```

- Đối với biến công khai, từ khóa "public" có phạm vi rộng nhất và có thể được truy cập từ bất kỳ đâu trong code, gần như không có giới hạn nào cả!
```Java
//Public nè
public class Rectangle {
     public double width; // Public width
     public double height; // Public height

     public Rectangle(double width, double height) {
         this.width = width;
         this.height = height;
     }

     public double calculateArea() {
         return width * height;
     } 
}
```

#### **Ví dụ: Đóng gói trong Java**
```Java
public class Person {
     private String name;
     private int age;

     // Constructor
     public Person(String name, int age) {
         this.name = name;
         this.age = age;
     }

     // Getters
     public String getName() {
         return name;
     }

     public int getAge() {
         return age;
     }

     // Setters
     public void setName(String name) {
         this.name = name;
     }

     public void setAge(int age) {
         if (age >= 0) {
             this.age = age;
         } else {
             System.out.println("Invalid age");
         }
     } 
}
```
Trong ví dụ trên, chúng ta đã khai báo hai biến riêng tư: name và age. Các phương thức getter công khai getName và getAge được sử dụng để truy cập các giá trị của name và age tương ứng. SetName và setAge là các phương thức setter công khai sửa đổi các biến name và age tương ứng.

>Tóm lại: Đóng gói là một trong những  khái niệm cốt lõi trong lập trình hướng đối tượng và mô tả việc đóng gói dữ liệu và phương thức hoạt động trên dữ liệu này thành một đơn vị.

Bài viết khác mà bạn có thể thích: [TCP và UDP khác nhau như thế nào?](/ThaoBlog/posts/tcpvaudplagi).