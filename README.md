**Project Summary: User Segmentation

Project objective (Why):
Dựa theo dữ liệu người dùng, tìm ra các lựa chọn mô hình và phương pháp phù hợp để phân tập người dùng (User) trên Mạng xã hội X. Từ đó các hoạt động vận hành và truyền thông marketing sẽ được phát triển tương ứng.

Methodology (What):

1.	Business understanding
Xác định nhu cầu của việc phân tập người dùng (Marketing, Product).
Mục đích của việc áp dụng Machine Learning.
Ước lượng outcome của project: có bao nhiêu nhóm User và đặc điểm nhận diện của những nhóm này như thế nào.
Công cụ sử dụng (Google Bigquery, Google Colab, Python, SparkSQL), thuật toán clustering sử dụng (K-means, Hierarchical).
Xây dựng các kế hoạch cho từng giai đoạn cụ thể.

2.	Data understanding
Xác định các loại dữ liệu, các nguồn dữ liệu khác nhau.
Phân tập người dùng chia danh sách các ID người dùng thành các nhóm dựa trên các đặc điểm chung về hành vi người dùng, nhân khẩu học hoặc sở thích. Dưới đây là một số features để phân tập người dùng:
•	Nhân khẩu học: dữ liệu về thông tin cá nhân của User trên Mạng xã hội X: vị trí, tuổi, giới tính, tình trạng hôn nhân. (~ 1m records)
•	Dữ liệu về hành vi, sự kiện của User hoạt động trên app X trong 7 ngày ( ~ 100m records)
•	Dữ liệu tổng kết về thời gian sử dụng app; số lần cài đặt app; số ngày kể từ ngày tạo account; số group, page, chat, friend,...

3.	Data preparation
Source data: Google Bigquery
Data selection: chọn lọc ra các features từ Source data cần phân tích
Data cleaning: làm sạch bộ dữ liệu ( dữ liệu trùng lặp, dữ liệu không hợp lý)
Data transformation: MinMaxScaler, Feature Engneering (PCA)

4.	Modelling
Framework: Google Colab, PySpark
Xác định số cluste tối ưu: Elbow methods
Fit data with clustering algorithm (K-mean and Hierarchical)

5.	Evaluation
Trực quan hóa dữ liệu đã được dán nhãn sau khi fit data (Tableu)
So sánh kết quả phân cụm giữa K-mean and Hierarchical
Kết luận về các đặc điểm phân biệt, nhận dạng của mỗi nhóm User.

Weekly timeline (When): 
Week 1: Tìm hiểu cấu trúc dữ liệu, hệ thống của một Mạng xã hội
Week 2: Chuẩn bị dữ liệu, làm sạch và train model
Week 3: Kết quả, đánh giá mô hình
Week 4: Thuyết trình kết quả Project với line manager, team BI và business user

Applied field (Where): 
+ Chương trình bán hàng, khuyến mãi hoặc các chiến dịch quảng cáo khác của team Marketing và muốn nhắm đến mục tiêu vào một loại khách hàng cụ thể cho từng sản phẩm.
+ Đem đến sự linh hoạt để phân chia ngân sách Marketing vào đâu và như thế nào.
+ Phát triển sự thấu hiểu nhu cầu khách hàng một cách tốt hơn để team Customer Service cải thiện chất lượng dịch vụ khách hàng.
+ Kết hợp cùng với team Tech để phát triển thêm mô hình và xây dựng thêm một số metrics cần thiết.

Related people (Who): 
Trình bày cho line manager, team BI, team Tech và các Business user khác (BOD, team Marketing, CS, Sale)

