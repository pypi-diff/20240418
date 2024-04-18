# Comparing `tmp/datavns-0.0.4.tar.gz` & `tmp/datavns-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datavns-0.0.4.tar", last modified: Thu Mar  7 23:03:27 2024, max compression
+gzip compressed data, was "datavns-0.0.5.tar", last modified: Thu Apr 18 19:15:14 2024, max compression
```

## Comparing `datavns-0.0.4.tar` & `datavns-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 23:03:27.100690 datavns-0.0.4/
--rw-rw-rw-   0        0        0     1066 2024-03-03 09:52:30.000000 datavns-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    15482 2024-03-07 23:03:27.100690 datavns-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    14920 2024-03-07 23:01:33.000000 datavns-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-07 23:03:27.085063 datavns-0.0.4/datavns/
--rw-rw-rw-   0        0        0      121 2024-02-28 07:23:21.000000 datavns-0.0.4/datavns/__init__.py
--rw-rw-rw-   0        0        0     1070 2024-03-02 20:56:11.000000 datavns-0.0.4/datavns/back_test.py
--rw-rw-rw-   0        0        0     6493 2024-03-02 20:47:10.000000 datavns-0.0.4/datavns/data_function.py
--rw-rw-rw-   0        0        0     2007 2024-01-29 17:44:08.000000 datavns-0.0.4/datavns/headers.py
--rw-rw-rw-   0        0        0     2302 2024-03-02 22:11:47.000000 datavns-0.0.4/datavns/indicator.py
--rw-rw-rw-   0        0        0      281 2024-02-26 21:57:34.000000 datavns-0.0.4/datavns/lib.py
--rw-rw-rw-   0        0        0      836 2024-03-03 08:15:22.000000 datavns-0.0.4/datavns/optimize.py
--rw-rw-rw-   0        0        0     2162 2024-03-02 22:52:24.000000 datavns-0.0.4/datavns/take_data_for_backtest.py
-drwxrwxrwx   0        0        0        0 2024-03-07 23:03:27.100690 datavns-0.0.4/datavns.egg-info/
--rw-rw-rw-   0        0        0    15482 2024-03-07 23:03:27.000000 datavns-0.0.4/datavns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-03-07 23:03:27.000000 datavns-0.0.4/datavns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 23:03:27.000000 datavns-0.0.4/datavns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-07 23:03:27.000000 datavns-0.0.4/datavns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2024-03-07 23:02:00.000000 datavns-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-07 23:03:27.100690 datavns-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 19:15:14.433414 datavns-0.0.5/
+-rw-rw-rw-   0        0        0     1066 2024-03-03 09:52:30.000000 datavns-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    16755 2024-04-18 19:15:14.432242 datavns-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    16193 2024-04-18 19:10:41.000000 datavns-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 19:15:14.412227 datavns-0.0.5/datavns/
+-rw-rw-rw-   0        0        0      121 2024-02-28 07:23:21.000000 datavns-0.0.5/datavns/__init__.py
+-rw-rw-rw-   0        0        0     1146 2024-04-18 19:04:27.000000 datavns-0.0.5/datavns/back_test.py
+-rw-rw-rw-   0        0        0     7461 2024-03-07 22:10:13.000000 datavns-0.0.5/datavns/data_function.py
+-rw-rw-rw-   0        0        0     2007 2024-01-29 17:44:08.000000 datavns-0.0.5/datavns/headers.py
+-rw-rw-rw-   0        0        0     2349 2024-04-12 03:00:44.000000 datavns-0.0.5/datavns/indicator.py
+-rw-rw-rw-   0        0        0      281 2024-02-26 21:57:34.000000 datavns-0.0.5/datavns/lib.py
+-rw-rw-rw-   0        0        0      919 2024-04-08 03:06:46.000000 datavns-0.0.5/datavns/optimize.py
+-rw-rw-rw-   0        0        0     2162 2024-03-02 22:52:24.000000 datavns-0.0.5/datavns/take_data_for_backtest.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:15:14.430342 datavns-0.0.5/datavns.egg-info/
+-rw-rw-rw-   0        0        0    16755 2024-04-18 19:15:14.000000 datavns-0.0.5/datavns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-18 19:15:14.000000 datavns-0.0.5/datavns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:15:14.000000 datavns-0.0.5/datavns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 19:15:14.000000 datavns-0.0.5/datavns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2024-04-18 19:14:31.000000 datavns-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 19:15:14.433414 datavns-0.0.5/setup.cfg
```

### Comparing `datavns-0.0.4/LICENSE` & `datavns-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datavns-0.0.4/PKG-INFO` & `datavns-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datavns
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to collect and backtest the trading strategy on Vietnam stocks market
 Author-email: the-a1pha <buitruonganbta@gmail.com>
 Project-URL: Homepage, https://github.com/the-a1pha/datavns
 Project-URL: Issues, https://github.com/the-a1pha/datavns/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,29 +15,39 @@
 <div align="center">
 
 # **Thư viện thu thập dữ liệu và backtest chiến lược đầu tư**
 # **dữ liệu dựa trên thị trường chứng khoán Việt Nam**
 </div>
 
 
+## Hướng dẫn cài đặt
+
+Để cài đặt package sử dụng câu lệnh:
+
+    pip install datavns
+  
+Để import thư viện vào file và sử dụng
+
+    from datavns import *
 
 ## I. GIỚI THIỆU TỔNG QUAN
 Dự án được thực hiện gồm 2 phần chính
 - Phần một là thu thập dữ liệu về giá cổ phiếu và các thông tin vi mô của doanh nghiệp
 
