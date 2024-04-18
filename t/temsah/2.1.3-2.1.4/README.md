# Comparing `tmp/temsah-2.1.3.tar.gz` & `tmp/temsah-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temsah-2.1.3.tar", last modified: Tue Apr  9 18:15:14 2024, max compression
+gzip compressed data, was "temsah-2.1.4.tar", last modified: Thu Apr 18 14:17:21 2024, max compression
```

## Comparing `temsah-2.1.3.tar` & `temsah-2.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:14.968891 temsah-2.1.3/
--rw-rw-rw-   0        0        0     1095 2024-02-28 08:08:30.000000 temsah-2.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      268 2024-04-09 18:15:14.960914 temsah-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2024-02-23 01:03:41.000000 temsah-2.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 18:15:14.969888 temsah-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      395 2024-04-09 18:14:16.000000 temsah-2.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:14.920500 temsah-2.1.3/temsah/
--rw-rw-rw-   0        0        0       19 2024-02-22 20:21:12.000000 temsah-2.1.3/temsah/__init__.py
--rw-rw-rw-   0        0        0     1656 2024-04-09 18:12:37.000000 temsah-2.1.3/temsah/currency.py
--rw-rw-rw-   0        0        0    14576 2024-03-26 23:24:14.000000 temsah-2.1.3/temsah/data_extractor.py
--rw-rw-rw-   0        0        0     1695 2024-04-09 18:13:31.000000 temsah-2.1.3/temsah/main.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:14.955405 temsah-2.1.3/temsah.egg-info/
--rw-rw-rw-   0        0        0      268 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 14:17:21.220898 temsah-2.1.4/
+-rw-rw-rw-   0        0        0     1095 2024-02-28 08:08:30.000000 temsah-2.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      268 2024-04-18 14:17:21.219900 temsah-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1746 2024-04-09 22:22:13.000000 temsah-2.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 14:17:21.220898 temsah-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      395 2024-04-18 14:15:27.000000 temsah-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:17:21.210318 temsah-2.1.4/temsah/
+-rw-rw-rw-   0        0        0       19 2024-02-22 20:21:12.000000 temsah-2.1.4/temsah/__init__.py
+-rw-rw-rw-   0        0        0     1656 2024-04-09 18:12:37.000000 temsah-2.1.4/temsah/currency.py
+-rw-rw-rw-   0        0        0    16801 2024-04-18 14:15:12.000000 temsah-2.1.4/temsah/data_extractor.py
+-rw-rw-rw-   0        0        0     1695 2024-04-09 18:13:31.000000 temsah-2.1.4/temsah/main.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:17:21.218899 temsah-2.1.4/temsah.egg-info/
+-rw-rw-rw-   0        0        0      268 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/top_level.txt
```

### Comparing `temsah-2.1.3/LICENSE.txt` & `temsah-2.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temsah-2.1.3/README.md` & `temsah-2.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 ## Temsah Python Library
 
-Temsah is a powerful Python library specifically designed for web scraping e-commerce platforms such as Amazon. With its user-friendly interface and extensive functionality, Temsah allows developers to easily extract and collect product information and prices from these websites.
+Temsah is a powerful Python library specifically designed for web scraping e-commerce platforms such as Amazon. With its user-friendly interface and extensive functionality, Temsah allows developers to easily extract and collect product information and prices from these websites.Another usage has also been added to this library , Get the spot price of AED.
 
 ## Installation
 
 You can install Temsah using pip:
 
 ```sh
 pip install temsah
@@ -18,26 +18,40 @@
 import temsah
 ```
 
 Then use the main function of the library to perform web scraping on the desired URL:
 ```sh
 result = temsah.scrape(url)
 ```
+It returns information from scraping e-commerce platforms.
 
