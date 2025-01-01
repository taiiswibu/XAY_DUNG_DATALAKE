# Xây Dựng Data Lake Trên Nền Tảng Hadoop

### **Giới Thiệu**
Chào mừng bạn đến với dự án **Xây dựng Data Lake trên nền tảng Hadoop**! Đây là một giải pháp mạnh mẽ giúp bạn lưu trữ, xử lý và phân tích dữ liệu lớn với hiệu quả cao. Dự án này được thiết kế để đơn giản hóa quá trình cài đặt và triển khai, giúp bạn bắt đầu nhanh chóng với công nghệ Big Data.

![Data Lake Architecture](https://www.interviewbit.com/blog/wp-content/uploads/2022/06/Data-Lake-Architecture-1-1024x694.png)

---

## **Tính Năng Chính**
- **Lưu trữ linh hoạt:** Hỗ trợ lưu trữ dữ liệu từ nhiều nguồn khác nhau ở định dạng thô (Raw), đã xử lý (Processed).
- **Xử lý dữ liệu mạnh mẽ:** Sử dụng Apache Spark để làm sạch, chuyển đổi và phân tích dữ liệu.
- **Realtime Streaming:** Tích hợp Apache Kafka để thu thập dữ liệu thời gian thực.
- **Phân tích dữ liệu:** Tích hợp Spark SQL và các công cụ trực quan hóa.

---

## **Cấu Trúc Dự Án**
```plaintext
XAY_DUNG_DATALAKE/
├── README.md          # Tài liệu hướng dẫn
├── install.sh         # Script cài đặt tự động
├── requirements.txt   # Danh sách thư viện cần thiết
├── src/               # Thư mục chứa mã nguồn
│   ├── ingestion/     # Thu thập dữ liệu
│   ├── processing/    # Xử lý dữ liệu
│   └── analytics/     # Phân tích dữ liệu
├── data/              # Thư mục chứa dữ liệu mẫu
└── docs/              # Tài liệu bổ sung
```

---

## **Hướng Dẫn Cài Đặt**
### **Yêu Cầu Hệ Thống**
- **Hệ điều hành**: Ubuntu 20.04 hoặc mới hơn
- **Dung lượng ổ cứng**: Tối thiểu 100GB
- **RAM**: 8GB (khuyến nghị 16GB)
- **Công cụ cần thiết**:
  - Java (JDK 11+)
  - Python 3.8+
  - Hadoop 3.3+
  - Spark 3.4+

### **Cài Đặt Tự Động**
1. **Clone dự án:**
   ```bash
   git clone https://github.com/username/XAY_DUNG_DATALAKE.git
   cd XAY_DUNG_DATALAKE
   ```

2. **Cài đặt thư viện Python:**
   Nếu cần cài đặt riêng, bạn chỉ cần chạy lệnh sau:
   ```bash
   pip install -r requirements.txt
   ```

# Xây Dựng Data Lake Trên Nền Tảng Hadoop

### **Giới Thiệu**
Chào mừng bạn đến với dự án **Xây dựng Data Lake trên nền tảng Hadoop**! Đây là một giải pháp mạnh mẽ giúp bạn lưu trữ, xử lý và phân tích dữ liệu lớn với hiệu quả3. **Cài đặt Hadoop:**
   - Tải về từ trang chính thức:
     ```bash
     wget https://archive.apache.org/dist/hadoop/common/hadoop-3.3.4/hadoop-3.3.4.tar.gz
     ```
   - Giải nén và cấu hình:
     ```bash
     tar -xvf hadoop-3.3.4.tar.gz
     sudo mv hadoop-3.3.4 /usr/local/hadoop
     ```
   - Thêm biến môi trường:
     ```bash
     export HADOOP_HOME=/usr/local/hadoop
     export PATH=$PATH:$HADOOP_HOME/bin:$HADOOP_HOME/sbin
     ```
   - Khởi động dịch vụ:
     ```bash
     hdfs namenode -format
     start-dfs.sh
     start-yarn.sh
     ```

4. **Cài đặt Spark:**
   - Tải Spark:
     ```bash
     wget https://downloads.apache.org/spark/spark-3.4.1/spark-3.4.1-bin-hadoop3.tgz
     ```
   - Giải nén và cấu hình:
     ```bash
     tar -xvf spark-3.4.1-bin-hadoop3.tgz
     sudo mv spark-3.4.1-bin-hadoop3 /usr/local/spark
     ```
   - Thêm biến môi trường:
     ```bash
     export SPARK_HOME=/usr/local/spark
     export PATH=$PATH:$SPARK_HOME/bin:$SPARK_HOME/sbin
     ```
   - Kiểm tra Spark:
     ```bash
     spark-shell
     ```
---

## **Hướng Dẫn Sử Dụng**
### **Khởi Động Các Dịch Vụ**
1. **Khởi động Hadoop:**
   ```bash
   start-dfs.sh
   start-yarn.sh
   ```
   ![HDFS UI](https://tse4.mm.bing.net/th?id=OIP.PfHpyMgnYoEQDUivc9iqYQHaDU&pid=Api&P=0&h=180)


2. **Khởi động Spark:**
   ```bash
   pyspark
   ```
 



## **Đóng Góp**
Nếu bạn muốn đóng góp vào dự án, hãy:
1. Fork dự án này.
2. Tạo branch mới: `git checkout -b feature-name`
3. Commit thay đổi: `git commit -m "Add feature-name"`
4. Push branch: `git push origin feature-name`
5. Tạo Pull Request.

---

## **Liên Hệ**
Mọi thắc mắc hoặc góp ý, vui lòng liên hệ qua email: **vovantai2k4@gmail.com**.

---

⭐ Hãy nhấn sao (**Star**) nếu bạn thấy dự án hữu ích!