-- Phần hai là xây dựng hệ thống kiểm thử cho chiến lược cụ thể dựa trên lịch sử giao dịch của cổ phiếu đó
+- Phần hai là xây dựng hệ thống kiểm thử cho chiến lược cụ thể dựa trên lịch sử giao dịch của cổ phiếu và tối ưu hóa danh mục
 
 
 ## II. NỘI DUNG CHÍNH CỦA DỰ ÁN
 
 ### Phần 1: Thu thập dữ liệu
+
 #### 1.1 Thu thập dữ liệu về danh sách cổ phiếu niêm yết
 *Để thu thập dữ liệu về danh sách cổ phiếu theo sàn, chúng ta có thể sử dụng câu lệnh*
 ```python
-list_cp()
+list_cp(exchange = 'HSX')
 ```
 <details>
   <summary>Output</summary>
 
 ```
     Symbol TradeCenterId                                        CompanyName     CategoryName
 0      AAA          HOSE                  Công ty Cổ phần Nhựa An Phát Xanh  Nguyên vật liệu
@@ -57,17 +67,19 @@
 #### 1.2 Thu thập dữ liệu về lịch sử giao dịch của cổ phiếu
 *Để thu thập dữ liệu về thông tin giao dịch của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 price(cp = 'VCB',start_date='2000-01-01',end_date='2024-01-01')
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `start_date (str)`: Ngày bắt đầu trong khoảng thời gian cần lấy thông tin giao dịch
-    `end_date (str)`: Ngày kết thúc trong khoảng thời gian cần lấy thông tin giao dịch
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `start_date (str)`: Ngày bắt đầu trong khoảng thời gian cần lấy thông tin giao dịch
+
+  `end_date (str)`: Ngày kết thúc trong khoảng thời gian cần lấy thông tin giao dịch
 <details>
   <summary>Output</summary>
 
 ```
                   date symbol  priceHigh   priceLow  priceOpen  priceAverage  priceClose  ...  sellQuantity  adjRatio  currentForeignRoom  propTradingNetDealValue  propTradingNetPTValue  propTradingNetValue    unit
 2009-06-30  2009-06-30    VCB  13.753204  13.753204  13.753204     13.753204   13.753204  ...      294070.0   4.36262          82612532.0                      NaN                    NaN                  NaN  1000.0
 2009-07-01  2009-07-01    VCB  14.440864  13.638594  14.440864     13.867814   13.867814  ...     9434870.0   4.36262          82441852.0                      NaN                    NaN                  NaN  1000.0
@@ -86,24 +98,30 @@
 #### 1.3 Thu thập dữ liệu về báo cáo tài chính
 *Để thu thập dữ liệu về báo cáo tài chính của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 bctc('VHM',type=1,year=2023,quarter=4)
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `type (int)`: Loại báo cáo trong báo cáo tài chính cần lấy
-        type = 1: Bảng cân đối kế toán
-        type = 2: Báo cáo kết quả hoạt động kinh doanh
-        type = 3: Báo cáo lưu chuyển tiền tệ trực tiếp (Đa số các doanh nghiệp bị trống dữ liệu về báo cáo lưu chuyển tiền tệ trực tiếp, trừ nhóm ngành ngân hàng)
-        type = 4: Báo cáo lưu chuyển tiền tệ gián tiếp
-    `year (int)`: Năm cuối cùng trong danh sách báo cáo tài chính cần lấy
-    `quarter (int)`: Quý của báo cáo tài chính cần lấy
-        quarter = 0: Sẽ lấy báo cáo tài chính theo năm của doanh nghiệp
-        quarter = 1-4: Sẽ lấy báo cáo tài chính theo quý của năm tương ứng với parameter `year`
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `type (int)`: Loại báo cáo trong báo cáo tài chính cần lấy
+
+      type = 1: Bảng cân đối kế toán
+      type = 2: Báo cáo kết quả hoạt động kinh doanh
+      type = 3: Báo cáo lưu chuyển tiền tệ trực tiếp (Đa số các doanh nghiệp bị trống dữ liệu về báo cáo lưu chuyển tiền tệ trực tiếp, trừ nhóm ngành ngân hàng)
+      type = 4: Báo cáo lưu chuyển tiền tệ gián tiếp
+
+  `year (int)`: Năm cuối cùng trong danh sách báo cáo tài chính cần lấy
+
+  `quarter (int)`: Quý của báo cáo tài chính cần lấy
+
+      quarter = 0: Sẽ lấy báo cáo tài chính theo năm của doanh nghiệp
+      quarter = 1-4: Sẽ lấy báo cáo tài chính theo quý của năm tương ứng với parameter `year`
+
 <details>
   <summary>Output</summary>
 
 ```
 TÀI SẢN A. Tài sản lưu động và đầu tư ngắn hạn I. Tiền và các khoản tương đương tiền           1. Tiền  ... 2. Nguồn kinh phí đã hình thành tài sản cố định 3. Quỹ dự phòng trợ cấp mất việc làm TỔNG CỘNG NGUỒN VỐN Symbol
 2016-4       0                       16491882437206.0                       2802422910160.0    941467410160.0  ...                                             0.0                                  0.0    37520745782451.0    VHM   
 2017-4       0                       44421050167080.0                       1561577770818.0    818341400251.0  ...                                               0                                    0    51303819026055.0    VHM   
@@ -130,23 +148,24 @@
 2023-1       0                      205327661000000.0                       1889644000000.0   1642692000000.0  ...                                             0.0                                  0.0   377621667000000.0    VHM   
 2023-2       0                      190310276000000.0                       5105284000000.0   3829067000000.0  ...                                             0.0                                  0.0   391330538000000.0    VHM   
 2023-3       0                      215057869000000.0                       2909914000000.0   2482981000000.0  ...                                             0.0                                  0.0   417039474000000.0    VHM   
 2023-4       0                      240250006000000.0                      14104131000000.0  13124281000000.0  ...                                             0.0                                  0.0   447360776000000.0    VHM 
 ```
 </details>
 
