# Data Analysis_Online Retail Dataset
Đồ án môn học Lập trình phân tích dữ liệu (UEH)

# Mô tả bộ dữ liệu
Bộ dữ liệu Online Retail chứa các giao dịch trong khoảng thời gian từ 01/12/2010 đến 09/12/2011 của một cửa hàng kinh doanh bán lẻ trực tuyến có trụ sở tại UK, bao gồm 10 thuộc tính và 541909 dòng.
Bộ dữ liệu có thể tìm thấy ở [Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset) hoặc [UCI Machine Learning](http://archive.ics.uci.edu/ml/datasets/Online+Retail)

- InvoiceNo: Mã đơn hàng 
- InvoiceDate: Ngày đặt hàng
- InvoiceTime: Thời gian đặt hàng
- StockCode: Mã sản phẩm
- Description: Mô tả sản phẩm
- Quantity: Số lượng sản phẩm trong mỗi đơn hàng
- UnitPrice: Giá bán mỗi đơn vị sản phẩm
- Totalsale: Doanh thu từ mỗi sản phẩm trong 1 đơn hàng
- CustomerID: Mã khách hàng
- Country: Quốc gia nơi khách hàng đặt hàng

# Tổng quan dự án

1. EDA (Exploratory Data Analysis – Phân tích Khám phá Dữ liệu) để thăm dò bộ dữ liệu trước khi tiến hành tiền xử lý. Biết được tổng quan các thông tin về: số dòng, số cột, có tồn tại giá trị bị thiếu hay không, nếu có thì ở dòng nào, thuộc cột nào và chiếm bao nhiêu phần trăm của bộ dữ liệu. Phác họa biểu đồ tương quan giữa các biến.
2. Tiền xử lý dữ liệu: Chỉnh dạng dữ liệu, thêm biến mới cần thiết, bỏ bớt biến cũ không cần thiết. Xử lý missing values. Xử lý outliers của các biến định lượng. Xử lý NLP cho biến dạng văn bản
3. Phân tích dữ liệu theo chuỗi thời gian (Time Series) và tìm luật kết hợp các nhóm sản phẩm bán chạy cùng nhau (Market Basket Analysis - FP-Growth).
4. Machine Learning: 
Phân khúc khách hàng theo vị trí địa lý và hành vi mua hàng (K-Prototypes) và phân nhóm sản phẩm theo biến Description (K-Means)
