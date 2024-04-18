# Comparing `tmp/codetool-0.18-py3-none-any.whl.zip` & `tmp/codetool-0.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3845 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    12662 b- defN 24-Mar-08 20:57 codetool.py
+Zip file size: 5111 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    17731 b- defN 24-Apr-17 18:05 codetool.py
 -rw-rw-rw-  2.0 fat       29 b- defN 24-Mar-06 11:19 codetool/hash.py
--rw-rw-rw-  2.0 fat      899 b- defN 24-Mar-08 20:58 codetool-0.18.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-08 20:58 codetool-0.18.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Mar-08 20:58 codetool-0.18.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      436 b- defN 24-Mar-08 20:58 codetool-0.18.dist-info/RECORD
-6 files, 14127 bytes uncompressed, 3057 bytes compressed:  78.4%
+-rw-rw-rw-  2.0 fat     1642 b- defN 24-Apr-17 18:11 codetool-0.19.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 18:11 codetool-0.19.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-17 18:11 codetool-0.19.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      437 b- defN 24-Apr-17 18:11 codetool-0.19.dist-info/RECORD
+6 files, 19940 bytes uncompressed, 4323 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: codetool.py
 Comment: 
 
 Filename: codetool/hash.py
 Comment: 
 
-Filename: codetool-0.18.dist-info/METADATA
+Filename: codetool-0.19.dist-info/METADATA
 Comment: 
 
-Filename: codetool-0.18.dist-info/WHEEL
+Filename: codetool-0.19.dist-info/WHEEL
 Comment: 
 
-Filename: codetool-0.18.dist-info/top_level.txt
+Filename: codetool-0.19.dist-info/top_level.txt
 Comment: 
 
-Filename: codetool-0.18.dist-info/RECORD
+Filename: codetool-0.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## codetool.py