-#### 1.3 Thu thập dữ liệu về lịch sử chi trả cổ tức
+#### 1.4 Thu thập dữ liệu về lịch sử chi trả cổ tức
 *Để thu thập dữ liệu về lịch sử chi trả cổ tức của của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 dividends_historical(cp='VIC',num=20)
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `num (int)`: Số năm lấy dữ liệu chi trả cổ tức, tính ngược từ thời điểm hiện tại
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `num (int)`: Số năm lấy dữ liệu chi trả cổ tức, tính ngược từ thời điểm hiện tại
 
 <details>
   <summary>Output</summary>
 
 ```
     year  cashDividend  stockDividend   totalAssets  stockHolderEquity
 0   2005           0.0       0.000000  4.891457e+11       3.137832e+11
@@ -167,14 +186,46 @@
 15  2020           0.0       0.000000  4.225038e+14       1.358527e+14
 16  2021           0.0      12.499993  4.283845e+14       1.595719e+14
 17  2022           0.0       0.000000  5.774072e+14       1.356554e+14
 18  2023           0.0       0.000000  6.696171e+14       1.480216e+14
 ```
 </details>
 
+### Phần 2: Backtest
+
+#### 2.1. Tải & lưu dữ liệu phục vụ cho backtest
+
+*Các bước cần thực hiện để tải dữ liệu phục vụ cho quá trình backtest*
+
+* Tạo đường dẫn thư mục đến file dữ liệu backtest
+
+  Chạy file `update_data_for_backtest.py` sau đó chỉ đường dẫn thư mục mong muốn để lưu dữ liệu phục vụ backtest, đường dẫn default đến thư mục sẽ là `D:\Python\datavns\Data`
+
+* Để import dữ liệu vào backtest, sử dụng câu lệnh:
+
+```python
+data_for_backtest.take()
+```
+<details>
+  <summary>Output</summary>
+
+```
+Dữ liệu phục vụ backtest được lưu tại dict: .data
+```
+</details>
+
+#### 2.2. Đối với danh mục đầu tư gồm các cổ phiếu được xác định trước
+
+
+#### 2.3. Đối với danh mục đầu tư được tối ưu hóa tự động
+
+### Phần 3: Các chỉ số đánh giá hiệu quả danh mục
+
+*Đang trong giai đoạn phát triển, vui lòng chờ*
+
```

### Comparing `datavns-0.0.4/README.md` & `datavns-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 <div align="center">
 
 # **Thư viện thu thập dữ liệu và backtest chiến lược đầu tư**
 # **dữ liệu dựa trên thị trường chứng khoán Việt Nam**
 </div>
 
 
+## Hướng dẫn cài đặt
+
+Để cài đặt package sử dụng câu lệnh:
+
+    pip install datavns
+  
+Để import thư viện vào file và sử dụng
+
+    from datavns import *
 
 ## I. GIỚI THIỆU TỔNG QUAN
 Dự án được thực hiện gồm 2 phần chính
 - Phần một là thu thập dữ liệu về giá cổ phiếu và các thông tin vi mô của doanh nghiệp
 
-- Phần hai là xây dựng hệ thống kiểm thử cho chiến lược cụ thể dựa trên lịch sử giao dịch của cổ phiếu đó
+- Phần hai là xây dựng hệ thống kiểm thử cho chiến lược cụ thể dựa trên lịch sử giao dịch của cổ phiếu và tối ưu hóa danh mục
 
 
 ## II. NỘI DUNG CHÍNH CỦA DỰ ÁN
 
 ### Phần 1: Thu thập dữ liệu
