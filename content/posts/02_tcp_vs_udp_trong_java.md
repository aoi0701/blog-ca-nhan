---
title: "So sánh TCP và UDP trong Java"
date: 2025-12-22
draft: false
tags: ["tcp", "udp", "java", "lap-trinh-mang"]
categories: ["Java", "Network"]
---

## 1. Giới thiệu
Trong lập trình mạng, **TCP** và **UDP** là hai giao thức nền tảng được sử dụng phổ biến.
Bài viết này giúp phân biệt TCP và UDP, đặc biệt trong ngữ cảnh **lập trình Java**.

---

## 2. TCP là gì?
TCP (Transmission Control Protocol) là giao thức:
- Có **kết nối**
- Đảm bảo **dữ liệu gửi đúng thứ tự**
- Có cơ chế **kiểm soát lỗi và tắc nghẽn**

📌 Trong Java, TCP thường được dùng với:
- `Socket`
- `ServerSocket`

👉 Phù hợp với:
- Ứng dụng chat
- Truyền file
- Ứng dụng cần độ tin cậy cao

---

## 3. UDP là gì?
UDP (User Datagram Protocol) là giao thức:
- **Không cần kết nối**
- Không đảm bảo dữ liệu đến đầy đủ
- Tốc độ nhanh, ít overhead

📌 Trong Java, UDP dùng:
- `DatagramSocket`
- `DatagramPacket`

👉 Phù hợp với:
- Game online
- Streaming
- Ứng dụng thời gian thực

---

## 4. So sánh TCP và UDP

| Tiêu chí | TCP | UDP |
|--------|-----|-----|
| Kết nối | Có | Không |
| Độ tin cậy | Cao | Thấp |
| Thứ tự dữ liệu | Có đảm bảo | Không |
| Tốc độ | Chậm hơn | Nhanh hơn |
| Độ phức tạp | Cao | Thấp |

---

## 5. Nên dùng TCP hay UDP trong Java?
- Dùng **TCP** khi cần độ chính xác và an toàn
- Dùng **UDP** khi ưu tiên tốc độ và chấp nhận mất dữ liệu

Việc lựa chọn giao thức phụ thuộc vào **bài toán cụ thể**.

---

## 6. Kết luận
TCP và UDP đều có vai trò quan trọng trong lập trình mạng Java.
Nắm rõ sự khác biệt sẽ giúp lập trình viên lựa chọn đúng giao thức cho ứng dụng của mình.