```diff
@@ -1,14 +1,44 @@
-__version__=0.18
+__version__=0.19
 def info():
     print("CodeTool",str(__version__))
 carac_id=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z","A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z","0","1","2","3","4","5","6","7","8","9","&","é","#","è","ç","à","@","+","=","ê","ë","$","£","%","ù","µ","*",]
-import random,datetime
+carac_code=carac_code=['8', 'B', 'h', 'o', 'ê', 'M', '[', 'z', '#', 'G', '1', 'Y', 'ç', 'n', 'à', 'D', '{', '~', 'u', 'X', '}', 'i', 'g', 'K', 'Z', ':', '!', '=', '.', '7', '&', '"', '4', 'x', '\\', '0', 'p', '?', '°', '$', 'W', 'E', 'H', ';', 'a', 'ë', 'w', 'y', '5', 'A', 'q', 'r', 'd', '*', 'U', 'I', 'J', '_', '§', '^', '%', 'S', 't', ')', ',', 'b', '3', ' ', 'j', ']', '+', 'é', 'C', 'R', '/', 'P', '6', 'm', 'v', '£', 'V', 'c', 'N', 'è', 'µ', 's', 'L', 'l', '2', 'f', '-', 'Q', 'ù', 'O', 'F', '(', 'k', '9', 'e', 'T', '@']
+class CeasarCode:
+    def __init__(self,key,liste):
+        self.key = key
+        self.liste = liste
+    def encrypt(self,text):
+        encrypted_text=''
+        for char in text:
+            if char in self.liste:
+                shifted_index=(self.liste.index(char) + self.key) % len(self.liste)
+                encrypted_text += self.liste[shifted_index]
+            else:
+                encrypted_text += char
+        return encrypted_text
+    def decrypt(self,text):
+        decrypted_text=''
+        for char in text:
+            if char in self.liste:
+                shifted_index = (self.liste.index(char) - self.key) % len(self.liste)
+                decrypted_text += self.liste[shifted_index]
+            else:
+                decrypted_text += char
+        return decrypted_text
+class KeyLenghtError(Exception):
+    pass
+class LenghtError(Exception):
+    pass
+import random,datetime,time
 def mix(lenght=30):
+    random.seed(generate_key()[random.randint(0,99)])
     random.shuffle(carac_id)
+    if not type(lenght)==int:
+        raise TypeError("Lenght must be a int.")
     start="" 
     for i in range(random.randint(lenght+1,lenght+284)):
         random.seed=int(i*3.1415)
         start=start+random.choice(carac_id)
     startt=start[0:lenght]
     try:
         endd=start[lenght+1::]
@@ -26,14 +56,107 @@
     smonth=int(time[5:6])*2592000
     sday=int(time[8:9])*86400
     shour=int(time[11:12])*3600
     smin=int(time[14:15])*60
     second=int(time[17:18])
     time=str(syear+smonth+sday+shour+smin+second)[0:10]
     return time+"-"+mix(8)+"-"+mix(8)+"-"+mix(8)+"-"+mix(32)+"-1"
+def generate_key():
+    liste=[]
+    while len(liste)!=100:
+        for i in range(100):
+            try:
+                first=int(str(time.time()).split(".")[1][1:6])/int(str(time.time()).split(".")[0])
+                time.sleep(first/5875875)
+                first=str(first)[3:7]
+                first=int(first)
+                liste.append(first)
+            except ValueError:
+                pass
+    random.seed(liste[66])
+    random.shuffle(liste)
+    for i in range(len(liste)):
+        if len(str(liste[i]))==4:
+            pass
+        elif len(str(liste[i]))>4:
+            liste[i]=int(str(liste[i])[0:5])
+        elif len(str(liste[i]))<4:
+            while not len(str(liste[i]))==4:
+                liste[i]=int(str(liste[i])+str(random.randint(0,9)))
+    return liste
+def code(text:str,key:list=generate_key()):
+    if not type(key)==list:
+        raise TypeError("Key must be a list.")
+    if not len(key)==100:
+        raise KeyLenghtError("Key lenght must be 100.")
+    if not type(text)==str:
+        raise TypeError("Text to encode must be a string.")
+    for i in key:
+        if not type(i)==int:
+            raise TypeError("All the number inside the key must integer.")
+    for i in key:
+        if not len(str(i))==4:
+            raise LenghtError("One number isn't the required lenght.")
+    schema=[]
+    for i in range(len(key)):
+        if str(key[i])[0] in ["1","6","8","9"]:
+            schema.append("+")
+        else:
+            schema.append("-")
+    move=0
+    for o in range(len(schema[1::])):
+        if schema[i]=="+":
+            move=move+int(key[o])
+        else:
+            move=move-int(key[o])
+    if str(move).startswith("-"):
+        move=move*-1
+    newtext=CeasarCode(move,carac_code).encrypt(text)
+    return newtext
+def decode(text:str,key:list):
+    if not type(key)==list:
+        raise TypeError("Key must be a list.")
+    if not len(key)==100:
+        raise KeyLenghtError("Key lenght must be 100.")
+    if not type(text)==str:
+        raise TypeError("Text to decode must be a string.")
+    for i in key:
+        if not type(i)==int:
+            raise TypeError("All the number inside the key must integer.")
+    for i in key:
+        if not len(str(i))==4:
+            raise LenghtError("One number isn't the required lenght.")
+    schema=[]
+    for i in range(len(key)):
+        if str(key[i])[0] in ["1","6","8","9"]:
+            schema.append("+")
+        else:
+            schema.append("-")
+    move=0
+    for o in range(len(schema[1::])):
+        if schema[i]=="+":
+            move=move+int(key[o])
+        else:
+            move=move-int(key[o])
+    if str(move).startswith("-"):
+        move=move*-1
+    newtext=CeasarCode(move,carac_code).decrypt(text)
+    return newtext
+if __name__=="__main__":
+    liste=['8', 'B', 'h', 'o', 'ê', 'M', '[', 'z', '#', 'G', '1', 'Y', 'ç', 'n', 'à', 'D', '{', '~', 'u', 'X', '}', 'i', 'g', 'K', 'Z', ':', '!', '=', '.', '7', '&', '"', '4', 'x', '\\', '0', 'p', '?', '°', '$', 'W', 'E', 'H', ';', 'a', 'ë', 'w', 'y', '5', 'A', 'q', 'r', 'd', '*', 'U', 'I', 'J', '_', '§', '^', '%', 'S', 't', ')', ',', 'b', '3', ' ', 'j', ']', '+', 'é', 'C', 'R', '/', 'P', '6', 'm', 'v', '£', 'V', 'c', 'N', 'è', 'µ', 's', 'L', 'l', '2', 'f', '-', 'Q', 'ù', 'O', 'F', '(', 'k', '9', 'e', 'T', '@']
+    text=""
+    import random
+    for i in range(500):
+        text=text+liste[random.randint(0,len(liste)-1)]
+    t=generate_key()
+    print(t)
+    c=code("hello",key=t)
+    print(c)
+    d=decode(c,t)
+    print(d)
 
 #Secure_id
 
 import random
 from random import sample
 lettremin=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z"]
 lettremaj=["A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z"]
@@ -306,8 +429,8 @@
             if str((hash_carac.index(text[i])+8192)**8192).endswith("0"):
                 cara=str((hash_carac.index(text[i])+8192)**8192)[::str((hash_carac.index(text[i])+8192)**8192).index("0")]
             else:
                 cara=str((hash_carac.index(text[i])+8192)**8192)
                 newtext=newtext+cara
         else:
             raise HashintError("'"+car+"' is not hashable")
-    return newtext
+    return newtext
```

## Comparing `codetool-0.18.dist-info/METADATA` & `codetool-0.19.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codetool
-Version: 0.18
+Version: 0.19
 Summary: Id generation, hash and encryption
 Author: lolo859
 Keywords: code,tool,codetool,hash,id,cdtl
 Classifier: Natural Language :: French
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Code Generators
 
@@ -22,10 +22,32 @@
 Functions
 ---------
 
 CodeTool reunites the indecode, hashint and secure_id as well as new functions for generating new types of ID, new methods of encryption, new hash algoryths and more.
 
 CodeTool provide all this functions :
 
-- mix(lenght:int=30) : return a mix of caracters with the lenght provided, default to 30
+- mix(lenght:int=30) : return a mix of caracters with the lenght provided, default to 30, in the form of a string
 
-- universal_id1() : return a new type of unique identifier
+- universal_id1() : return a new type of unique identifier in the form of a string
+
+- generate_key() : return a new type of key in the form of list
+
+- code(text:str,key:list=generate_key()) : need a text to encod in the form of a string and a key generate by the generate_key() function, return the incoded text
+
+- decode(text:str,key:list) : need the encoded text generate by the code() function and the key to decrypt it, return the decoded text
+
+Class
+-----
+
+CodeTool provide all this class:
+
+- CeasarCode(key,list) : allow you to encode text by providing an alphabet in the form of list in the list argument and a key in the form of int in the key argument
+
+Exceptions
+----------
+
+CodeTool can raise all this errors :
+
+- LenghtError
+
+- KeyLenghtError
```

