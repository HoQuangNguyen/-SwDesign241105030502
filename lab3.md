1.Subsystem context diagrams

![Diagram](https://www.planttext.com/api/plantuml/png/T99DJiCm48NtFeNPmQ8No0Arb0WX0K9DBp1r9i7WF-n9gWXnCXOSYIlW_92s8VNopSpdDy_--VfU1W9FbLRi8iT26kIRTBrTFTqzf5me286nW_0CZRTAPKqWrFo3yUuuRmM6C1GlhmPPWu4IK-sKRH13r3zFM5uQoj3NKk0HAeeHb56r6q6Tk45dFSrGx2iAUkpkqcZe5WXs40x84cbeQaiZj78v40wLjGt_qN_ELyufAO2aDIEqbhYVsko9zwQmKz8DcBUpcRMcHqQDNXRDreC98DeRUzISbSNYUl8U2OyveO-3WUyblR3JSZTm77h2FRvN65Vl8vQcd1qvbt32GRHBO3lVDV6O0CmmZW98kB1QLwPT0mUVR8acZr_m5m00__y30000
)

Giải thích:
PayrollSystem: Đây là trung tâm của hệ thống, nơi xử lý tất cả các thông tin và quy trình liên quan đến lương. Nó tương tác với các hệ thống con khác để thực hiện các chức năng của mình.
PrintService:
Chức năng: Cung cấp các dịch vụ in ấn cho hệ thống. Bao gồm việc in phiếu lương và các báo cáo liên quan đến lương.
Tương tác: PayrollSystem gửi yêu cầu in đến PrintService khi cần in các tài liệu, như phiếu lương cho nhân viên hoặc báo cáo cho quản lý.
ProjectManagementDatabase:
Chức năng: Quản lý thông tin liên quan đến các dự án, bao gồm dữ liệu về các dự án đang diễn ra và chi phí liên quan.
Tương tác: PayrollSystem truy cập dữ liệu từ ProjectManagementDatabase để lấy thông tin cần thiết cho việc tính toán lương và chi phí liên quan đến dự án.
EmployeeApplication: Giao diện mà nhân viên sử dụng để tương tác với hệ thống, cho phép họ xem thông tin cá nhân và phiếu lương của mình.
BankSystem: Hệ thống con này xử lý các giao dịch ngân hàng, cho phép hệ thống Payroll gửi thông tin thanh toán đến ngân hàng.

2.Analysis class to design element map
