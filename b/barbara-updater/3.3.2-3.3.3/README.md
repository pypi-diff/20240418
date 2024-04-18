# Comparing `tmp/barbara_updater-3.3.2.tar.gz` & `tmp/barbara_updater-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barbara_updater-3.3.2.tar", last modified: Fri Apr 12 03:10:33 2024, max compression
+gzip compressed data, was "barbara_updater-3.3.3.tar", last modified: Thu Apr 18 01:16:04 2024, max compression
```

## Comparing `barbara_updater-3.3.2.tar` & `barbara_updater-3.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-12 03:10:33.308236 barbara_updater-3.3.2/
--rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-12 03:10:33.308236 barbara_updater-3.3.2/PKG-INFO
--rw-r--r--   0 santod    (1000) santod    (1000)   235072 2024-04-12 03:03:47.000000 barbara_updater-3.3.2/barbara3.py
-drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-12 03:10:33.308236 barbara_updater-3.3.2/barbara_updater.egg-info/
--rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-12 03:10:33.000000 barbara_updater-3.3.2/barbara_updater.egg-info/PKG-INFO
--rw-r--r--   0 santod    (1000) santod    (1000)      176 2024-04-12 03:10:33.000000 barbara_updater-3.3.2/barbara_updater.egg-info/SOURCES.txt
--rw-r--r--   0 santod    (1000) santod    (1000)        1 2024-04-12 03:10:33.000000 barbara_updater-3.3.2/barbara_updater.egg-info/dependency_links.txt
--rw-r--r--   0 santod    (1000) santod    (1000)        9 2024-04-12 03:10:33.000000 barbara_updater-3.3.2/barbara_updater.egg-info/top_level.txt
--rw-r--r--   0 santod    (1000) santod    (1000)       38 2024-04-12 03:10:33.308236 barbara_updater-3.3.2/setup.cfg
--rw-r--r--   0 santod    (1000) santod    (1000)      327 2024-02-23 03:13:41.000000 barbara_updater-3.3.2/setup.py
+drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-18 01:16:04.259585 barbara_updater-3.3.3/
+-rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-18 01:16:04.259585 barbara_updater-3.3.3/PKG-INFO
+-rw-r--r--   0 santod    (1000) santod    (1000)   237997 2024-04-18 01:08:58.000000 barbara_updater-3.3.3/barbara3.py
+drwxr-xr-x   0 santod    (1000) santod    (1000)        0 2024-04-18 01:16:04.259585 barbara_updater-3.3.3/barbara_updater.egg-info/
+-rw-r--r--   0 santod    (1000) santod    (1000)      100 2024-04-18 01:16:04.000000 barbara_updater-3.3.3/barbara_updater.egg-info/PKG-INFO
+-rw-r--r--   0 santod    (1000) santod    (1000)      176 2024-04-18 01:16:04.000000 barbara_updater-3.3.3/barbara_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)        1 2024-04-18 01:16:04.000000 barbara_updater-3.3.3/barbara_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)        9 2024-04-18 01:16:04.000000 barbara_updater-3.3.3/barbara_updater.egg-info/top_level.txt
+-rw-r--r--   0 santod    (1000) santod    (1000)       38 2024-04-18 01:16:04.259585 barbara_updater-3.3.3/setup.cfg
+-rw-r--r--   0 santod    (1000) santod    (1000)      327 2024-02-23 03:13:41.000000 barbara_updater-3.3.3/setup.py
```

### Comparing `barbara_updater-3.3.2/barbara3.py` & `barbara_updater-3.3.3/barbara3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-# 4/11/24 done - password protect escape key
-# increase security. password protect escape key, store email, terminal password
-# fixed 4-10E-24.py rewritten reg sat code to accommodate dark borders all views
-# accidentally may have fixed problem with reg sat and two streams while
-# working on resizing the two smaller reg sat views
-# adjust code at end of try/except in reg sat functions to prevent two streams
-# applied threading to lighting and station plot
+# 4/17B/24 working well. Still need to fill gap betwx lcl radar / reg sat
+# fixed gap baro to lcl radar, but now other previous imgs need to be destroyed 
+# 4/17/24 will begin again to work on 4/17A/24 on gaps to station plot, to local radar from baro
+# 4/17/24 patched failed attempts to fill gaps working well fixed transition from reg sat to sonde
+# after filling image gaps problems with baro overlapping after changing maps & ntl sfc map after 3 hours
+# 4/15/24 adding new try/except blocks to reg sat to avoid lock ups
+# 4/15/24 not done transition from baro trace to lcl radar. Not smooth every time
+# 4/15/24 not done transition from ntl sfc to new or recycled station plots
+# 4/14/24 covered delay ntl sat to reg sat
+# 4/14/24 covered delay lcl radar to lightning and ntl radar directly to lightning
+# 4/14/24 try to cover blank screens by allowing previous image to linger
 # versions after this mostly a waste of time until 4/10/24 
-# threading working for lcl radar and reg sat, but still no display before reg sat
-# fixed with NWS API a problem with baro_input out of nowhere. Can't print line 2870
-# work to include more responsiveness and leave image up before reg sat loop
 # 4/3/24 threading added to scrape, assemble, but not display reg sat loops
-# working to forget ntl radar image just before lcl radar loop ready to display
-# try to extend display of previous image while lcl radar is rendering
-# threading for lcl radar loop is done. Try to thread other heavy tasks
-# 3/25/24 enable functional screenshot button, email is next
 # 3/26/24 email is working - join scraped frame gracefully
-# 3/25/24 Two display buttons set. all button code in show_national_radar
-# done 3/24/24 keyborad to right, focus in tkinter box, larger buttons, remove escape key
-# timeout errors for lightning geopy nominatim may cause hang ups or double
 # scraped frame cycles - consider adding clearing frames function, currently code at
 # start of national radar
 # GUI display with the same keyboard.
 # Use this on a large monitor to take screenshots: grim -g "$(slurp)" screenshot.png
 # This allows you to select an area to capture
 
 #import smbus