+
 #### 1.1 Thu thập dữ liệu về danh sách cổ phiếu niêm yết
 *Để thu thập dữ liệu về danh sách cổ phiếu theo sàn, chúng ta có thể sử dụng câu lệnh*
 ```python
-list_cp()
+list_cp(exchange = 'HSX')
 ```
 <details>
   <summary>Output</summary>
 
 ```
     Symbol TradeCenterId                                        CompanyName     CategoryName
 0      AAA          HOSE                  Công ty Cổ phần Nhựa An Phát Xanh  Nguyên vật liệu
@@ -43,17 +53,19 @@
 #### 1.2 Thu thập dữ liệu về lịch sử giao dịch của cổ phiếu
 *Để thu thập dữ liệu về thông tin giao dịch của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 price(cp = 'VCB',start_date='2000-01-01',end_date='2024-01-01')
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `start_date (str)`: Ngày bắt đầu trong khoảng thời gian cần lấy thông tin giao dịch
-    `end_date (str)`: Ngày kết thúc trong khoảng thời gian cần lấy thông tin giao dịch
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `start_date (str)`: Ngày bắt đầu trong khoảng thời gian cần lấy thông tin giao dịch
+
+  `end_date (str)`: Ngày kết thúc trong khoảng thời gian cần lấy thông tin giao dịch
 <details>
   <summary>Output</summary>
 
 ```
                   date symbol  priceHigh   priceLow  priceOpen  priceAverage  priceClose  ...  sellQuantity  adjRatio  currentForeignRoom  propTradingNetDealValue  propTradingNetPTValue  propTradingNetValue    unit
 2009-06-30  2009-06-30    VCB  13.753204  13.753204  13.753204     13.753204   13.753204  ...      294070.0   4.36262          82612532.0                      NaN                    NaN                  NaN  1000.0
 2009-07-01  2009-07-01    VCB  14.440864  13.638594  14.440864     13.867814   13.867814  ...     9434870.0   4.36262          82441852.0                      NaN                    NaN                  NaN  1000.0
@@ -72,24 +84,30 @@
 #### 1.3 Thu thập dữ liệu về báo cáo tài chính
 *Để thu thập dữ liệu về báo cáo tài chính của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 bctc('VHM',type=1,year=2023,quarter=4)
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `type (int)`: Loại báo cáo trong báo cáo tài chính cần lấy
-        type = 1: Bảng cân đối kế toán
-        type = 2: Báo cáo kết quả hoạt động kinh doanh
-        type = 3: Báo cáo lưu chuyển tiền tệ trực tiếp (Đa số các doanh nghiệp bị trống dữ liệu về báo cáo lưu chuyển tiền tệ trực tiếp, trừ nhóm ngành ngân hàng)
-        type = 4: Báo cáo lưu chuyển tiền tệ gián tiếp
-    `year (int)`: Năm cuối cùng trong danh sách báo cáo tài chính cần lấy
-    `quarter (int)`: Quý của báo cáo tài chính cần lấy
-        quarter = 0: Sẽ lấy báo cáo tài chính theo năm của doanh nghiệp
-        quarter = 1-4: Sẽ lấy báo cáo tài chính theo quý của năm tương ứng với parameter `year`
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `type (int)`: Loại báo cáo trong báo cáo tài chính cần lấy
+
+      type = 1: Bảng cân đối kế toán
+      type = 2: Báo cáo kết quả hoạt động kinh doanh
+      type = 3: Báo cáo lưu chuyển tiền tệ trực tiếp (Đa số các doanh nghiệp bị trống dữ liệu về báo cáo lưu chuyển tiền tệ trực tiếp, trừ nhóm ngành ngân hàng)
+      type = 4: Báo cáo lưu chuyển tiền tệ gián tiếp
+
+  `year (int)`: Năm cuối cùng trong danh sách báo cáo tài chính cần lấy
+
+  `quarter (int)`: Quý của báo cáo tài chính cần lấy
+
+      quarter = 0: Sẽ lấy báo cáo tài chính theo năm của doanh nghiệp
+      quarter = 1-4: Sẽ lấy báo cáo tài chính theo quý của năm tương ứng với parameter `year`
+
 <details>
   <summary>Output</summary>
 
 ```
 TÀI SẢN A. Tài sản lưu động và đầu tư ngắn hạn I. Tiền và các khoản tương đương tiền           1. Tiền  ... 2. Nguồn kinh phí đã hình thành tài sản cố định 3. Quỹ dự phòng trợ cấp mất việc làm TỔNG CỘNG NGUỒN VỐN Symbol
 2016-4       0                       16491882437206.0                       2802422910160.0    941467410160.0  ...                                             0.0                                  0.0    37520745782451.0    VHM   
 2017-4       0                       44421050167080.0                       1561577770818.0    818341400251.0  ...                                               0                                    0    51303819026055.0    VHM   
@@ -116,23 +134,24 @@
 2023-1       0                      205327661000000.0                       1889644000000.0   1642692000000.0  ...                                             0.0                                  0.0   377621667000000.0    VHM   
 2023-2       0                      190310276000000.0                       5105284000000.0   3829067000000.0  ...                                             0.0                                  0.0   391330538000000.0    VHM   
 2023-3       0                      215057869000000.0                       2909914000000.0   2482981000000.0  ...                                             0.0                                  0.0   417039474000000.0    VHM   
 2023-4       0                      240250006000000.0                      14104131000000.0  13124281000000.0  ...                                             0.0                                  0.0   447360776000000.0    VHM 
 ```
 </details>
 
-#### 1.3 Thu thập dữ liệu về lịch sử chi trả cổ tức
+#### 1.4 Thu thập dữ liệu về lịch sử chi trả cổ tức
 *Để thu thập dữ liệu về lịch sử chi trả cổ tức của của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 dividends_historical(cp='VIC',num=20)
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `num (int)`: Số năm lấy dữ liệu chi trả cổ tức, tính ngược từ thời điểm hiện tại
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `num (int)`: Số năm lấy dữ liệu chi trả cổ tức, tính ngược từ thời điểm hiện tại
 
 <details>
   <summary>Output</summary>
 
 ```
     year  cashDividend  stockDividend   totalAssets  stockHolderEquity
 0   2005           0.0       0.000000  4.891457e+11       3.137832e+11
@@ -153,14 +172,46 @@
 15  2020           0.0       0.000000  4.225038e+14       1.358527e+14
 16  2021           0.0      12.499993  4.283845e+14       1.595719e+14
 17  2022           0.0       0.000000  5.774072e+14       1.356554e+14
 18  2023           0.0       0.000000  6.696171e+14       1.480216e+14
 ```
 </details>
 
