# Xây Dựng Data Lake Trên Nền Tảng Hadoop

### **Giới Thiệu**
Chào mừng bạn đến với dự án **Xây dựng Data Lake trên nền tảng Hadoop**! Đây là một giải pháp mạnh mẽ giúp bạn lưu trữ, xử lý và phân tích dữ liệu lớn với hiệu quả cao. Dự án này được thiết kế để đơn giản hóa quá trình cài đặt và triển khai, giúp bạn bắt đầu nhanh chóng với công nghệ Big Data.

![Data Lake Architecture](docs/images/data_lake_architecture.png)

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
2. **Chạy script cài đặt:**
   ```bash
   bash install.sh
   ```
   ![Installation Process](docs/images/installation_process.png)

3. **Cài đặt thư viện Python:**
   Nếu cần cài đặt riêng, bạn chỉ cần chạy lệnh sau:
   ```bash
   pip install -r requirements.txt
   ```

---

## **Hướng Dẫn Sử Dụng**
### **Khởi Động Các Dịch Vụ**
1. **Khởi động Hadoop:**
   ```bash
   start-dfs.sh
   start-yarn.sh
   ```
   ![HDFS UI](docs/images/hdfs_ui.png)

2. **Khởi động Kafka:**
   ```bash
   bin/zookeeper-server-start.sh config/zookeeper.properties
   bin/kafka-server-start.sh config/server.properties
   ```
   ![Kafka Dashboard](docs/images/kafka_dashboard.png)

3. **Khởi động Spark:**
   ```bash
   pyspark
   ```
   ![Spark Shell](docs/images/spark_shell.png)

### **Chạy Quy Trình ETL**
1. Thu thập dữ liệu:
   ```bash
   python src/ingestion/data_ingestion.py
   ```
2. Xử lý dữ liệu:
   ```bash
   python src/processing/data_processing.py
   ```
3. Phân tích dữ liệu:
   ```bash
   python src/analytics/data_analysis.py
   ```

---

## **Đóng Góp**
Nếu bạn muốn đóng góp vào dự án, hãy:
1. Fork dự án này.
2. Tạo branch mới: `git checkout -b feature-name`
3. Commit thay đổi: `git commit -m "Add feature-name"`
4. Push branch: `git push origin feature-name`
5. Tạo Pull Request.

---

## **Liên Hệ**
Mọi thắc mắc hoặc góp ý, vui lòng liên hệ qua email: **admin@dataproject.com**.

---

⭐ Hãy nhấn sao (**Star**) nếu bạn thấy dự án hữu ích!
