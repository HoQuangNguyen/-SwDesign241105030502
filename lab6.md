# 1. **BankSystem:deposit**
1. **Xác định lớp và thuộc tính**:
   - `BankSystem`: Đại diện hệ thống ngân hàng.
   - `BankTransaction`: Quản lý giao dịch.
   - `Paycheck`: Đại diện bảng lương, chứa số tiền và thông tin nhân viên.
   - `BankInformation`: Thông tin ngân hàng (tên, số định tuyến).

2. **Xác định phương thức (operations)**:
   - `BankSystem.deposit(Paycheck, BankInformation)`
   - `BankTransaction.create(op, amount, routingNum)`
   - `BankTransaction.submit()`
## Class Diagram:
![Diagram](https://www.planttext.com/api/plantuml/png/T58xRiCm3Drr2euEO5z0Gn5qA90bA93k1YsphH7h0uaQZA8dwz0ZzGgrOgjL74GJGRqF7wMVh-zzOFGSzIZKY2708vhpQGfC6Zu4fDEJis7Wok6atacT9JolLGtTZ3wOLoill5HvZJnOinEVeb1yyMW2gdIJPPKdPAgiat1YFvYt6b3RQ5Z2qsYHQ_0syjm_HfqXkuKQOgVdWGgFFD4gtbmfBItIRhGJqQ7FQejOsmvcuBQjDkwt-4sc8cssJUiuegOhX-O_HqV-ZlcMMQOlM9SHYYTg7cxMAo462cBRdf5_IvBWl5KKxk2suLP5iIVJfu_o2m00__y30000)
## Biểu đồ trạng thái:
![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3bUqLgo2hgwTWcTAJYeN5uW4SqEA4lEA4vDBClFpd8jI4qjIKnIi59B1B0rDBYooQ9g2IvDoCqiWseh1R5Hj27cGHf0Zh1HA4D8AoVcv1Jcf9K0dEQJcfO0S2W000F__0m00)
# 2. **PrintService::print**
1. **Xác định lớp và thuộc tính**:
   - `PrintService`: Quản lý việc in.
   - `PaycheckPrinterImage`: Tạo hình ảnh in từ bảng lương.
   - `PrinterInterface`: Kết nối với máy in.
   - `Employee`: Thông tin nhân viên.

2. **Xác định phương thức (operations)**:
   - `PrintService.print(Paycheck, String)`
   - `PaycheckPrinterImage.buildPrintImage(fromPaycheck)`
## Clas diagram:
![Diagram](https://www.planttext.com/api/plantuml/png/T951Ri8m44NtFiKiGKeka0L2NLHYWoh11IREj8s8FP5dl8WG9sF1aRW22Ks20TNBxpzl_hUlvyjQ58D6rnZRe0Xye3_iEb5oS3HmFnMrBBKklh2plsGFsTsqyTyS76hDVcbE9XdV1_I2ThYP6JOGAYsuBM2deVO_6Q3ZwBM0puPHCmWSjTUtqKsMvJWhiNJz-cJBb6J4vy-iKIFNDjmHRQe9-1mpAJ1pobxVegDvuaz-P2iffBJajV9yzTQ-W2WavbKUh7E50jh0bkG_uslKaRacNms_TWC00F__0m00)
3. **Biểu đồ trạng thái**:
  
![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3XUGKPAge1HGb5gGM9IPbwwaa5Yi0E8XP3BpIX0IG0vCnZa_jo0djIGr1Ipbaf-NoiKLhHMheAjh1p41H41vG6qALWh1gNaf2YNv2WKWVceH5qGSf0Aa6wZ0BJClipW38W-qayi1g07aIW00003__mC0)
# 3. **ProjectManagementDatabase:getChargeNumbers**
**Xác định lớp và thuộc tính**:
   - `ProjectManagementDatabase`: Đại diện hệ thống cơ sở dữ liệu.
   - `ChargeNumList`: Danh sách số tính phí.
   - `ChargeNum`: Đối tượng số tính phí, chứa tên dự án và giá trị.

**Xác định phương thức (operations)**:
   - `getChargeNumbers(String)`: Truy vấn danh sách số tính phí.
   - `ChargeNumList.add(theChargeNum)`.
  
## Class diagram:

![Diagram](https://www.planttext.com/api/plantuml/png/T55B3e8m4Dtt55t2WWiGOqnqgOJ4nFr09r03nNIcRemdS-6Hl885aO-VBj-ytqmVj_kA62oxkX9v1KGojSqHSzw1WG9hDBm1XWm8vKN8xXN8wn9iWOchCxGKd5wI16gCvPwjDaKOou6prSJYAdh_6TnxHZ9_enJBTh0OQCi-5PGAkCG1dmJui7EZrOzw58JVVjzLXXe_DfaLF43b_4GrBgjmp4j7MHiu4KxgTDfstAjzZV-tZgBbnwLYQP6TDIJc-8pfMNbZ6BIdhT2ezbkV0000__y30000)


##Biểu đồ trạng thái:

![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3bUqLgo2hgwTWcjkGKab5nUO0Wk45gGabcJcfIjOAGI35CC5kE0o86NE-Ra5EQabgIb0TM29L8NWqkJarEBYjD8SLAKGi-7At18pSr9JkBWG9e0K0Tt3vP2Qbm9o6m000F__0m00)
# 4. **ProjectManagementDatabase::initialize**
1. **Xác định lớp và thuộc tính**:
   - `DBChargeNumbers`: Kết nối cơ sở dữ liệu.
   - `DriverManager`: Quản lý kết nối.

2. **Xác định phương thức (operations)**:
   - `initialize()`: Thiết lập kết nối.
   - `getConnection(url, user, pass)`: Lấy kết nối đến cơ sở dữ liệu.
## Class diagram:
![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3bToJc9niOABatD6Ob5wgbzfRb9gKR52DPS266JcPPPa9kPaLgLgQ7BLSi5K5sMMfHRv9kObfgSMmTMcfvOuv-VbfIQNPERdQPGMvLWf19SKPUQbwoYK5gSM8NW5G3DWFB2fwBRhwjgXsM45CgAOoo4rBmNaQ000003__mC0)
3. **Biểu đồ trạng thái**:

![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3XUGKPAgeEIIMPoSdvUNcboIcgAaa5YiW2m0K-GC4SZCImShGN3H542DWFEukAArOXLqTUrGJKNcW6KH1YfOAJWdvkGePEPbbcGcvcHMfN8XIIAf1UgqWklBprCeBarEJYqkJYlDuN98pKi1-H00003__mC0)

