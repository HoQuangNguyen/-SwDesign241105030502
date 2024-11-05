1. Phân tích các ca sử dụng trong Payroll System
1. Xác định các lớp phân tích
ReportGenerator: Lớp này chịu trách nhiệm tạo báo cáo. Nó sẽ thu thập dữ liệu từ các lớp khác và định dạng báo cáo.
PayrollSystem: Lớp này quản lý các chức năng chính của hệ thống bảng lương, bao gồm việc truy xuất thông tin nhân viên và tạo báo cáo.
Employee: Lớp này đại diện cho thông tin của nhân viên, bao gồm các thuộc tính như EmployeeID, Name, và Salary.
Report: Lớp này đại diện cho báo cáo được tạo ra, bao gồm các thuộc tính như ReportID, Title, và Content.
DatabaseManager: Lớp này chịu trách nhiệm kết nối và truy vấn cơ sở dữ liệu (DB2) để lấy thông tin cần thiết cho báo cáo.

2 Biểu đồ Lớp

![Diagram](https://www.planttext.com/api/plantuml/png/j59BJiCm4Dtx55x28XVe0XNH3HjK4IumD4COoPzqPbefGfoC1KVY2iIf6nIttLJ22qj-8yzxR-RzV7qlHO5rvvtPE12nQ-WvEdVVU0eaog2HxOUnmwai9FHnjR2rCeKsenso9n6AGMOLQpUCeFYCNMIzkLtOVQGcbmJsPU7Jp3NKlIZwYLp6Pwr3nuA6SRj3qGScHIOecAuKSS0dTXwVBts7XVjNR2ciHb7fpYY6vXJpdOizuXDuB2VLOa0-bLceEJhyVrK5SJsa05gSUD_8uHhqlM1DSEfJc3i_vhD9gwgx-VhDF0ofVcXbyeB-aEDqBdx9Binoc4DA_2y0003__mC0)

3. Biếu đồ Sequence

![Diagram](https://www.planttext.com/api/plantuml/png/b991JWCn34NtFeKlm0Lc0KLbZIf6GkhIIYnaAPCCZbkfPsF1aRX2KqgWWM4qpI8Bn-__-2SVR--hRAIs6mAGiwIueOEc4Exz856oAPKYZAL5d8mKhJRqXsmyD2TFF2QrYL9VDEY50QR4yUQsrUmAzRhZRAYVD3fbCaaHchOBhj6RmCLOXPQwRpJjnVD_-1_toZrJ44_6CyGvZWxNfucgmzAnsdjTcwKbpBIlz1rGCDno1YphobmZ3OmKFORapWzp8R8qtLcHtubzVQ0E-vyHW4DcV4op4rJN1ycEr7-ZqSEgRATlVmG00F__0m00)
4. Nhiệm vụ của từng lớp phân tích
PayrollAdministrator: Thực hiện yêu cầu tạo báo cáo, nhập tiêu chí báo cáo, và quyết định lưu hay không lưu báo cáo.
Report: Đại diện cho báo cáo đã được tạo và chứa thông tin báo cáo.
ReportCriteria: Quản lý các tiêu chí báo cáo mà Payroll Administrator nhập vào.
PayrollSystem: Thực hiện xử lý và tạo báo cáo dựa trên thông tin từ Payroll Administrator.
ReportStorage: Quản lý việc lưu trữ báo cáo, đảm bảo báo cáo được lưu đúng vị trí và tên đã chỉ định.
2. Phân tích các ca sử dụng Create Employee Report
1. Xác định các lớp phân tích chính
Employee: Đại diện cho người dùng muốn tạo báo cáo cá nhân.
EmployeeReport: Đại diện cho báo cáo được tạo, có thể là "Total Hours Worked", "Total Hours Worked for a Project", "Vacation/Sick Leave", hoặc "Total Pay Year-to-Date".
ReportCriteria: Chứa các thông tin tiêu chí báo cáo mà Employee nhập vào, như loại báo cáo, ngày bắt đầu và kết thúc, và số mã charge (nếu có).
PayrollSystem: Lớp chính để thực hiện các thao tác liên quan đến báo cáo, xử lý yêu cầu từ Employee.
ProjectManagementDB: Đại diện cho cơ sở dữ liệu dự án hiện có, nơi lưu trữ thông tin về mã charge của các dự án.
ReportStorage: Quản lý việc lưu trữ báo cáo, bao gồm tên và vị trí lưu báo cáo.

2. Biểu đồ Lớp

![Diagram](https://www.planttext.com/api/plantuml/png/j5DBJeH04DrpYbxgWWiGCvauk33H2H4zG0sKJ1lenkg2X1XFvi8ZUGMxWI7IC74rB3gfJrwzUlNu-VhU6WRYfYg3h0HZn5rLbxf351-1i5yeS4pSnv58cQGgneA22cSf8GZV6pJyXBKclhgEHAjbFjOCjEWLFWDlw52VHbCVFdSrUgCFM4WL0zkyUqzCLRx8PKUW0lTDTK3oG5h8WAMsE9rvCPX7GYeUoHQea2pAES93VaUIaIHSdF0qDu6ET5ccdM6ifh6c3rFkiTOESYBgdIGZNExu_xKIqc-OyICeAB12nV7jHEMitewBZR35tPyMuz0VfE6ReNNZIvoo9Zjbmd-L9IR0HqzVbzul_RY-nMJnCDpC5Gtc-hhwt9g1vrJNCVV22iIANYjTits3hVM6-ob_0G00__y3000)

3. Biểu đồ Sequence
   
![Diagram](https://www.planttext.com/api/plantuml/png/b9J1JiCm38RlUGfhTrvW1vXWI5n0Y4qWZYRrHY2DY-DEwhDnu95u1T9DOShQeT533xK_--__f_t-_9f5HT6szWQjii1rtNZkY4oJ7Zlh6WmAzzW9Ux_eeb9TL7Bx0pKiMaB2RsJr5WEkgQQWyykYlaCMQMcg6vCdmTbvkM-QEZzQYWgo9S0AeJeEfcZhkJnZ175Aul2lBKdlnbKqGD1dhR3i6W8NOR9aHGytt4g49vPtgc2LpCFyqXC3wHhe6x6abwhYQ4FWNHBCAx2lA6k2qDOl974tQGYE-gIjX0D-EtPSpj2k0eL8FYtjdUxn4wmhS4EX6aPqG3wYTnKgxUq-gdANmHIk-lXpJ7-TWJBGKmwOCaJSPE9Y6_qpnLFT2rWJOAZ0iyN_-3OE3ZOMNymK5dkfXdmakECZnwxSEdVHebI_Q8ffbcxzF-07003__mC0)

. Nhiệm vụ của từng lớp phân tích
Employee: Thực hiện yêu cầu tạo báo cáo, nhập tiêu chí báo cáo, và quyết định lưu hay không lưu báo cáo.
EmployeeReport: Đại diện cho báo cáo được tạo, có chứa thông tin phù hợp với loại báo cáo được chọn.
ReportCriteria: Quản lý các tiêu chí báo cáo mà Employee nhập vào.
PayrollSystem: Xử lý các yêu cầu từ Employee, quản lý quá trình tạo báo cáo và lưu báo cáo.
ProjectManagementDB: Lấy danh sách mã charge của dự án, cần thiết cho báo cáo "Total Hours Worked for a Project".
ReportStorage: Quản lý việc lưu trữ báo cáo, đảm bảo báo cáo được lưu đúng vị trí và tên đã chỉ định.