+Also to get the spot price in dirhams:
+```sh
+object_currency = Currency()
+data = object_currency.scrape()
+print(data)
+```
+This code will show you an output similar to the output below:
+```sh
+{"AED_currency": "175,340"}
+```
+
+hope you enjoy !
 ## Supported Websites
 
 Temsah provides support for the following e-commerce websites:
 1. [Adidas](https://www.adidas.ae/)
 2. [Nike](https://www.nike.ae/en/home)
 3. [Amazon](https://www.amazon.ae/)
 4. [Namshi](https://www.namshi.com/)
 5. [Sharaf DG](https://uae.sharafdg.com/)
 6. [Noon](https://www.noon.com/uae-en/)
 7. [Carrefour](https://www.carrefouruae.com/)
 
-
+## A website that is scraped to get instant prices
+[tgju.org](https://www.tgju.org/profile/price_aed)
 ## Contact
 
 For any inquiries or contributions to improving this library, please [contact me](mailto:seyedsahel1383@gmail.com "Email Me").
 
 **Note**: This library is continuously being improved, and you are welcome to contribute to its enhancement.
```

### Comparing `temsah-2.1.3/temsah/currency.py` & `temsah-2.1.4/temsah/currency.py`

 * *Files identical despite different names*

### Comparing `temsah-2.1.3/temsah/data_extractor.py` & `temsah-2.1.4/temsah/data_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,39 +195,36 @@
             else:
                 print("price tag not found")
 
         except Exception as e:
             print(f"An error occurred while scraping the URL adidas")
             print(e)
 
+    
     # ---------------------------namshi---------------------------
 
     def namshi(self):
         soup = self.soup
         self.product = Product("namshi")
 
         try:
             # product name
             name=soup.find('h1',class_='ProductConversion_productTitle__F7CGH')
             if name:
                 product_name = name.text
                 self.product.name = product_name.strip()
-            else:
-                print("name tag not found")
 
             # img
             div_tag = soup.find('div', class_='ImageGallery_imageContainer__1yXdp')
             final_src = ""
             if div_tag:
                 img_tag = div_tag.find("img")
                 if img_tag:
                     final_src = f"https://www.namshi.com{img_tag['src']}"
                     self.product.image = final_src
-            else:
-                print("img tag not found")
 
             # price
             section_tag = soup.find('section', class_='ProductPrice_container__ff_N1')
             if section_tag:
                 div_tag = section_tag.find('div', class_='ProductPrice_preReductionPrice__bYwzp')
                 if div_tag:
                     self.product.discount = True
@@ -235,23 +232,70 @@
                     self.product.unit = div_tag.text.strip()[0:3].strip()
                     span_tag=section_tag.find('span', class_='ProductPrice_sellingPrice__cSv1f')
                     self.product.price_in = span_tag.text.strip()[3:].strip()
                 else:
                     self.product.discount = False
                     self.product.price = section_tag.text.strip()[3:].strip()
                     self.product.unit = section_tag.text.strip()[0:3].strip()
-            else:
-                    print("price tag not found")
-            
-            
-            
 
         except Exception as e:
-            print(f"An error occurred while scraping the URL namshi")
-            print(e)
+                print(f"An error occurred while scraping the URL namshi")
+                print(e)
+            
+        if not (self.product.name or self.product.price or self.product.price_out or self.product.price_in or self.product.image):
+            try:
+                # product name
+                name = soup.find("h1", class_="ProductConversion_productTitle__dvlc5")
+                if name:
+                    product_name = name.text
+                    self.product.name = product_name.strip()
+                else:
+                    print("name tag not found")
+
+                # img
+                div_tag = soup.find("div", class_="ImageGallery_imageContainer__jmn93")
+                final_src = ""
+                if div_tag:
+                    img_tag = div_tag.find("img")
+                    if img_tag:
+                        final_src = f"https://www.namshi.com{img_tag['src']}"
+                        self.product.image = final_src
+                else:
+                    print("img tag not found")
+
+                # price
+                span1_tag = soup.find(
+                    "span",
+                    class_="ProductPrice_sellingPrice__y8kib ProductPrice_xLarge__6DRdu",
+                )
+                if span1_tag:
+                    self.product.discount = False
+                    self.product.price = span1_tag.text[3:].strip()
+                    self.product.unit = span1_tag.text.strip()[0:3]
+                else:
+                    self.product.discount = True
+                    div_tag = soup.find(
+                        "div", class_="ProductPrice_preReductionPrice__S72wT"
+                    )  # in discount
+                    if div_tag:
+                        self.product.price_out = div_tag.text.strip()[3:].strip()
+                        self.product.unit = div_tag.text.strip()[0:3].strip()
+                    else:
+                        print("price tag not found")
+                    span_tag = soup.find(
+                        "span",
+                        class_="ProductPrice_sellingPrice__y8kib ProductPrice_discounted__Puxu6 ProductPrice_xLarge__6DRdu",
+                    )
+                    if span_tag:
+                        self.product.price_in = span_tag.text.strip()[3:].strip()
+                    else:
+                        print("price tag not found")
+            except Exception as e:
+                print(f"An error occurred while scraping the URL namshi")
+                print(e)
 
     # ---------------------------sharafdg---------------------------
 
     def sharafdg(self):
         soup = self.soup
         self.product = Product("sharafdg")
```

### Comparing `temsah-2.1.3/temsah/main.py` & `temsah-2.1.4/temsah/main.py`

 * *Files identical despite different names*