@@ -60,14 +54,15 @@
 from geopy.geocoders import Nominatim
 from geopy.distance import geodesic
 from geopy.exc import GeocoderTimedOut
 import urllib.parse
 from geopy.exc import GeocoderUnavailable
 import subprocess
 from selenium import webdriver
+from selenium.common.exceptions import WebDriverException, NoSuchElementException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.chrome.options import Options
 import threading #allows to manage hang ups in solenium
 import tkinter as tk
@@ -133,14 +128,18 @@
 national_radar_hidden = False
 
 # Global variables for images
 img_tk_national_radar = None
 img_label_national_radar = None
 img_label_national_satellite = None
 img_label_satellite = None
+baro_img_label = None
+
+label_delay_for_lightning = None # to manage transition from lcl radar to lightning
+label_lcl_radar = None # to manage transition from ntl radar to lightning this had to be defined too
 
 last_national_radar_scrape_time = None
 last_national_satellite_scrape_time = None
 last_national_sfc_map_scrape_time = None
 last_vorticity_scrape_time = None
 last_sounding_scrape_time = None
 last_station_model_scrape_time = None
@@ -465,26 +464,30 @@
 
     alternative_town_3 = " "
     alternative_state_3 = " "
 
     land_or_buoy()
 
 def change_maps_only():
-    global refresh_flag
+    global refresh_flag, baro_img_label
     refresh_flag = True
-    
+
     transparent_frame.grid_forget()
     
     for widget in transparent_frame.winfo_children():        
         widget.destroy()
         
     scraped_frame.grid_forget()
-    # Don't destroy scraped frame during loop displays will crash        
+    # Don't destroy scraped frame during loop displays will crash       
     baro_frame.grid_forget()
     
+    # baro_img_label hangs in the back if refresh is chosen
+    if baro_img_label and baro_img_label.winfo_exists():
+        baro_img_label.destroy()
+        
     frame1.grid(row=0, column=0, sticky="nsew")
     
     page_choose()
 
 def email_to_maps():
     global refresh_flag
     refresh_flag = False
@@ -494,15 +497,15 @@
     # return to map images
     #Do I need to use lift?
     scraped_frame.grid(row=0, column=0, sticky="nsew")
     transparent_frame.grid(row=0, column=0, sticky="nw")    
 
 def submit_pic_email():
     global email_entry  # Declare the use of the global variable
-
+    
     to_email = email_entry.get()  # Get the email address from the entry widget
     if not to_email:
         print("No email address provided.")
         return
 
     # Email details
     from_email = 'picturesfromtheweatherobserver@gmail.com'
@@ -517,33 +520,32 @@
     msg.attach(MIMEText(body, 'plain'))
 
     # Attach the screenshot
     with open(screenshot_filename, 'rb') as attachment:
         img = MIMEImage(attachment.read(), name=screenshot_filename)
         msg.attach(img)
 
-    # Retrieve the app password
-    email_app_password = os.getenv('EMAIL_APP_PASSWORD')
-    if email_app_password is None:
-        print("App Password not found. Please check the environment variable setting.")
-        return  # Exit the function if the password isn't set
-
+    # For example:
     try:
+        # Connect to Gmail's SMTP server and send the email
         server = smtplib.SMTP_SSL('smtp.gmail.com', 465)
-        server.login(from_email, email_app_password)
+        server.login(from_email, 'apedhdhxnyhkfepv')  # Use your app password
+        #server.login(from_email, os.getenv('EMAIL_APP_PASSWORD'))  # Use the environment variable 
         server.send_message(msg)
         server.quit()
-        print("Email sent successfully")
-
-        # GUI Update on success
+        # Clear the current display
         for widget in frame1.winfo_children():
-            widget.destroy()
+            if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button, tk.Entry)):
+                widget.destroy()
+                
+        # I think these need to stay. 
         transparent_frame.grid_forget()
         scraped_frame.grid_forget()
         baro_frame.grid_forget()
+        
         frame1.grid(row=0, column=0, sticky="nsew")
         root.grid_rowconfigure(0, weight=1)
         root.grid_columnconfigure(0, weight=1)
         root.geometry('1024x600')
 
         label1 = tk.Label(frame1, text="The Weather Observer", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
         label1.grid(row=0, column=0, columnspan=20, padx=50, pady=(50,0), sticky="nw")
@@ -554,60 +556,61 @@
 
         return_text = "Click the button to return to the maps"
         return_label = tk.Label(frame1, text=return_text, font=("Helvetica", 16), bg=tk_background_color, justify="left")
         return_label.grid(row=2, column=0, columnspan=20, padx=50, pady=25, sticky='nw') 
 
         return_button = tk.Button(frame1, text="Return", command=email_to_maps, font=("Helvetica", 16, "bold"))
         return_button.grid(row=3, column=0, columnspan=20, padx=50, pady=(15,0), sticky='nw')
-
-    except Exception as e:
-        print("Failed to send email:", str(e))
         
-        # GUI Update on failure
+    except Exception as e:
+        print("line 538. failed to send email: ", e)
+        # Clear the current display
         for widget in frame1.winfo_children():
-            widget.destroy()
+            if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button, tk.Entry)):
+                widget.destroy()
+        
         transparent_frame.grid_forget()
         scraped_frame.grid_forget()
         baro_frame.grid_forget()