+### Phần 2: Backtest
+
+#### 2.1. Tải & lưu dữ liệu phục vụ cho backtest
+
+*Các bước cần thực hiện để tải dữ liệu phục vụ cho quá trình backtest*
+
+* Tạo đường dẫn thư mục đến file dữ liệu backtest
+
+  Chạy file `update_data_for_backtest.py` sau đó chỉ đường dẫn thư mục mong muốn để lưu dữ liệu phục vụ backtest, đường dẫn default đến thư mục sẽ là `D:\Python\datavns\Data`
+
+* Để import dữ liệu vào backtest, sử dụng câu lệnh:
+
+```python
+data_for_backtest.take()
+```
+<details>
+  <summary>Output</summary>
+
+```
+Dữ liệu phục vụ backtest được lưu tại dict: .data
+```
+</details>
+
+#### 2.2. Đối với danh mục đầu tư gồm các cổ phiếu được xác định trước
+
+
+#### 2.3. Đối với danh mục đầu tư được tối ưu hóa tự động
+
+### Phần 3: Các chỉ số đánh giá hiệu quả danh mục
+
+*Đang trong giai đoạn phát triển, vui lòng chờ*
+
```

### Comparing `datavns-0.0.4/datavns/back_test.py` & `datavns-0.0.5/datavns/back_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from .data_function import *
 from .optimize import *
 from .indicator import *
 ##########
 
-class back_test:
-
+class back_test: 
     @classmethod
     def buy_conditions(cls, conds = None) -> pd.DataFrame:
-        conds = conds.replace('and', '*')
-        conds = conds.replace('or', '+')
-        df_raw = eval(conds).astype(int)
-        cls.buy_matrix = df_raw
-
+        matrix = 1
+        for i in conds:
+            i = i.replace(' and ', '*').replace(' or ', '+')
+            matrix *= eval(i)
+        cls.buy_matrix  = matrix
+    
     @classmethod
-    def sell_conditions(cls, conds = None) -> pd.DataFrame:
-        conds = conds.replace('and', '*')
-        conds = conds.replace('or', '+')
-        df_raw = eval(conds).astype(int)
-        cls.sell_matrix = df_raw
-        cls.order_matrix = cls.buy_matrix.mask(cls.sell_matrix == 1, -1).apply(order_matrix_optimize, axis=0,result_type='expand')
+    def sub_conditions(cls,els = [['totalValue',False,50]]) -> pd.DataFrame:
+        sub_matrix = 1
+        try:
+            for el in els:
+                df = element(el[0])
+                sub_matrix *= df
+        except:
+            pass
+        cls.total = (sub_matrix * cls.buy_matrix).apply(lambda x: sub_conditions_optimize(row=x,nums=el[2]),axis = 1, result_type='expand')
 
-        
-    sub_matrix = 1
     @classmethod
-    def sub_conditions(cls,els = [['totalVolume',False,5]]) -> pd.DataFrame:
-        result = 1
-        for el in els:
-            df = element(el[0])
-            result *= df.apply(sub_conditions_optimize,axis = 1,result_type='expand')
-            cls.sub_matrix = result
-
-
-
+    def sell_conditions(cls, conds = None) -> pd.DataFrame:
+        matrix = 1
+        for i in conds:
+            i = i.replace(' and ', '*').replace(' or ', '+')
+            matrix *= eval(i)
+        cls.sell_matrix = matrix
+        cls.order_matrix = cls.total.mask(cls.sell_matrix == 1,-1).apply(order_matrix_optimize,axis = 0)
```

### Comparing `datavns-0.0.4/datavns/data_function.py` & `datavns-0.0.5/datavns/data_function.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,19 +69,19 @@
         `year (int)`: Năm cuối cùng trong danh sách báo cáo tài chính cần lấy
         `quarter (int)`: Quý của báo cáo tài chính cần lấy
             quarter = 0: Sẽ lấy báo cáo tài chính theo năm của doanh nghiệp
             quarter = 1-4: Sẽ lấy báo cáo tài chính theo quý của năm tương ứng với parameter `year`
 
         Return:
         -----
-            pd.Dataframe chứa thông tin về cổ phiếu bao gồm:
-                Các khoản mục của báo cáo tương ứng là columns của DataFrame
-                    Eg: Để xem các khoản mục có thể thực hiện
-                        `bctc('HPG',type=1).columns`
-                Năm báo cáo tương ứng là index của DataFrame
+        pd.Dataframe chứa thông tin về cổ phiếu bao gồm:
+            Các khoản mục của báo cáo tương ứng là columns của DataFrame
+                Eg: Để xem các khoản mục có thể thực hiện
+                    `bctc('HPG',type=1).columns`
+            Năm báo cáo tương ứng là index của DataFrame
     '''
     url_raw = 'https://restv2.fireant.vn/symbols/{}/full-financial-reports?type={}&year={}&quarter={}&limit=999999'.format(cp,type,year,quarter)
     df_raw = rq.get(url_raw,headers=fireant_header).json()
     indexs = [x['name'] for x in df_raw]
     year = [x['year'] for x in df_raw[0]['values']]
     quarter = [x['quarter'] for x in df_raw[0]['values']]
     if quarter != 0:
@@ -146,7 +146,29 @@
                 Eg: Để xem các khoản mục có thể thực hiện
                     `infor('HPG').columns`
     '''
     url = 'https://restv2.fireant.vn/symbols/{}/fundamental'.format(cp)
     df_raw = rq.get(url,headers=fireant_header).json()
     return pd.DataFrame(df_raw,index=[0])
 
