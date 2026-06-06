# Hi there, I'm Tiến Lê 👋

### Fullstack Engineer

Tôi là một nhà phát triển phần mềm tập trung vào mảng Full-stack. Bản thân có kinh nghiệm thực tế với kiến trúc hệ thống phân tán (Microservices), xử lý bất đồng bộ và vận hành các ứng dụng container hóa. Tôi thích tìm tòi, giải quyết các bài toán kỹ thuật thực tế và xây dựng quy trình tự động hóa để tối ưu hiệu suất công việc.

---

## My Engineer Mindset

*   **Compliance Mindset:** Luôn tuân thủ các tiêu chuẩn bảo mật (OWASP, ISO) và tài liệu kiến trúc tổng thể của hệ thống.
*   **KISS Principle (Keep It Simple, Stupid):** Ưu tiên viết code đơn giản, dễ đọc, hạn chế tối đa các thiết kế phức tạp hóa vấn đề khi chưa cần thiết.
*   **Continuous Improvement:** Xem lỗi/sự cố là một vòng lặp phản hồi để cải tiến hệ thống bền bỉ hơn qua từng phiên bản.

---

## Technology Stack

<!-- Hệ thống Badge công nghệ chuẩn hóa theo năng lực thực tế -->
![](https://img.shields.io/badge/Java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![](https://img.shields.io/badge/Spring_Boot-%236DB33F.svg?style=for-the-badge&logo=springboot&logoColor=white)
![](https://img.shields.io/badge/Node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![](https://img.shields.io/badge/C%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)
![](https://img.shields.io/badge/React-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![](https://img.shields.io/badge/Docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![](https://img.shields.io/badge/Kubernetes-%23326CE5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![](https://img.shields.io/badge/Apache_Kafka-%23000000.svg?style=for-the-badge&logo=apachekafka&logoColor=white)

---

## Core Expertise

- **Backend & Architecture:** Phát triển hệ thống phân tán dựa trên kiến trúc **Microservices (Domain-driven design)** và **Kiến trúc 3 lớp (Controllers - Services - Repositories)**; xử lý và tối ưu hóa lưu trữ với MySQL, MongoDB, Redis.
- **Integration & Messaging:** Định tuyến và bảo mật tập trung qua **Kong Gateway (DB-less mode, custom Lua plugin)**, hiện thực kiến trúc hướng sự kiện (Event-driven) sử dụng **Apache Kafka & Saga Pattern** để đảm bảo tính nhất quán dữ liệu.
- **DevOps & Infrastructure:** Đóng gói container với Docker/Docker Compose, xây dựng pipeline tự động hóa **CI/CD bằng GitHub Actions** triển khai lên cụm **Kubernetes (DOKS)** và quản lý mạng qua Cloudflare.
- **Observability & Testing:** Giám sát hiệu năng hệ thống toàn diện thông qua **Jaeger Distributed Tracing**, Prometheus, Grafana; đảm bảo chất lượng với TDD, Unit test và Automation Testing (Selenium).

---

## Featured Projects

### [Distributed E-Commerce Platform](https://github.com/SGU-K22C4/CNLTHD26K1_Nhom9) *(Dự án Nhóm)*
*Hệ thống TMĐT hoàn chỉnh áp dụng kiến trúc Microservices phân tán (gồm 15 containers hệ thống), vận hành trên môi trường sản xuất mô phỏng.*

- **Frontend:** Phát triển giao diện chính Client & Admin bằng **React (Vite)**, tối ưu luồng trải nghiệm người dùng và xử lý dữ liệu thời gian thực.
- **Backend Services:** Thiết kế và triển khai độc lập các dịch vụ cốt lõi: *Promotion-service* (quản lý mã giảm giá), *Review-service* (tích hợp MongoDB) và *AI Chatbot-service* (tích hợp OpenAI/OpenRouter hỗ trợ khách hàng).
- **Data Consistency:** Ứng dụng **Apache Kafka** lắng nghe sự kiện bất đồng bộ; hiện thực kịch bản **Saga Compensation** để hoàn trả chính xác điểm tích lũy của khách hàng thời gian thực khi cổng thanh toán VNPay thất bại.
- **Observability:** Sử dụng **Kong Gateway** làm API Gateway trung tâm kết hợp JWT Auth custom Lua plugin. Tích hợp **Jaeger Distributed Tracing** kiểm soát độ trễ toàn chuỗi (End-to-End Latency) ổn định ở mức 341ms - 510ms.
- **Deployment:** Xây dựng pipeline CI/CD tự động đóng gói image, push lên DigitalOcean Container Registry (DOCR) và triển khai trực tiếp lên cụm **Kubernetes (DOKS)**.

### [Food Fast Delivery](https://github.com/tinhnguyen0123/Food-Fast-Delivery) *(Dự án Nhóm)*
*Hệ thống giao đồ ăn trực tuyến ứng dụng drone delivery, cho phép đặt món, thanh toán và theo dõi hành trình thời gian thực.*

- **Architecture:** Thiết kế kiến trúc backend 3 lớp rõ ràng tách biệt nghiệp vụ phần mềm. Hiện thực hệ thống xác thực JWT và phân quyền nghiêm ngặt (Role-based access control) cho Khách hàng, Nhà hàng và Admin.
- **Realtime Logic:** Xây dựng luồng quản lý đơn hàng realtime và mô phỏng thuật toán di chuyển của Drone giao hàng. Tích hợp cổng thanh toán MoMo, tải ảnh qua Cloudinary và API định vị bản đồ động.
- **Tech Stack:** Node.js, Express.js, MongoDB, React 18, TailwindCSS, Leaflet, Recharts, GitHub Actions.

### [Shogi Strategy Game](https://github.com/tienle-dev/shogi) *(Dự án Nhóm)*
*Trò chơi cờ chiến thuật Nhật Bản (Shogi) phiên bản 2D trên môi trường cross-platform sử dụng Unity Engine và ngôn ngữ C#.*

- **Algorithm & Logic:** Hiện thực ma trận trạng thái bàn cờ hai chiều `GameObject[9, 9]` hiệu năng cao. Phát triển thành công thuật toán giả lập nước đi nâng cao (Speculative Move Execution) trên bản sao ma trận động để kiểm tra trạng thái chiếu tướng (Check/Checkmate) và ngăn chặn nước đi phạm quy.
- **Optimization:** Quản lý vòng đời Object cho cơ chế thả quân (Drop slots). Mã hóa lịch sử bàn cờ thành chuỗi định dạng duy nhất bằng StringBuilder và ứng dụng LINQ để phát hiện trạng thái lặp chuỗi 4 lần (Thiên Nhật Thủ) mà không làm suy giảm hiệu năng game.

---

## Reach on me

<a href="mailto:Imt180304@gmail.com">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" />
</a>
<a href="https://linkedin.com/in/tien-le-02a609414">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