+        
         frame1.grid(row=0, column=0, sticky="nsew")
         root.grid_rowconfigure(0, weight=1)
         root.grid_columnconfigure(0, weight=1)
         root.geometry('1024x600')
 
         label1 = tk.Label(frame1, text="The Weather Observer", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
         label1.grid(row=0, column=0, columnspan=20, padx=50, pady=(50,0), sticky="nw")
 
         not_sent_text = "Your email was not able to be sent"
         not_sent_label = tk.Label(frame1, text=not_sent_text, font=("Helvetica", 16), bg=tk_background_color, justify="left")
         not_sent_label.grid(row=1, column=0, columnspan=20, padx=50, pady=25, sticky='nw')
-
-        try_again_text = "Try another email address or return to the Maps"
-        try_again_label = tk.Label(frame1, text=try_again_text, font=("Helvetica", 16), bg=tk_background_color, justify="left")
-        try_again_label.grid(row=2, column=0, columnspan=20, padx=50, pady=25, sticky='nw')
         
-        email_button = tk.Button(frame1, text="Email", command=submit_pic_email, font=("Helvetica", 16, "bold"))
+        not_sent_text = "Try another email address or return to the Maps"
+        not_sent_label = tk.Label(frame1, text=not_sent_text, font=("Helvetica", 16), bg=tk_background_color, justify="left")
+        not_sent_label.grid(row=2, column=0, columnspan=20, padx=50, pady=25, sticky='nw')
+        
+        email_button = tk.Button(frame1, text="Email", command=pic_email, font=("Helvetica", 16, "bold"))
         email_button.grid(row=3, column=0, columnspan=20, padx=50, pady=(15,0), sticky='nw')
         
         maps_button = tk.Button(frame1, text="Maps", command=email_to_maps, font=("Helvetica", 16, "bold"))
         maps_button.grid(row=3, column=1, columnspan=20, padx=50, pady=(15,0), sticky='nw')
 
-
 def pic_email():
     global email_entry, refresh_flag  # Use the global variable
     refresh_flag = True
     
-    # use this code for rp5 development machine. this strated working for rp4 on 4/11/24
-    subprocess.run(['grim', screenshot_filename])
+#     #use the following line for rp 5 development machine, and Henry's
+#     subprocess.run(['grim', screenshot_filename])
 
     # use the following codes for rp4s in place of subprocess line above
     # Specify the filename for the screenshot
-    #screenshot_filename = 'screenshot.png'
+    screenshot_filename = 'screenshot.png'
     
     # Take the screenshot and overwrite the existing file
-    #subprocess.run(['scrot', screenshot_filename, '--overwrite']) 
+    subprocess.run(['scrot', screenshot_filename, '--overwrite']) 
 
     # Clear the current display
     for widget in frame1.winfo_children():
         if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button, tk.Entry, tk.Radiobutton)):
             widget.destroy()
             
     # I think I need these. Maybe not if I do frame1.left()
@@ -2257,40 +2260,35 @@
             reg_sat_choice_variables = [var.get() for var in choice_vars]
             for index, value in enumerate(reg_sat_choice_variables):
                 if value == 1:
                     # Adjust the values as needed based on your requirements
                     #reg_sat_choice_variables[index] = 2 if index in {10} else 1
                     reg_sat_choice_variables[index] = 1
                     has_submitted_choice = True
-             
-            # Clear the current display                    
-            for widget in frame1.winfo_children():
-                if isinstance(widget, (tk.Checkbutton, tk.Label, tk.Button)):                            
-                    widget.destroy()
                     
             # Clear the current display
             for widget in frame1.winfo_children():
                 widget.destroy()
             
-            # Destroy all checkboxes
-            for checkbox in choice_check_buttons:
-                checkbox.destroy()
-                
-            if box_variables[8] == 1:
+            frame1.grid(row=0, column=0, sticky="nsew")
+            frame1.config(width=1024, height=600)
+ 
+            # destroy these frames to clean layout
+            column1_frame.destroy()
+            column2_frame.destroy()
+            column3_frame.destroy()
                 
-                choose_radiosonde_site()            
-            
+            if box_variables[8] == 1:                
+                choose_radiosonde_site()                        
             else:
                 station_center_input()
             # Print the values of the checkbox choices
             #for i, value in enumerate(reg_sat_choice_variables, start=1):
                 #print(f"reg_sat_choice{i}: {value}")
 
-        submit_frame = tk.Frame(frame1)
-        submit_frame.grid(row=4, column=0, padx=0, pady=10, sticky='se')
         submit_button = tk.Button(frame1, text="Submit", command=submit_sat_choice, font=("Arial", 14, "bold"))
         submit_button.grid(row=4, column=3)
 
 # Define submit_choices at the top level
 def submit_choices():
     global box_variables
     box_variables = [var.get() for var in page_choose_choice_vars]
@@ -2919,29 +2917,29 @@
  
     # Continue with other actions or functions as needed
     land_or_buoy()
 
 frame1.grid(row=0, column=0, sticky="nsew")
 
 # First line (bold)