+def dividends_historical(cp = 'VCB', num = 50) -> pd.DataFrame:
+    '''
+    In ra dữ liệu về chi trả cổ tức của các doanh nghiệp
+    -----
+
+        Parameter:
+        -----
+        `cp (str)`: Mã cổ phiếu niêm yết
+        `num (int)`: Số năm lấy dữ liệu chi trả cổ tức, tính ngược từ thời điểm hiện tại
+
+        Return:
+        -----
+        pd.Dataframe chứa thông tin về cổ phiếu bao gồm:
+            Năm thực hiện: year
+            Cổ tức tiền mặt: cashDividend
+            Cổ tức cổ phiếu: stockDividend
+            Tổng tài sản doanh nghiệp tại thời điểm chi trả: totalAssets
+            Tổng vốn chủ sở hữu tại thời điểm chi trả: stockHolderEquity
+    '''
+    url = 'https://restv2.fireant.vn/symbols/{}/dividends?count={}'.format(cp,num)
+    df_raw = rq.get(url=url,headers=fireant_header).json()
+    return pd.DataFrame(df_raw).fillna(0)
```

### Comparing `datavns-0.0.4/datavns/headers.py` & `datavns-0.0.5/datavns/headers.py`

 * *Files identical despite different names*

### Comparing `datavns-0.0.4/datavns/indicator.py` & `datavns-0.0.5/datavns/indicator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .data_function import *
 
 
 
 class data_for_backtest:
     @classmethod
-    def take(cls):
+    def take(cls) -> list:
         try:
             with open('file_path.txt', 'r') as file:
                 file_path = file.read()
             with open(file_path + r'\data_price.pkl', 'rb') as file:
                 df_raw = pickle.load(file)
 
             with open(file_path + r'\cps.pkl', 'rb') as file:
@@ -40,25 +40,24 @@
         
         Lưu ý:
         ------
         Nếu dữ liệu chưa được cập nhật sẽ không lấy được data, vui lòng cập nhật dữ liệu
     '''
     try:
         data = [x[el].rename(y) for x,y in zip(data_for_backtest.data,data_for_backtest.cps)]
-        df = pd.DataFrame(data).transpose().sort_index(ascending=True)
+        df = pd.DataFrame(data).transpose().sort_index(ascending=True).fillna(0)
         if stocks == None:
             return df
         else:
             return df.loc[:,stocks]
     except:
         print('Vui lòng cập nhật data phục vụ backtest')
 
 
 
 class indicatior:
-
-    def Moving_Average(method = 'priceClose', period = 20):
+    def Moving_Average(method = 'priceClose', period = 20) -> pd.DataFrame:
 
         return element(method).rolling(window=period).mean()
     
-    def Relative_Streng_Index(method, period ):
+    def Relative_Streng_Index(method, period )-> pd.DataFrame:
         return
```

### Comparing `datavns-0.0.4/datavns/optimize.py` & `datavns-0.0.5/datavns/optimize.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 
 
 
 def order_matrix_optimize(columns):
     '''
     Function dùng optimize cho order matrix
     '''
-    cumulative_sum = 0
     result = []
+    order = 0
+    gap = 2
     for value in columns:
-        cumulative_sum += value
-        if cumulative_sum > 1 :
-            result.append(0)
-            cumulative_sum = 1
-        elif cumulative_sum < 0:
-            result.append(0)
-            cumulative_sum = 0
-        elif cumulative_sum in [0,1]:
-            result.append(value)
+        gap += 1
+        if gap > 2:
+            if order == 0 and value == 1:
+                result.append(value)
+                order = 1
+                gap = 0
+            elif order == 1 and value == -1 :
+                result.append(value)
+                order = 0
+                gap = 0
+            else:
+                result.append(0)
         else:
             result.append(0)
+            
     return result
 
 
 def sub_conditions_optimize(row,nums = 5):
     '''
     Function dùng để optimize điều kiện phụ cho danh mục đầu tư
     '''
```

### Comparing `datavns-0.0.4/datavns/take_data_for_backtest.py` & `datavns-0.0.5/datavns/take_data_for_backtest.py`

 * *Files identical despite different names*

### Comparing `datavns-0.0.4/datavns.egg-info/PKG-INFO` & `datavns-0.0.5/datavns.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datavns
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to collect and backtest the trading strategy on Vietnam stocks market
 Author-email: the-a1pha <buitruonganbta@gmail.com>
 Project-URL: Homepage, https://github.com/the-a1pha/datavns
 Project-URL: Issues, https://github.com/the-a1pha/datavns/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,29 +15,39 @@
 <div align="center">
 
 # **Thư viện thu thập dữ liệu và backtest chiến lược đầu tư**
 # **dữ liệu dựa trên thị trường chứng khoán Việt Nam**
 </div>
 
 
+## Hướng dẫn cài đặt
+
+Để cài đặt package sử dụng câu lệnh:
+
+    pip install datavns
+  
+Để import thư viện vào file và sử dụng
+
+    from datavns import *
 
 ## I. GIỚI THIỆU TỔNG QUAN
 Dự án được thực hiện gồm 2 phần chính
 - Phần một là thu thập dữ liệu về giá cổ phiếu và các thông tin vi mô của doanh nghiệp
 
-- Phần hai là xây dựng hệ thống kiểm thử cho chiến lược cụ thể dựa trên lịch sử giao dịch của cổ phiếu đó
+- Phần hai là xây dựng hệ thống kiểm thử cho chiến lược cụ thể dựa trên lịch sử giao dịch của cổ phiếu và tối ưu hóa danh mục
 
 
 ## II. NỘI DUNG CHÍNH CỦA DỰ ÁN
 
 ### Phần 1: Thu thập dữ liệu
+
 #### 1.1 Thu thập dữ liệu về danh sách cổ phiếu niêm yết
 *Để thu thập dữ liệu về danh sách cổ phiếu theo sàn, chúng ta có thể sử dụng câu lệnh*
 ```python
-list_cp()
+list_cp(exchange = 'HSX')
 ```
 <details>
   <summary>Output</summary>
 
 ```
     Symbol TradeCenterId                                        CompanyName     CategoryName
 0      AAA          HOSE                  Công ty Cổ phần Nhựa An Phát Xanh  Nguyên vật liệu
@@ -57,17 +67,19 @@
 #### 1.2 Thu thập dữ liệu về lịch sử giao dịch của cổ phiếu
 *Để thu thập dữ liệu về thông tin giao dịch của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 price(cp = 'VCB',start_date='2000-01-01',end_date='2024-01-01')
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `start_date (str)`: Ngày bắt đầu trong khoảng thời gian cần lấy thông tin giao dịch
-    `end_date (str)`: Ngày kết thúc trong khoảng thời gian cần lấy thông tin giao dịch
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `start_date (str)`: Ngày bắt đầu trong khoảng thời gian cần lấy thông tin giao dịch
+
+  `end_date (str)`: Ngày kết thúc trong khoảng thời gian cần lấy thông tin giao dịch
 <details>
   <summary>Output</summary>
 
 ```
                   date symbol  priceHigh   priceLow  priceOpen  priceAverage  priceClose  ...  sellQuantity  adjRatio  currentForeignRoom  propTradingNetDealValue  propTradingNetPTValue  propTradingNetValue    unit
 2009-06-30  2009-06-30    VCB  13.753204  13.753204  13.753204     13.753204   13.753204  ...      294070.0   4.36262          82612532.0                      NaN                    NaN                  NaN  1000.0
 2009-07-01  2009-07-01    VCB  14.440864  13.638594  14.440864     13.867814   13.867814  ...     9434870.0   4.36262          82441852.0                      NaN                    NaN                  NaN  1000.0
@@ -86,24 +98,30 @@
 #### 1.3 Thu thập dữ liệu về báo cáo tài chính
 *Để thu thập dữ liệu về báo cáo tài chính của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 bctc('VHM',type=1,year=2023,quarter=4)
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `type (int)`: Loại báo cáo trong báo cáo tài chính cần lấy
-        type = 1: Bảng cân đối kế toán
-        type = 2: Báo cáo kết quả hoạt động kinh doanh
-        type = 3: Báo cáo lưu chuyển tiền tệ trực tiếp (Đa số các doanh nghiệp bị trống dữ liệu về báo cáo lưu chuyển tiền tệ trực tiếp, trừ nhóm ngành ngân hàng)
-        type = 4: Báo cáo lưu chuyển tiền tệ gián tiếp
-    `year (int)`: Năm cuối cùng trong danh sách báo cáo tài chính cần lấy
-    `quarter (int)`: Quý của báo cáo tài chính cần lấy
-        quarter = 0: Sẽ lấy báo cáo tài chính theo năm của doanh nghiệp
-        quarter = 1-4: Sẽ lấy báo cáo tài chính theo quý của năm tương ứng với parameter `year`
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `type (int)`: Loại báo cáo trong báo cáo tài chính cần lấy
+
+      type = 1: Bảng cân đối kế toán
+      type = 2: Báo cáo kết quả hoạt động kinh doanh
+      type = 3: Báo cáo lưu chuyển tiền tệ trực tiếp (Đa số các doanh nghiệp bị trống dữ liệu về báo cáo lưu chuyển tiền tệ trực tiếp, trừ nhóm ngành ngân hàng)
+      type = 4: Báo cáo lưu chuyển tiền tệ gián tiếp
+
+  `year (int)`: Năm cuối cùng trong danh sách báo cáo tài chính cần lấy
+
+  `quarter (int)`: Quý của báo cáo tài chính cần lấy
+
+      quarter = 0: Sẽ lấy báo cáo tài chính theo năm của doanh nghiệp
+      quarter = 1-4: Sẽ lấy báo cáo tài chính theo quý của năm tương ứng với parameter `year`
+
 <details>
   <summary>Output</summary>
 
 ```
 TÀI SẢN A. Tài sản lưu động và đầu tư ngắn hạn I. Tiền và các khoản tương đương tiền           1. Tiền  ... 2. Nguồn kinh phí đã hình thành tài sản cố định 3. Quỹ dự phòng trợ cấp mất việc làm TỔNG CỘNG NGUỒN VỐN Symbol
 2016-4       0                       16491882437206.0                       2802422910160.0    941467410160.0  ...                                             0.0                                  0.0    37520745782451.0    VHM   
 2017-4       0                       44421050167080.0                       1561577770818.0    818341400251.0  ...                                               0                                    0    51303819026055.0    VHM   
@@ -130,23 +148,24 @@
 2023-1       0                      205327661000000.0                       1889644000000.0   1642692000000.0  ...                                             0.0                                  0.0   377621667000000.0    VHM   
 2023-2       0                      190310276000000.0                       5105284000000.0   3829067000000.0  ...                                             0.0                                  0.0   391330538000000.0    VHM   
 2023-3       0                      215057869000000.0                       2909914000000.0   2482981000000.0  ...                                             0.0                                  0.0   417039474000000.0    VHM   
 2023-4       0                      240250006000000.0                      14104131000000.0  13124281000000.0  ...                                             0.0                                  0.0   447360776000000.0    VHM 
 ```
 </details>
 
-#### 1.3 Thu thập dữ liệu về lịch sử chi trả cổ tức
+#### 1.4 Thu thập dữ liệu về lịch sử chi trả cổ tức
 *Để thu thập dữ liệu về lịch sử chi trả cổ tức của của từng cổ phiếu, chúng ta có thể sử dụng câu lệnh*
 ```python
 dividends_historical(cp='VIC',num=20)
 ```
 Trong đó:
 
-    `cp (str)`: Mã cổ phiếu niêm yết
-    `num (int)`: Số năm lấy dữ liệu chi trả cổ tức, tính ngược từ thời điểm hiện tại
+  `cp (str)`: Mã cổ phiếu niêm yết
+
+  `num (int)`: Số năm lấy dữ liệu chi trả cổ tức, tính ngược từ thời điểm hiện tại
 
 <details>
   <summary>Output</summary>
 
 ```
     year  cashDividend  stockDividend   totalAssets  stockHolderEquity
 0   2005           0.0       0.000000  4.891457e+11       3.137832e+11
@@ -167,14 +186,46 @@
 15  2020           0.0       0.000000  4.225038e+14       1.358527e+14
 16  2021           0.0      12.499993  4.283845e+14       1.595719e+14
 17  2022           0.0       0.000000  5.774072e+14       1.356554e+14
 18  2023           0.0       0.000000  6.696171e+14       1.480216e+14
 ```
 </details>
 
+### Phần 2: Backtest
+
+#### 2.1. Tải & lưu dữ liệu phục vụ cho backtest
+
+*Các bước cần thực hiện để tải dữ liệu phục vụ cho quá trình backtest*
+
+* Tạo đường dẫn thư mục đến file dữ liệu backtest
+
+  Chạy file `update_data_for_backtest.py` sau đó chỉ đường dẫn thư mục mong muốn để lưu dữ liệu phục vụ backtest, đường dẫn default đến thư mục sẽ là `D:\Python\datavns\Data`
+
+* Để import dữ liệu vào backtest, sử dụng câu lệnh:
+
+```python
+data_for_backtest.take()
+```
+<details>
+  <summary>Output</summary>
+
+```
+Dữ liệu phục vụ backtest được lưu tại dict: .data
+```
+</details>
+
+#### 2.2. Đối với danh mục đầu tư gồm các cổ phiếu được xác định trước
+
+
+#### 2.3. Đối với danh mục đầu tư được tối ưu hóa tự động
+
+### Phần 3: Các chỉ số đánh giá hiệu quả danh mục
+
+*Đang trong giai đoạn phát triển, vui lòng chờ*
+
```

### Comparing `datavns-0.0.4/pyproject.toml` & `datavns-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 00000060: 2020 2022 6e75 6d70 7922 2c0d 0a20 2020     "numpy",..   
 00000070: 2022 6d61 7470 6c6f 746c 6962 220d 0a20   "matplotlib".. 
 00000080: 2020 205d 0d0a 0d0a 6275 696c 642d 6261     ]....build-ba
 00000090: 636b 656e 6420 3d20 2273 6574 7570 746f  ckend = "setupto
 000000a0: 6f6c 732e 6275 696c 645f 6d65 7461 220d  ols.build_meta".
 000000b0: 0a0d 0a5b 7072 6f6a 6563 745d 0d0a 6e61  ...[project]..na
 000000c0: 6d65 203d 2022 6461 7461 766e 7322 0d0a  me = "datavns"..
-000000d0: 7665 7273 696f 6e20 3d20 2230 2e30 2e34  version = "0.0.4
+000000d0: 7665 7273 696f 6e20 3d20 2230 2e30 2e35  version = "0.0.5
 000000e0: 220d 0a61 7574 686f 7273 203d 205b 0d0a  "..authors = [..
 000000f0: 2020 7b20 6e61 6d65 3d22 7468 652d 6131    { name="the-a1
 00000100: 7068 6122 2c20 656d 6169 6c3d 2262 7569  pha", email="bui
 00000110: 7472 756f 6e67 616e 6274 6140 676d 6169  truonganbta@gmai
 00000120: 6c2e 636f 6d22 207d 2c0d 0a5d 0d0a 6465  l.com" },..]..de
 00000130: 7363 7269 7074 696f 6e20 3d20 2241 2070  scription = "A p
 00000140: 6163 6b61 6765 2074 6f20 636f 6c6c 6563  ackage to collec
```

