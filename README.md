# ETL (SSIS)

**ETL (SSIS)** là một dự án nhằm thực hiện luồng ETL khi sử dụng tool SSIS. Dự án này giúp phục vụ và giải quyết một project xây dựng DWH dựa trên những câu hỏi mang tính chất báo cáo nghiệp vụ cho một cửa hàng kinh doanh.

![cauhoi](https://github.com/user-attachments/assets/841199cb-2dd7-4489-bc42-50ea0f5ad2bf)


## Công nghệ

Công nghệ sử dụng trong dự án:
- SQL Server Integration Services (SSIS)
- SQL Server
- Power Bi (dùng để trực quan hoá dữ liệu sau khi xây dựng DWH)

## Các bước làm

### - Bước 1: Xây dựng Database cho cửa hàng kinh doanh đó
  ![image](https://github.com/user-attachments/assets/4229aca6-c269-4c5d-bd4c-fe990535b03d)
### - Bước 2: Xây dựng những table Dimension và Fact theo mô hình Snowflake Schema
![image](https://github.com/user-attachments/assets/654a37e9-b094-46db-8f9c-c60fbea6a308)
### - Bước 3: Dùng tool SSIS, import data source vào các bảng Stagging dựa trên Data Source
![image](https://github.com/user-attachments/assets/18345c53-46b8-4f6f-b7db-58b55bd966c7)
### - Bước 4: Dùng tool SSIS làm sạch,biến đổi và lưu vào các bảng Stagging dựa trên Dimension và Fact
![image](https://github.com/user-attachments/assets/75f50cf6-03ac-412c-9ec2-a6e7ecc7bfb1)
### - Bước 5: Dùng tool SSIS lưu vào các bảng Dimension và Fact hoàn thiện DWH
#### 1.Dimension (theo thứ tự tổng quát đến chi tiết)
![image](https://github.com/user-attachments/assets/cee9099e-06b8-4644-beb3-20f687ec516c)

![image](https://github.com/user-attachments/assets/7738a51a-26c3-4a6a-a3d6-b3feb198dd83)

![image](https://github.com/user-attachments/assets/5321471c-0fa3-43cb-aa5f-929286bdf672)

#### 2.Fact 
![image](https://github.com/user-attachments/assets/dc79a8eb-21fd-4be7-b4f0-6f7b82145412)

### - Bước 6: Xây dựng dashboard bằng Power PI
![image](https://github.com/user-attachments/assets/4763fbb2-9e14-4000-ac67-8170184a97e9)





## Về project

Dưới đây là ví dụ về cách sử dụng dự án:

1. Tool SSIS được dùng qua Visual Studio 2019
2. Clone project này rồi vào file 'Final Project ColeVN.sln'
![image](https://github.com/user-attachments/assets/09ce46a3-933d-4d0c-919d-2f77e678915b)
3. Bên phải màn hình, chọn đúng file 'Package.dtsx'
![image](https://github.com/user-attachments/assets/bbbb4081-cb39-4b24-be55-e5ca08fd031b)



## Tác giả
Nguyễn Duy Hải Anh