-label1 = tk.Label(frame1, text="Welcome to The Weather Observer v3.3.2", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
+label1 = tk.Label(frame1, text="Welcome to The Weather Observer v3.3.3", font=("Arial", 18, "bold"), bg=tk_background_color, justify="left")
 label1.grid(row=0, column=0, padx=50, pady=(50, 10), sticky="w")
 
 # Main block of text including the question
 info_text = f'''
 In order to begin, your new instrument needs to be calibrated,
 and you need to make choices about which weather to observe.
 
-The nearest NWS Observation site found is:
+Your Wifi router indicates that you are near:
 {aobs_site}
 
 This site will be used to calibrate the first barometric pressure reading.
 The current barometric pressure reading there is: {baro_input:.2f} inches.
 
-Do you want to keep the default calibration site,
+Do you want to keep the this default calibration site,
 change to another site, or
 enter your own barometric pressure?
 '''
 
 label2 = tk.Label(frame1, text=info_text, font=("Arial", 16), bg=tk_background_color, justify="left")
 label2.grid(row=1, column=0, padx=50, pady=(0, 10), sticky='w')
 
@@ -3961,17 +3959,21 @@
     gif.close()
 
     return output.getvalue()
 
 #@profile
 def display_national_radar():
     try:
-        global last_national_radar_scrape_time
+        global last_national_radar_scrape_time, baro_img_label
         global img_label_national_radar, img_tk_national_radar, national_radar_hidden
 
+        # destroy baro image if it's been saved for lcl radar, but lcl radar not used
+        if baro_img_label and baro_img_label.winfo_exists():
+            baro_img_label.destroy()
+            
         # Check if 10 minutes have passed since the last scrape or if it's the first time
         current_time = datetime.now()
         if last_national_radar_scrape_time is None or (current_time - last_national_radar_scrape_time).total_seconds() >= 600:
             #print("Getting new national radar. time ", current_time)
             radar_url = 'https://radar.weather.gov/ridge/standard/CONUS_0.gif'
             response = requests.get(radar_url)
 
@@ -4027,26 +4029,26 @@
         show_local_radar_loop()
         
 #@profile
 def hide_national_radar():
     global img_label_national_radar, national_radar_hidden
     global img_tk_national_radar  # Declare img_tk_national_radar as a global variable
 
-    if img_label_national_radar and box_variables[2] != 1 and img_label_national_radar.winfo_exists():
+    if img_label_national_radar and box_variables[2] != 1 and box_variables [3] != 1 and img_label_national_radar.winfo_exists():
         # flag established to track whether img_label_national_radar is forgotten to smooth displays
         national_radar_hidden = True
 
         img_label_national_radar.grid_forget()
 
     show_local_radar_loop()
     
 #@profile
 def show_national_radar():
     global img_tk_national_radar, img_label_national_radar, last_forget_clock, last_national_radar_scrape_time, last_national_sfc_map_scrape_time, last_station_model_scrape_time, last_sounding_scrape_time, last_vorticity_scrape_time, last_national_satellite_scrape_time  # Declare global variables
-
+    global baro_img_label
     # Code to forget images every set amount of time
     current_time = datetime.now()
 
     # Ensure last_forget_clock is initialized
     if last_forget_clock is None:
         last_forget_clock = current_time
 
@@ -4092,14 +4094,17 @@
     reboot_button.grid(row=1, column=0, padx=15, pady=(500,0), sticky='nw')
 
     if box_variables[1] == 1 and refresh_flag == False:
         # Clear previous image label
         if img_label_national_radar and img_label_national_radar.winfo_exists():
             img_label_national_radar.destroy()
         
+        if baro_img_label and baro_img_label.winfo_exists():
+            baro_img_label.destroy()
+        
         # show_national_satellite()
         display_national_radar()
     else:
         #show_local_radar_loop()
         show_local_radar_loop()
 
 # Code begins for lcl radar loop
@@ -4176,23 +4181,26 @@
     num_cycles = 4
     extended_display_duration = 6000 
 
     # Reverse the order of resized_images to start with the oldest
     reversed_images = list(reversed(resized_images))
 
     def display_next_image(index=0, cycle=0):
-        global img_label_national_radar
+        global img_label_national_radar, baro_img_label
         global national_radar_hidden  # Refer to the flag
         # Forget national radar image before lcl radar loop is displayed, only once
         #if not national_radar_hidden and img_label_national_radar and img_label_national_radar.winfo_exists():
         if national_radar_hidden == False and img_label_national_radar and img_label_national_radar.winfo_exists():    
 
             img_label_national_radar.grid_forget()
             national_radar_hidden = True  # Set the flag to True after hiding
         
+        if baro_img_label and baro_img_label.winfo_exists():
+            baro_img_label.destroy()
+        
         try:
             if index < len(reversed_images):  # Use reversed_images here
                 label_lcl_radar.config(image=reversed_images[index])  # And here
                 label_lcl_radar.image = reversed_images[index]  # And also here
                 root.after(frame_duration, display_next_image, index + 1, cycle)
             elif cycle + 1 < num_cycles:
                 root.after(pause_duration, display_next_image, 0, cycle + 1)
@@ -4217,17 +4225,21 @@
             print("line 4121. on way to show_lightning")
             show_lightning()
     else:
         print("Error: Unable to find working URLs.")
 
 
 def hide_local_radar_loop(label_lcl_radar):
-    # Directly use 'label_lcl_radar' to check if it exists and forget it from the grid layout
-    if label_lcl_radar and label_lcl_radar.winfo_exists():
+    # Directly use 'label_lcl_radar' to check if it exists and forget it from the grid layout        
+    if label_lcl_radar and box_variables[3] != 1 and box_variables[5] != 1 and label_lcl_radar.winfo_exists():
         label_lcl_radar.grid_forget()
+        
+    if label_lcl_radar and box_variables[3] == 1:
+        global label_delay_for_lightning
+        label_delay_for_lightning == label_lcl_radar
     
     # Proceed to the next function in your application's flow
     show_lightning()
 
 
 def display_local_radar_loop():
     global label_lcl_radar
@@ -4239,106 +4251,99 @@
 
     # Start checking URLs in a background thread
     start_check_url_lcl_radar_thread(lcl_radar_current_time, on_urls_checked)
 
 
 #@profile
 def show_local_radar_loop():
-    #global refresh_flag
+    global label_lcl_radar, label_delay_for_lightning
+    
+    # when change maps is chosen need to get rid of old images if they exist
+    if label_lcl_radar and label_lcl_radar.winfo_exists():
+        label_lcl_radar.grid_forget()
+        
+    if label_delay_for_lightning and label_delay_for_lightning.winfo_exists():
+        label_delay_for_lightning.grid_forget()
+    
     if box_variables[2] == 1 and refresh_flag == False :
         # show_national_satellite()
         display_local_radar_loop()
     else:
         show_lightning()
         
 # Code for lightning
 #@profile
 def display_lightning():
-    global img_tk_lightning  # Declare img_tk_lightning as a global variable
-    
+    global img_tk_lightning
+
     lightning_current_time = datetime.now()
-    
     MAX_RETRIES = 2  # Maximum number of retries in case of failures
 
     def capture_screenshot(lightning_url):
-        global img_tk_lightning  # Declare img_tk_lightning as a nonlocal variable
-         
+        global img_tk_lightning, label_delay_for_lightning, label_lcl_radar, img_label_national_radar 
+
         try:
-                         
             for _ in range(MAX_RETRIES):
-            
-                # Configure Chrome options for headless mode
-                chrome_options = Options()
-                chrome_options.add_argument("--headless")
-                chrome_options.add_argument("--disable-gpu")
-
-                # Use the system-installed ChromeDriver executable
-                driver = webdriver.Chrome(service=Service("chromedriver"), options=chrome_options)
-
-                # Navigate to the URL
-                driver.get(lightning_url)
-
-                # Wait for the "Got it!" button to be clickable
-                wait = WebDriverWait(driver, 15)
-                got_it_button = wait.until(EC.element_to_be_clickable((By.XPATH, "//a[@class='cc-btn cc-dismiss']")))
-
-                # Click the "Got it!" button
-                got_it_button.click()
-
-                time.sleep(5)
-
-                # Capture a screenshot of the entire page
-                lightning_screenshot = driver.get_screenshot_as_png()
-
-                # Close the WebDriver
-                driver.quit()
-
-                # Display the screenshot using PIL
-                lightning_screenshot_image = Image.open(BytesIO(lightning_screenshot))
-                # Crop 46 units from the left side
-                crop_box = (46, 0, lightning_screenshot_image.width, lightning_screenshot_image.height - 90)
-                lightning_screenshot_crop = lightning_screenshot_image.crop(crop_box)
-
-                # Resize the image to fit the desired dimensions
-                target_width = 800
-                target_height = 515
-                lightning_screenshot_resized = lightning_screenshot_crop.resize((target_width, target_height), Image.LANCZOS)
-
-                # Release memory by deleting intermediate images
-                del lightning_screenshot_image
-                del lightning_screenshot_crop
-                del lightning_screenshot
-
-                # Update the Tkinter GUI with the lightning image
-                img_tk_lightning = ImageTk.PhotoImage(lightning_screenshot_resized)
-                img_label = tk.Label(scraped_frame, image=img_tk_lightning)
-                img_label.image = img_tk_lightning
-                img_label.grid(row=1, column=0, padx=150, pady=80, sticky="se")
-                root.update()  # Update the tkinter window to show the image
-
-                # Use after() to schedule hiding the image after some seconds
-                root.after(15000, lambda: hide_lightning(img_label))
-
-                # Successful execution, break out of the loop
-                break
-
-        except TimeoutError:
-            print("Selenium & Display lightning image: Timeout occurred (15 seconds). Retrying...")
-            pass #decided not to call another function to avoid two cycles of scraped frame
+                try:
+                    chrome_options = Options()
+                    chrome_options.add_argument("--headless")
+                    chrome_options.add_argument("--disable-gpu")
+                    driver = webdriver.Chrome(service=Service("chromedriver"), options=chrome_options)
+                    driver.get(lightning_url)
+
+                    wait = WebDriverWait(driver, 15)
+                    got_it_button = wait.until(EC.element_to_be_clickable((By.XPATH, "//a[@class='cc-btn cc-dismiss']")))
+                    got_it_button.click()
+                    time.sleep(5)
+
+                    lightning_screenshot = driver.get_screenshot_as_png()
+                    driver.quit()
+
+                    try:                        
+                        # Directly use 'label_lcl_radar' to check if it exists and forget it from the grid layout
+                        if box_variables[2] == 1:
+                            if label_lcl_radar and label_lcl_radar.winfo_exists():
+                                label_lcl_radar.grid_forget()
+                            
+                        if img_label_national_radar and img_label_national_radar.winfo_exists():
+                            img_label_national_radar.grid_forget()
+                            
+                        lightning_screenshot_image = Image.open(BytesIO(lightning_screenshot))
+                        crop_box = (46, 0, lightning_screenshot_image.width, lightning_screenshot_image.height - 90)
+                        lightning_screenshot_crop = lightning_screenshot_image.crop(crop_box)
+                        target_width, target_height = 800, 515
+                        lightning_screenshot_resized = lightning_screenshot_crop.resize((target_width, target_height), Image.LANCZOS)
+
+                        del lightning_screenshot_image
+                        del lightning_screenshot_crop
+                        del lightning_screenshot
+
+                        img_tk_lightning = ImageTk.PhotoImage(lightning_screenshot_resized)
+                        img_label = tk.Label(scraped_frame, image=img_tk_lightning)
+                        img_label.image = img_tk_lightning
+                        img_label.grid(row=1, column=0, padx=150, pady=80, sticky="se")
+                        root.update()
+                        root.after(15000, lambda: hide_lightning(img_label))
+                        break
+                    except Exception as img_e:
+                        print(f"Image processing failed: {img_e}")
+
+                except (TimeoutError, NoSuchElementException, WebDriverException) as e:
+                    print(f"Selenium operation failed: {e}")
+                    if isinstance(e, TimeoutError):
+                        print("Retrying...")
+                    else:
+                        break  # No retry for other Selenium-specific issues
         except Exception as e:
-            print("Selenium & Display lightning image:", e)
-            pass #decided not to call another function to avoid two cycles of scraped frame
-            #break  # Break out of the loop in case of other exceptions
+            print(f"Unexpected error in capture_screenshot: {e}")
 
-    # URL of the website to capture
     lightning_url = (
         "https://www.lightningmaps.org/?lang=en#m=oss;t=1;s=200;o=0;b=0.00;ts=0;d=2;dl=2;dc=0;y=" +
         str(lightning_lat) + ";x=" + str(lightning_lon) + ";z=6;"
     )
-
     capture_screenshot(lightning_url)
     
 
 #@profile
 def hide_lightning(img_label):
     # Explicitly set the reference to None and destroy the PhotoImage object
     global img_tk_lightning  
@@ -4358,15 +4363,15 @@
         show_national_satellite()
 
         
 # Code for national satellite
 #@profile
 def display_national_satellite():
     global img_tk_satellite, last_national_satellite_scrape_time, resized_image, img_label_national_satellite
-
+    global label_lcl_radar, label_delay_for_lightning
     # Initialize img_label_national_satellite as None
     img_label_national_satellite = None
 
     try:
         current_time = time.time()
         if last_national_satellite_scrape_time is None or (current_time - last_national_satellite_scrape_time) >= 600:
 
@@ -4416,14 +4421,22 @@
             
             # Set the last scrape time to the current time
             last_national_satellite_scrape_time = current_time
 
             # Explicitly set the reference to None before creating a new PhotoImage
             img_tk_satellite = None
 
+            # get rid of saved images intended to fill gaps
+                
+            if label_lcl_radar and label_lcl_radar.winfo_exists():
+                label_lcl_radar.grid_forget()
+                
+            if label_delay_for_lightning and label_delay_for_lightning.winfo_exists():
+                label_delay_for_lightning.grid_forget()
+
             # Create a new PhotoImage object
             img_tk_satellite = ImageTk.PhotoImage(resized_image)
 
             # Check if the label already exists, if not, create it
             if img_label_national_satellite is None:
                 img_label_national_satellite = tk.Label(scraped_frame, image=img_tk_satellite)
                 img_label_national_satellite.grid(row=1, column=0, padx=150, pady=75, sticky="se")
@@ -4455,15 +4468,16 @@
             root.after(16000, lambda: hide_image(img_label_national_satellite))
 
     except Exception as e:
         print(f"An error occurred: {e}")
         show_reg_sat_loop()
 
 def hide_image(img_label_national_satellite):
-    if img_label_national_satellite and img_label_national_satellite.winfo_exists():
+    
+    if img_label_national_satellite and box_variables[5] != 1 and img_label_national_satellite.winfo_exists():
         img_label_national_satellite.grid_forget()
 
     show_reg_sat_loop()
     
 #@profile
 def show_national_satellite():
     #global refresh_flag
@@ -4565,33 +4579,53 @@
 
         current_time_utc -= timedelta(minutes=5)  # Go back 5 minutes for the next iteration
 
     return urls
 
 def trim_near_black_borders_reg_sat(img, threshold=30):
     """Trim borders that are near-black by dynamically finding the content's bounding box."""
-    # Convert the image to grayscale to simplify finding the border
-    grayscale_img = img.convert("L")
-    # Create a binary image where pixels darker than the threshold are black, others are white
-    binary_img = grayscale_img.point(lambda p: 255 if p > threshold else 0, '1')
-    # Use the binary image to find the bounding box of the content
-    bbox = binary_img.getbbox()
-    if bbox:
-        return img.crop(bbox)
-    return img  # Return the original image if no cropping is needed
+    try:
+        # Convert the image to grayscale to simplify finding the border
+        grayscale_img = img.convert("L")
+    except Exception as e:
+        print(f"Error converting image to grayscale in reg_sat: {e}")
+        return img  # Return the original image in case of error
+
+    try:
+        # Create a binary image where pixels darker than the threshold are black, others are white
+        binary_img = grayscale_img.point(lambda p: 255 if p > threshold else 0, '1')
+    except Exception as e:
+        print(f"Error creating binary image in reg_sat: {e}")
+        return img  # Return the original image in case of error
+
+    try:
+        # Use the binary image to find the bounding box of the content
+        bbox = binary_img.getbbox()
+        if bbox:
+            return img.crop(bbox)
+    except Exception as e:
+        print(f"Error cropping the image in reg_sat: {e}")
+        # Return the original image if there is an error in cropping
+
+    return img  # Return the original image if no cropping is needed or if an exception occurred
 
 
 def scrape_reg_sat_images(urls, sat_goes, sat_reg):
     global img_label_satellite
     images = []
 
     chrome_options = Options()
     chrome_options.add_argument("--headless")
     chrome_options.add_argument("--disable-gpu")
-    driver = webdriver.Chrome(service=Service("chromedriver"), options=chrome_options)
+        
+    try:
+        driver = webdriver.Chrome(service=Service("chromedriver"), options=chrome_options)
+    except Exception as e:
+        print(f"Failed to initialize the driver: {e}")
+        return  # Exit if the driver cannot be initialized
 
     try:
         for url in reversed(urls):  # Iterate over URLs
             try:
                 driver.get(url)
                 if "404 Not Found" in driver.title:
                     print(f"No image found for URL: {url}")
@@ -4616,79 +4650,80 @@
 
     finally:
         driver.quit()
 
     # Your existing code to display images
     display_reg_sat_loop(images)
 
-
-
 # Create a threading lock
 tkinter_lock = threading.Lock()
 
 # Function to display images in a Tkinter window
 def display_reg_sat_loop(images):
-    # Declare img_label_satellite as a global variable
-    global img_label_satellite
-    
+    global img_label_satellite, img_label_national_satellite, label_lcl_radar, label_delay_for_lightning  
+
+    #get rid of previous images if saved to fill gaps
+    if img_label_national_satellite and img_label_national_satellite.winfo_exists():
+        img_label_national_satellite.grid_forget()
+
+    if label_lcl_radar and label_lcl_radar.winfo_exists():
+        label_lcl_radar.grid_forget()
+                
+    if label_delay_for_lightning and label_delay_for_lightning.winfo_exists():
+        label_delay_for_lightning.grid_forget()
+
     try:
-        
-        # Create img_label_satellite only if it's not already created
         if not img_label_satellite:
             img_label_satellite = tk.Label(scraped_frame)
             img_label_satellite.grid(row=1, column=0, padx=250, pady=80, sticky='se')
 
         idx = 0
         reg_sat_num_cycles = 0
 
         def update_image():
             nonlocal idx, reg_sat_num_cycles
-            if idx < len(images):
-                # Acquire the lock before updating the Tkinter widget
-                tkinter_lock.acquire()
-                img_label_satellite.config(image=images[idx])
-                idx += 1
-                tkinter_lock.release()
-
-                scraped_frame.after(100, update_image)  # Schedule the next frame
-            elif reg_sat_num_cycles == 5:
-                scraped_frame.after(2000, hide_reg_sat_loop)
-            else:
-                # Schedule to reset index and increment reg_sat_num_cycles after a 2-second pause
-                def reset_and_continue():
-                    nonlocal idx, reg_sat_num_cycles
-                    idx = 0
-                    reg_sat_num_cycles += 1
-                    update_image()  # Continue with the next image
-
-                scraped_frame.after(2000, reset_and_continue)
+            try:
+                if idx < len(images):
+                    tkinter_lock.acquire()
+                    try:
+                        img_label_satellite.config(image=images[idx])
+                    finally:
+                        tkinter_lock.release()
+                    idx += 1
+                    scraped_frame.after(100, update_image)
+                elif reg_sat_num_cycles == 5:
+                    scraped_frame.after(2000, hide_reg_sat_loop)
+                else:
+                    scraped_frame.after(2000, reset_and_continue)
 
+            except Exception as e:
+                print(f"Error updating image: {e}")
+                scraped_frame.after(1000, show_national_sfc_map)
 
-        # Use grid to specify the row and column, and padx/pady for padding
-        img_label_satellite.grid(row=1, column=0, padx=250, pady=80, sticky='se')
+        def reset_and_continue():
+            nonlocal idx, reg_sat_num_cycles
+            idx = 0
+            reg_sat_num_cycles += 1
+            update_image()
 
-        # Schedule the first call to update_image
         scraped_frame.after(0, update_image)
-        
+
     except Exception as e:
-        print("Line 4553. display_reg_sat_loop", e, "on way to national sfc map")
-        show_national_sfc_map()
-        
+        print(f"Error setting up image loop: {e}")
+        show_national_sfc_map()        
         
 # Function to hide the Tkinter window after displaying images
 def hide_reg_sat_loop():
     global img_label_satellite
     if img_label_satellite:
         img_label_satellite.grid_forget()
         img_label_satellite = None
-        
-        
+                
     show_national_sfc_map()
 
-
 def threaded_satellite_scraping():
     # Place the setup code here if any
     base_url = "https://cdn.star.nesdis.noaa.gov/GOES{}/ABI/SECTOR/{}/GEOCOLOR/"
     num_images_to_scrape = 12
     sat_goes, sat_reg = get_reg_sat_settings()
     urls_to_scrape = generate_sat_reg_urls(base_url.format(sat_goes, sat_reg), num_images_to_scrape, sat_goes, sat_reg)
 
@@ -4756,15 +4791,15 @@
     except Exception as e:
         print("National surface map scrape error:", e, "on way to show_station_models")
         show_station_models()
         
 #@profile
 def hide_national_sfc_map(img_label_sfc_map):
     
-    if img_label_sfc_map and img_label_sfc_map.winfo_exists():
+    if img_label_sfc_map and box_variables[7] != 1 and img_label_sfc_map.winfo_exists():
         img_label_sfc_map.grid_forget()
 
     show_station_models()
     
 #@profile
 def show_national_sfc_map():
     #global refresh_flag
@@ -4774,15 +4809,15 @@
 
         display_national_sfc_map()
     else:
         show_station_models()
         
 #@profile        
 def display_station_models():
-    global station_model_url, zoom_plot, img_tk_station_model, last_station_model_scrape_time
+    global station_model_url, zoom_plot, img_tk_station_model, last_station_model_scrape_time, img_label_sfc_map    
     timeout_seconds = 30
     try:
         # Check if 3 minutes have passed since the last scrape or if it's the first time
         current_timestamp = datetime.now()
         current_time = time.time()
         if last_station_model_scrape_time is None or (current_time - last_station_model_scrape_time) >= 180:
             
@@ -4828,14 +4863,18 @@
 
             # Convert the screenshot to a Tkinter PhotoImage
             station_model_image = Image.open(io.BytesIO(station_model_screenshot))
             station_model_image_crop = station_model_image.crop((42, 0, station_model_image.width, station_model_image.height))
 
             # Set the last scrape time to the current time
             last_station_model_scrape_time = current_time
+            
+            # if previous display saved to fill gap, then get rid of it now
+            if img_label_sfc_map and img_label_sfc_map.winfo_exists():
+                img_label_sfc_map.grid_forget()
 
             # Explicitly set the reference to None before creating a new PhotoImage
             img_tk_station_model = None
 
             # Create a new PhotoImage object
             img_tk_station_model = ImageTk.PhotoImage(station_model_image_crop)
 
@@ -4846,14 +4885,18 @@
 
             root.update()  # Update the tkinter window to show the image
 
             # Use after() to schedule hiding the image after some seconds
             root.after(20000, lambda: hide_station_models(img_label))
 
         else:
+            # get rid of the previous image if posting the recycled station plot map
+            if img_label_sfc_map and img_label_sfc_map.winfo_exists():
+                img_label_sfc_map.grid_forget()
+            
             # If less than 3 minutes have passed, still display the most recently scraped image
             img_label = tk.Label(scraped_frame, image=img_tk_station_model)
             img_label.image = img_tk_station_model
             img_label.grid(row=1, column=0, padx=150, pady=73, sticky="se")
 
             root.update()  # Update the tkinter window to show the image
 
@@ -4993,22 +5036,22 @@
                 # Explicitly set the reference to None before creating a new PhotoImage
                 img_tk_sounding = None
 
                 # Create a new PhotoImage object
                 img_tk_sounding = sound_img_tk
 
                 # Create a label to display the image in the Tkinter window
-                img_label = tk.Label(scraped_frame, image=img_tk_sounding)
-                img_label.image = img_tk_sounding
-                img_label.grid(row=1, column=0, padx=120, pady=90, sticky="se")
+                img_label_sounding = tk.Label(scraped_frame, image=img_tk_sounding)
+                img_label_sounding.image = img_tk_sounding
+                img_label_sounding.grid(row=1, column=0, padx=120, pady=90, sticky="se")
 
                 root.update()  # Update the tkinter window to show the image
 
                 # Use after() to schedule hiding the image after 6 seconds
-                root.after(20000, lambda: hide_sounding(img_label))
+                root.after(20000, lambda: hide_sounding(img_label_sounding))
 
         else:
             # If less than an hour has passed, still display the most recently scraped image
             img_label_sounding = tk.Label(scraped_frame, image=img_tk_sounding)
             img_label_sounding.image = img_tk_sounding
             img_label_sounding.grid(row=1, column=0, padx=115, pady=90, sticky="se")
 
@@ -5087,46 +5130,49 @@
             vort_img_label.grid(row=1, column=0, padx=150, pady=85, sticky="se")
 
             root.update()
             root.after(12000, lambda: hide_vorticity(vort_img_label))
 
         else:
             # If less than an hour has passed, still display the most recently scraped image
-            img_label_vorticity = tk.Label(scraped_frame, image=vort_img_tk)
-            img_label_vorticity.image = vort_img_tk
-            img_label_vorticity.grid(row=1, column=0, padx=150, pady=85, sticky="se")
+            vort_img_label = tk.Label(scraped_frame, image=vort_img_tk)
+            vort_img_label.image = vort_img_tk
+            vort_img_label.grid(row=1, column=0, padx=150, pady=85, sticky="se")
 
             root.update()  # Update the tkinter window to show the image
 
             # Use after() to schedule hiding the image after some seconds
-            root.after(12000, lambda: hide_vorticity(img_label_vorticity))
+            root.after(12000, lambda: hide_vorticity(vort_img_label))
 
     except Exception as e:
         print("Scrape, Save, and Display 500mb vort analysis", e, "on way to display_baro_trace")
         display_baro_trace()
 
-def hide_vorticity(img_label_vorticity):
+def hide_vorticity(vort_img_label):
     global iterate_flag  # Declare iterate_flag as global 
-    if img_label_vorticity and img_label_vorticity.winfo_exists():
-        img_label_vorticity.grid_forget()
+    if vort_img_label and vort_img_label.winfo_exists():
+        vort_img_label.grid_forget()
 
     display_baro_trace()
 
 def show_vorticity():
     #global refresh_flag  # Declare refresh_flag as global
     if box_variables[9] == 1 and refresh_flag == False:
         display_vorticity()
     else:        
         display_baro_trace()
 
 def display_baro_trace():
-    global img_tk  # Declare img_tk as a global variable
-#     print("line 4989. About to test refresh flag at display baro_trace", refresh_flag)
-#     if refresh_flag == False:
-#         print("line 4991. shouldn't be here if refresh_flag is true.", refresh_flag)
+    global baro_img_tk  # Declare baro_img_tk as a global variable
+    global baro_img_label #to manage transition from baro to lcl radar
+    
+    # destroy previous baro_img_label
+    if baro_img_label and baro_img_label.winfo_exists():
+        baro_img_label.destroy()
+    
     try:
         # Path to the image on the Raspberry Pi
         image_path = '/home/santod/baro_trace.png'
 
         # Open the image using PIL
         img = Image.open(image_path)
 
@@ -5134,41 +5180,43 @@
         left_crop_width = 100  # Adjust this value based on your requirements
         img = img.crop((left_crop_width, 0, img.width, img.height))
 
         # Resize the image to fit the window
         img = img.resize((1000, 560), Image.LANCZOS)
 
         # Keep a reference to the image to prevent garbage collection
-        img_tk = ImageTk.PhotoImage(img)
+        baro_img_tk = ImageTk.PhotoImage(img)
 
         # Create a label to display the image
-        img_label = tk.Label(scraped_frame, image=img_tk, bd=0)  # Set the background color to white
-        img_label.image = img_tk
-        img_label.grid(row=1, column=0, padx=110, pady=30, sticky="se")
+        baro_img_label = tk.Label(scraped_frame, image=baro_img_tk, bd=0)  # Set the background color to white
+        baro_img_label.image = baro_img_tk
+        baro_img_label.grid(row=1, column=0, padx=110, pady=30, sticky="se")
 
         root.update()  # Update the tkinter window to show the image
 
         # Use after() to schedule hiding the image after some seconds
-        root.after(20000, lambda: hide_baro_trace(img_label))
+        root.after(20000, lambda: hide_baro_trace(baro_img_label))
 
     except Exception as e:
         print("Display Baro Trace. Line 4343", e, "on way to show_national_radar")
         show_national_radar()
             
 #     else:
 #         show_national_radar()
         
-def hide_baro_trace(img_label):
-    global img_tk, iterate_flag  # Declare img_tk as a global variable
+def hide_baro_trace(baro_img_label):
+    global baro_img_tk, iterate_flag  # Declare baro_img_tk as a global variable
 
-    if img_label and img_label.winfo_exists():
-        img_label.destroy()
+    # experimenting with trying to extend baro while lcl radar or lighintg loads
+    if baro_img_label and box_variables[2] != 1 and baro_img_label.winfo_exists():
+    #if baro_img_label and baro_img_label.winfo_exists():
+        baro_img_label.destroy()
 
     # Reference set to None to allow for garbage collection
-    img_tk = None
+    baro_img_tk = None
     
     iterate_flag = True
     
     root.update_idletasks()  # Explicitly update the layout 
     
     show_national_radar()
```

