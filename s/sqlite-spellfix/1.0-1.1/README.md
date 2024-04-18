# Comparing `tmp/sqlite-spellfix-1.0.tar.gz` & `tmp/sqlite_spellfix-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/karl/code/github/sqlite-spellfix/dist/tmp9fcx2ut1/sqlite-spellfix-1.0.tar", last modified: Fri Feb  5 16:49:17 2021, max compression
+gzip compressed data, was "sqlite_spellfix-1.1.tar", last modified: Thu Apr 18 09:28:24 2024, max compression
```

## Comparing `sqlite-spellfix-1.0.tar` & `sqlite_spellfix-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 karl      (1000) karl      (1000)        0 2021-02-05 16:49:17.000000 sqlite-spellfix-1.0/
--rw-r--r--   0 karl      (1000) karl      (1000)     1422 2021-02-05 16:49:17.000000 sqlite-spellfix-1.0/PKG-INFO
--rw-r--r--   0 karl      (1000) karl      (1000)      880 2020-07-15 08:56:15.000000 sqlite-spellfix-1.0/README.md
--rw-r--r--   0 karl      (1000) karl      (1000)       38 2021-02-05 16:49:17.000000 sqlite-spellfix-1.0/setup.cfg
--rw-r--r--   0 karl      (1000) karl      (1000)      679 2021-02-05 16:48:48.000000 sqlite-spellfix-1.0/setup.py
--rw-r--r--   0 karl      (1000) karl      (1000)   102903 2018-07-13 20:28:54.000000 sqlite-spellfix-1.0/spellfix.c
-drwxr-xr-x   0 karl      (1000) karl      (1000)        0 2021-02-05 16:49:17.000000 sqlite-spellfix-1.0/sqlite_spellfix.egg-info/
--rw-r--r--   0 karl      (1000) karl      (1000)     1422 2021-02-05 16:49:17.000000 sqlite-spellfix-1.0/sqlite_spellfix.egg-info/PKG-INFO
--rw-r--r--   0 karl      (1000) karl      (1000)      204 2021-02-05 16:49:17.000000 sqlite-spellfix-1.0/sqlite_spellfix.egg-info/SOURCES.txt
--rw-r--r--   0 karl      (1000) karl      (1000)        1 2021-02-05 16:49:17.000000 sqlite-spellfix-1.0/sqlite_spellfix.egg-info/dependency_links.txt
--rw-r--r--   0 karl      (1000) karl      (1000)       26 2021-02-05 16:49:17.000000 sqlite-spellfix-1.0/sqlite_spellfix.egg-info/top_level.txt
--rw-r--r--   0 karl      (1000) karl      (1000)      101 2020-07-12 19:59:51.000000 sqlite-spellfix-1.0/sqlite_spellfix.py
+drwxr-xr-x   0 karl      (1000) karl      (1000)        0 2024-04-18 09:28:24.635133 sqlite_spellfix-1.1/
+-rw-r--r--   0 karl      (1000) karl      (1000)     1068 2020-07-15 08:42:01.000000 sqlite_spellfix-1.1/LICENSE
+-rw-r--r--   0 karl      (1000) karl      (1000)     1184 2024-04-18 09:28:24.635133 sqlite_spellfix-1.1/PKG-INFO
+-rw-r--r--   0 karl      (1000) karl      (1000)      964 2023-02-11 18:48:51.000000 sqlite_spellfix-1.1/README.md
+-rw-r--r--   0 karl      (1000) karl      (1000)       38 2024-04-18 09:28:24.635133 sqlite_spellfix-1.1/setup.cfg
+-rw-r--r--   0 karl      (1000) karl      (1000)      679 2024-04-18 09:25:44.000000 sqlite_spellfix-1.1/setup.py
+-rw-r--r--   0 karl      (1000) karl      (1000)   103496 2024-04-18 09:25:20.000000 sqlite_spellfix-1.1/spellfix.c
+drwxr-xr-x   0 karl      (1000) karl      (1000)        0 2024-04-18 09:28:24.635133 sqlite_spellfix-1.1/sqlite_spellfix.egg-info/
+-rw-r--r--   0 karl      (1000) karl      (1000)     1184 2024-04-18 09:28:24.000000 sqlite_spellfix-1.1/sqlite_spellfix.egg-info/PKG-INFO
+-rw-r--r--   0 karl      (1000) karl      (1000)      212 2024-04-18 09:28:24.000000 sqlite_spellfix-1.1/sqlite_spellfix.egg-info/SOURCES.txt
+-rw-r--r--   0 karl      (1000) karl      (1000)        1 2024-04-18 09:28:24.000000 sqlite_spellfix-1.1/sqlite_spellfix.egg-info/dependency_links.txt
+-rw-r--r--   0 karl      (1000) karl      (1000)       26 2024-04-18 09:28:24.000000 sqlite_spellfix-1.1/sqlite_spellfix.egg-info/top_level.txt
+-rw-r--r--   0 karl      (1000) karl      (1000)      101 2020-07-12 19:59:51.000000 sqlite_spellfix-1.1/sqlite_spellfix.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sqlite-spellfix-1.0/PKG-INFO` & `sqlite_spellfix-1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-Metadata-Version: 2.1
-Name: sqlite-spellfix
-Version: 1.0
-Summary: Loadable spellfix1 extension for sqlite
-Home-page: http://github.com/karlb/sqlite-spellfix
-License: UNKNOWN
-Description: # sqlite-spellfix
-        
-        This python package includes a loadable `spellfix1` extension module for sqlite. This allows other python packages to use this extension without requiring dependencies outside of the python ecosystem. For more details on the extension itself, see [the official documentation](https://www.sqlite.org/spellfix1.html).
-        
-        ## Installation
-        
-        ### Latest Release
-        
-        Install the `sqlite-spellfix` package from pypi.
-        
-        ### Current Development Version
-        
-        Install via pip
-        
-        ```sh
-        pip install git+git://github.com/karlb/sqlite-spellfix
-        ```
-        
-        or add this to you requirements.txt:
-        
-        ```
-        git+git://github.com/karlb/sqlite-spellfix
-        ```
-        
-        
-        ## Usage
-        
-        
-        ```python
-        import sqlite3
-        import sqlite_spellfix
-        
-        conn = sqlite3.connect(":memory:")
-        conn.enable_load_extension(True)
-        conn.load_extension(sqlite_spellfix.extension_path())
-        # now use as described in https://www.sqlite.org/spellfix1.html
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# sqlite-spellfix
+
+This python package includes a loadable `spellfix1` extension module for sqlite. This allows other python packages to use this extension without requiring dependencies outside of the python ecosystem. For more details on the extension itself, see [the official documentation](https://www.sqlite.org/spellfix1.html).
+
+## Installation
+
+### Latest Release
+
+Install the `sqlite-spellfix` package from pypi.
+
+### Current Development Version
+
+Install via pip
+
+```sh
+pip install git+https://github.com/karlb/sqlite-spellfix
+```
+
+or add this to you requirements.txt:
+
+```
+git+https://github.com/karlb/sqlite-spellfix
+```
+
+
+## Usage
+
+
+```python
+import sqlite3
+import sqlite_spellfix
+
+conn = sqlite3.connect(":memory:")
+conn.enable_load_extension(True)
+conn.load_extension(sqlite_spellfix.extension_path())
+# now use as described in https://www.sqlite.org/spellfix1.html
+```
+
+## See Also
+* [sqlite-icu python package](https://github.com/karlb/sqlite-icu)
```

### Comparing `sqlite-spellfix-1.0/README.md` & `sqlite_spellfix-1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: sqlite-spellfix
+Version: 1.1
+Summary: Loadable spellfix1 extension for sqlite
+Home-page: http://github.com/karlb/sqlite-spellfix
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sqlite-spellfix
 
 This python package includes a loadable `spellfix1` extension module for sqlite. This allows other python packages to use this extension without requiring dependencies outside of the python ecosystem. For more details on the extension itself, see [the official documentation](https://www.sqlite.org/spellfix1.html).
 
 ## Installation
 
 ### Latest Release
@@ -9,21 +17,21 @@
 Install the `sqlite-spellfix` package from pypi.
 
 ### Current Development Version
 
 Install via pip
 
 ```sh
-pip install git+git://github.com/karlb/sqlite-spellfix
+pip install git+https://github.com/karlb/sqlite-spellfix
 ```
 
 or add this to you requirements.txt:
 
 ```
-git+git://github.com/karlb/sqlite-spellfix
+git+https://github.com/karlb/sqlite-spellfix
 ```
 
 
 ## Usage
 
 
 ```python
@@ -31,7 +39,10 @@
 import sqlite_spellfix
 
 conn = sqlite3.connect(":memory:")
 conn.enable_load_extension(True)
 conn.load_extension(sqlite_spellfix.extension_path())
 # now use as described in https://www.sqlite.org/spellfix1.html
 ```
+
+## See Also
+* [sqlite-icu python package](https://github.com/karlb/sqlite-icu)
```

### Comparing `sqlite-spellfix-1.0/setup.py` & `sqlite_spellfix-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 spellfix1 = Extension("spellfix1", sources=["spellfix.c"])
 
 setup(
     name="sqlite-spellfix",
-    version="1.0",
+    version="1.1",
     description="Loadable spellfix1 extension for sqlite",
     py_modules=["sqlite_spellfix"],
     ext_modules=[spellfix1],
     url="http://github.com/karlb/sqlite-spellfix",
     long_description=long_description,
     long_description_content_type="text/markdown",
     setup_requires=['wheel'],
```

### Comparing `sqlite-spellfix-1.0/spellfix.c` & `sqlite_spellfix-1.1/spellfix.c`

 * *Files 0% similar despite different names*

```diff
@@ -111,17 +111,17 @@
  /* i */ CCLASS_VOWEL,    /* j */ CCLASS_C,       /* k */ CCLASS_C,
  /* l */ CCLASS_L,        /* m */ CCLASS_M,       /* n */ CCLASS_M,
  /* o */ CCLASS_VOWEL,    /* p */ CCLASS_B,       /* q */ CCLASS_C,
  /* r */ CCLASS_R,        /* s */ CCLASS_C,       /* t */ CCLASS_D,
  /* u */ CCLASS_VOWEL,    /* v */ CCLASS_B,       /* w */ CCLASS_B,
  /* x */ CCLASS_C,        /* y */ CCLASS_VOWEL,   /* z */ CCLASS_C,
  /* { */ CCLASS_OTHER,    /* | */ CCLASS_OTHER,   /* } */ CCLASS_OTHER,
- /* ~ */ CCLASS_OTHER,    /*   */ CCLASS_OTHER,   
+ /* ~ */ CCLASS_OTHER,    /*   */ CCLASS_OTHER,
 };
-/* 
+/*
 ** This tables gives the character class for ASCII characters that form the
 ** initial character of a word.  The only difference from midClass is with
 ** the letters H, W, and Y.
 */
 static const unsigned char initClass[] = {
  /*   */ CCLASS_OTHER,    /*   */ CCLASS_OTHER,   /*   */ CCLASS_OTHER,
  /*   */ CCLASS_OTHER,    /*   */ CCLASS_OTHER,   /*   */ CCLASS_OTHER,
@@ -161,15 +161,15 @@
  /* i */ CCLASS_VOWEL,    /* j */ CCLASS_C,       /* k */ CCLASS_C,
  /* l */ CCLASS_L,        /* m */ CCLASS_M,       /* n */ CCLASS_M,
  /* o */ CCLASS_VOWEL,    /* p */ CCLASS_B,       /* q */ CCLASS_C,
  /* r */ CCLASS_R,        /* s */ CCLASS_C,       /* t */ CCLASS_D,
  /* u */ CCLASS_VOWEL,    /* v */ CCLASS_B,       /* w */ CCLASS_B,
  /* x */ CCLASS_C,        /* y */ CCLASS_Y,       /* z */ CCLASS_C,
  /* { */ CCLASS_OTHER,    /* | */ CCLASS_OTHER,   /* } */ CCLASS_OTHER,
- /* ~ */ CCLASS_OTHER,    /*   */ CCLASS_OTHER,   
+ /* ~ */ CCLASS_OTHER,    /*   */ CCLASS_OTHER,
 };
 
 /*
 ** Mapping from the character class number (0-13) to a symbol for each
 ** character class.  Note that initClass[] can be used to map the class
 ** symbol back into the class number.
 */
@@ -185,28 +185,28 @@
 **   * Omit T when followed by CH
 **   * Omit W when followed by R
 **   * Omit D when followed by J or G
 **   * Omit K in KN or G in GN at the beginning of a word
 **
 ** Space to hold the result is obtained from sqlite3_malloc()
 **
-** Return NULL if memory allocation fails.  
+** Return NULL if memory allocation fails.
 */
 static unsigned char *phoneticHash(const unsigned char *zIn, int nIn){
   unsigned char *zOut = sqlite3_malloc64( nIn + 1 );
   int i;
   int nOut = 0;
   char cPrev = 0x77;
   char cPrevX = 0x77;
   const unsigned char *aClass = initClass;
 
   if( zOut==0 ) return 0;
   if( nIn>2 ){
     switch( zIn[0] ){
-      case 'g': 
+      case 'g':
       case 'k': {
         if( zIn[1]=='n' ){ zIn++; nIn--; }
         break;
       }
     }
   }
   for(i=0; i<nIn; i++){
@@ -219,15 +219,15 @@
       }
     }
     c = aClass[c&0x7f];
     if( c==CCLASS_SPACE ) continue;
     if( c==CCLASS_OTHER && cPrev!=CCLASS_DIGIT ) continue;
     aClass = midClass;
     if( c==CCLASS_VOWEL && (cPrevX==CCLASS_R || cPrevX==CCLASS_L) ){
-       continue; /* No vowels beside L or R */ 
+       continue; /* No vowels beside L or R */
     }
     if( (c==CCLASS_R || c==CCLASS_L) && cPrevX==CCLASS_VOWEL ){
        nOut--;   /* No vowels beside L or R */
     }
     cPrev = c;
     if( c==CCLASS_SILENT ) continue;
     cPrevX = c;
@@ -347,15 +347,15 @@
 ** on the end of zB.
 **
 ** Smaller numbers mean a closer match.
 **
 ** Negative values indicate an error:
 **    -1  One of the inputs is NULL
 **    -2  Non-ASCII characters on input
-**    -3  Unable to allocate memory 
+**    -3  Unable to allocate memory
 **
 ** If pnMatch is not NULL, then *pnMatch is set to the number of bytes
 ** of zB that matched the pattern in zA. If zA does not end with a '*',
 ** then this value is always the number of bytes in zB (i.e. strlen(zB)).
 ** If zA does end in a '*', then it is the number of bytes in the prefix
 ** of zB that was deemed to match zA.
 */
@@ -528,15 +528,15 @@
     if( res==(-3) ){
       sqlite3_result_error_nomem(context);
     }else if( res==(-2) ){
       sqlite3_result_error(context, "non-ASCII input to editdist()", -1);
     }else{
       sqlite3_result_error(context, "NULL input to editdist()", -1);
     }
-  }else{ 
+  }else{
     sqlite3_result_int(context, res);
   }
 }
 
 /* End of the fixed-cost edit distance implementation
 ******************************************************************************
 *****************************************************************************
@@ -562,15 +562,15 @@
   u8 nTo;                   /* Number of bytes in aTo */
   u16 iCost;                /* Cost of this transformation */
   char a[4]    ;            /* FROM string followed by TO string */
   /* Additional TO and FROM string bytes appended as necessary */
 };
 
 /*
-** Edit costs for a particular language ID 
+** Edit costs for a particular language ID
 */
 struct EditDist3Lang {
   int iLang;             /* Language ID */
   int iInsCost;          /* Default insertion cost */
   int iDelCost;          /* Default deletion cost */
   int iSubCost;          /* Default substitution cost */
   EditDist3Cost *pCost;  /* Costs */
@@ -793,15 +793,15 @@
       if( pCost==0 ){ rc = SQLITE_NOMEM; break; }
       pCost->nFrom = (u8)nFrom;
       pCost->nTo = (u8)nTo;
       pCost->iCost = (u16)iCost;
       memcpy(pCost->a, zFrom, nFrom);
       memcpy(pCost->a + nFrom, zTo, nTo);
       pCost->pNext = pLang->pCost;
-      pLang->pCost = pCost; 
+      pLang->pCost = pCost;
     }
   }
   rc2 = sqlite3_finalize(pStmt);
   if( rc==SQLITE_OK ) rc = rc2;
   if( rc==SQLITE_OK ){
     int iLang;
     for(iLang=0; iLang<p->nLang; iLang++){
@@ -962,15 +962,15 @@
   assert( iCost>=0 );
   assert( iCost<10000 );
   b = m[j] + iCost;
   if( b<m[i] ) m[i] = b;
 }
 
 /*
-** How much stack space (int bytes) to use for Wagner matrix in 
+** How much stack space (int bytes) to use for Wagner matrix in
 ** editDist3Core().  If more space than this is required, the entire
 ** matrix is taken from the heap.  To reduce the load on the memory
 ** allocator, make this value as large as practical for the
 ** architecture in use.
 */
 #ifndef SQLITE_SPELLFIX_STACKALLOC_SZ
 # define SQLITE_SPELLFIX_STACKALLOC_SZ  (1024)
@@ -980,15 +980,15 @@
 **
 ** If an error occurs, return a negative number which is the error code.
 **
 ** If pnMatch is not NULL, then *pnMatch is set to the number of characters
 ** (not bytes) in z2 that matched the search pattern in *pFrom. If pFrom does
 ** not contain the pattern for a prefix-search, then this is always the number
 ** of characters in z2. If pFrom does contain a prefix search pattern, then
-** it is the number of characters in the prefix of z2 that was deemed to 
+** it is the number of characters in the prefix of z2 that was deemed to
 ** match pFrom.
 */
 static int editDist3Core(
   EditDist3FromString *pFrom,  /* The FROM string */
   const char *z2,              /* The TO string */
   int n2,                      /* Length of the TO string */
   const EditDist3Lang *pLang,  /* Edit weights for a particular language ID */
@@ -1120,15 +1120,15 @@
 
   /* Free memory allocations and return the result */
   res = (int)m[szRow*(n2+1)-1];
   n = n2;
   if( f.isPrefix ){
     for(i2=1; i2<=n2; i2++){
       int b = m[szRow*i2-1];
-      if( b<=res ){ 
+      if( b<=res ){
         res = b;
         n = i2 - 1;
       }
     }
   }
   if( pnMatch ){
     int nExtra = 0;
@@ -1197,15 +1197,15 @@
     dist = editDist3Core(pFrom, zB, nB, pLang, 0);
     editDist3FromStringDelete(pFrom);
     if( dist==(-1) ){
       sqlite3_result_error_nomem(context);
     }else{
       sqlite3_result_int(context, dist);
     }
-  } 
+  }
 }
 
 /*
 ** Register the editDist3 function with SQLite
 */
 static int editDist3Install(sqlite3 *db){
   int rc;
@@ -1291,21 +1291,24 @@
   return nChar;
 }
 
 typedef struct Transliteration Transliteration;
 struct Transliteration {
  unsigned short int cFrom;
  unsigned char cTo0, cTo1, cTo2, cTo3;
+#ifdef SQLITE_SPELLFIX_5BYTE_MAPPINGS
+ unsigned char cTo4;
+#endif
 };
 
 /*
 ** Table of translations from unicode characters into ASCII.
 */
 static const Transliteration translit[] = {
-  { 0x00A0,  0x20, 0x00, 0x00, 0x00 },  /*   to   */
+  { 0x00A0,  0x20, 0x00, 0x00, 0x00 },  /*   to   */
   { 0x00B5,  0x75, 0x00, 0x00, 0x00 },  /* µ to u */
   { 0x00C0,  0x41, 0x00, 0x00, 0x00 },  /* À to A */
   { 0x00C1,  0x41, 0x00, 0x00, 0x00 },  /* Á to A */
   { 0x00C2,  0x41, 0x00, 0x00, 0x00 },  /* Â to A */
   { 0x00C3,  0x41, 0x00, 0x00, 0x00 },  /* Ã to A */
   { 0x00C4,  0x41, 0x65, 0x00, 0x00 },  /* Ä to Ae */
   { 0x00C5,  0x41, 0x61, 0x00, 0x00 },  /* Å to Aa */
@@ -1704,15 +1707,19 @@
 **
 ** The returned string might contain more characters than the input.
 **
 ** Space to hold the returned string comes from sqlite3_malloc() and
 ** should be freed by the caller.
 */
 static unsigned char *transliterate(const unsigned char *zIn, int nIn){
+#ifdef SQLITE_SPELLFIX_5BYTE_MAPPINGS
+  unsigned char *zOut = sqlite3_malloc64( nIn*5 + 1 );
+#else
   unsigned char *zOut = sqlite3_malloc64( nIn*4 + 1 );
+#endif
   int c, sz, nOut;
   if( zOut==0 ) return 0;
   nOut = 0;
   while( nIn>0 ){
     c = utf8Read(zIn, nIn, &sz);
     zIn += sz;
     nIn -= sz;
@@ -1728,14 +1735,19 @@
           zOut[nOut++] = tbl[x].cTo0;
           if( tbl[x].cTo1 ){
             zOut[nOut++] = tbl[x].cTo1;
             if( tbl[x].cTo2 ){
               zOut[nOut++] = tbl[x].cTo2;
               if( tbl[x].cTo3 ){
                 zOut[nOut++] = tbl[x].cTo3;
+#ifdef SQLITE_SPELLFIX_5BYTE_MAPPINGS
+                if( tbl[x].cTo4 ){
+                  zOut[nOut++] = tbl[x].cTo4;
+                }
+#endif /* SQLITE_SPELLFIX_5BYTE_MAPPINGS */
               }
             }
           }
           c = 0;
           break;
         }else if( tbl[x].cFrom>c ){
           xTop = x-1;
@@ -1795,15 +1807,15 @@
   return nChar;
 }
 
 
 /*
 **    spellfix1_translit(X)
 **
-** Convert a string that contains non-ASCII Roman characters into 
+** Convert a string that contains non-ASCII Roman characters into
 ** pure ASCII.
 */
 static void transliterateSqlFunc(
   sqlite3_context *context,
   int argc,
   sqlite3_value **argv
 ){
@@ -1926,15 +1938,15 @@
     sqlite3_int64 iRowid;         /* Rowid for this row */
     char *zWord;                  /* Text for this row */
     int iRank;                    /* Rank for this row */
     int iDistance;                /* Distance from pattern for this row */
     int iScore;                   /* Score for sorting */
     int iMatchlen;                /* Value of matchlen column (or -1) */
     char zHash[SPELLFIX_MX_HASH]; /* the phonehash used for this match */
-  } *a; 
+  } *a;
 };
 
 /*
 ** Construct one or more SQL statements from the format string given
 ** and then evaluate those statements. The success code is written
 ** into *pRc.
 **
@@ -2053,15 +2065,16 @@
     pNew->zDbName = (char*)&pNew[1];
     memcpy(pNew->zDbName, zDbName, nDbName+1);
     pNew->zTableName = sqlite3_mprintf("%s", zTableName);
     pNew->db = db;
     if( pNew->zTableName==0 ){
       rc = SQLITE_NOMEM;
     }else{
-      rc = sqlite3_declare_vtab(db, 
+      sqlite3_vtab_config(db, SQLITE_VTAB_INNOCUOUS);
+      rc = sqlite3_declare_vtab(db,
            "CREATE TABLE x(word,rank,distance,langid, "
            "score, matchlen, phonehash HIDDEN, "
            "top HIDDEN, scope HIDDEN, srchcnt HIDDEN, "
            "soundslike HIDDEN, command HIDDEN)"
       );
 #define SPELLFIX_COL_WORD            0
 #define SPELLFIX_COL_RANK            1
@@ -2097,15 +2110,15 @@
     for(i=3; rc==SQLITE_OK && i<argc; i++){
       if( strncmp(argv[i],"edit_cost_table=",16)==0 && pNew->zCostTable==0 ){
         pNew->zCostTable = spellfix1Dequote(&argv[i][16]);
         if( pNew->zCostTable==0 ) rc = SQLITE_NOMEM;
         continue;
       }
       *pzErr = sqlite3_mprintf("bad argument to spellfix1(): \"%s\"", argv[i]);
-      rc = SQLITE_ERROR; 
+      rc = SQLITE_ERROR;
     }
   }
 
   if( rc && pNew ){
     *ppVTab = 0;
     spellfix1Uninit(0, &pNew->base);
   }else{
@@ -2211,15 +2224,15 @@
   int i;
   const struct sqlite3_index_constraint *pConstraint;
   pConstraint = pIdxInfo->aConstraint;
   for(i=0; i<pIdxInfo->nConstraint; i++, pConstraint++){
     if( pConstraint->usable==0 ) continue;
 
     /* Terms of the form:  word MATCH $str */
-    if( (iPlan & SPELLFIX_IDXNUM_MATCH)==0 
+    if( (iPlan & SPELLFIX_IDXNUM_MATCH)==0
      && pConstraint->iColumn==SPELLFIX_COL_WORD
      && pConstraint->op==SQLITE_INDEX_CONSTRAINT_MATCH
     ){
       iPlan |= SPELLFIX_IDXNUM_MATCH;
       pIdxInfo->aConstraintUsage[i].argvIndex = 1;
       pIdxInfo->aConstraintUsage[i].omit = 1;
     }
@@ -2448,15 +2461,15 @@
       iDist = editdist1(p->zPattern, zK1, 0);
     }
     if( iDist<0 ){
       p->rc = SQLITE_NOMEM;
       break;
     }
     pCur->nSearch++;
-    
+
     /* If there is a "distance < $dist" or "distance <= $dist" constraint,
     ** check if this row meets it. If not, jump back up to the top of the
     ** loop to process the next row. Otherwise, if the row does match the
     ** distance constraint, check if the pCur->a[] array is already full.
     ** If it is and no explicit "top = ?" constraint was present in the
     ** query, grow the array to ensure there is room for the new entry. */
     assert( (p->iMaxDist>=0)==((pCur->idxNum & SPELLFIX_IDXNUM_DIST) ? 1 : 0) );
@@ -2662,15 +2675,15 @@
 
 /*
 ** Called to "rewind" a cursor back to the beginning so that
 ** it starts its output over again.  Always called at least once
 ** prior to any spellfix1Column, spellfix1Rowid, or spellfix1Eof call.
 */
 static int spellfix1Filter(
-  sqlite3_vtab_cursor *cur, 
+  sqlite3_vtab_cursor *cur,
   int idxNum, const char *idxStr,
   int argc, sqlite3_value **argv
 ){
   spellfix1_cursor *pCur = (spellfix1_cursor *)cur;
   int rc;
   pCur->idxNum = idxNum;
   if( idxNum & 1 ){
@@ -2865,15 +2878,15 @@
     char c;
     const char *zConflict = spellfix1GetConflict(db);
 
     if( zWord==0 ){
       /* Inserts of the form:  INSERT INTO table(command) VALUES('xyzzy');
       ** cause zWord to be NULL, so we look at the "command" column to see
       ** what special actions to take */
-      const char *zCmd = 
+      const char *zCmd =
          (const char*)sqlite3_value_text(argv[SPELLFIX_COL_COMMAND+2]);
       if( zCmd==0 ){
         pVTab->zErrMsg = sqlite3_mprintf("NOT NULL constraint failed: %s.word",
                                          p->zTableName);
         return SQLITE_CONSTRAINT_NOTNULL;
       }
       if( strcmp(zCmd,"reset")==0 ){
@@ -2954,15 +2967,15 @@
   spellfix1_vtab *p = (spellfix1_vtab*)pVTab;
   sqlite3 *db = p->db;
   int rc = SQLITE_OK;
   char *zNewName = sqlite3_mprintf("%s", zNew);
   if( zNewName==0 ){
     return SQLITE_NOMEM;
   }
-  spellfix1DbExec(&rc, db, 
+  spellfix1DbExec(&rc, db,
      "ALTER TABLE \"%w\".\"%w_vocab\" RENAME TO \"%w_vocab\"",
      p->zDbName, p->zTableName, zNewName
   );
   if( rc==SQLITE_OK ){
     sqlite3_free(p->zTableName);
     p->zTableName = zNewName;
   }else{
@@ -2992,14 +3005,19 @@
   spellfix1Update,         /* xUpdate */
   0,                       /* xBegin */
   0,                       /* xSync */
   0,                       /* xCommit */
   0,                       /* xRollback */
   0,                       /* xFindMethod */
   spellfix1Rename,         /* xRename */
+  0,                       /* xSavepoint */
+  0,                       /* xRelease */
+  0,                       /* xRollbackTo */
+  0,                       /* xShadowName */
+  0                        /* xIntegrity */
 };
 
 /*
 ** Register the various functions and the virtual table.
 */
 static int spellfix1Register(sqlite3 *db){
   int rc = SQLITE_OK;
@@ -3042,16 +3060,16 @@
 /*
 ** Extension load function.
 */
 #ifdef _WIN32
 __declspec(dllexport)
 #endif
 int sqlite3_spellfix_init(
-  sqlite3 *db, 
-  char **pzErrMsg, 
+  sqlite3 *db,
+  char **pzErrMsg,
   const sqlite3_api_routines *pApi
 ){
   SQLITE_EXTENSION_INIT2(pApi);
 #ifndef SQLITE_OMIT_VIRTUALTABLE
   return spellfix1Register(db);
 #endif
   return SQLITE_OK;
```

### Comparing `sqlite-spellfix-1.0/sqlite_spellfix.egg-info/PKG-INFO` & `sqlite_spellfix-1.1/sqlite_spellfix.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: sqlite-spellfix
-Version: 1.0
+Version: 1.1
 Summary: Loadable spellfix1 extension for sqlite
 Home-page: http://github.com/karlb/sqlite-spellfix
-License: UNKNOWN
-Description: # sqlite-spellfix
-        
-        This python package includes a loadable `spellfix1` extension module for sqlite. This allows other python packages to use this extension without requiring dependencies outside of the python ecosystem. For more details on the extension itself, see [the official documentation](https://www.sqlite.org/spellfix1.html).
-        
-        ## Installation
-        
-        ### Latest Release
-        
-        Install the `sqlite-spellfix` package from pypi.
-        
-        ### Current Development Version
-        
-        Install via pip
-        
-        ```sh
-        pip install git+git://github.com/karlb/sqlite-spellfix
-        ```
-        
-        or add this to you requirements.txt:
-        
-        ```
-        git+git://github.com/karlb/sqlite-spellfix
-        ```
-        
-        
-        ## Usage
-        
-        
-        ```python
-        import sqlite3
-        import sqlite_spellfix
-        
-        conn = sqlite3.connect(":memory:")
-        conn.enable_load_extension(True)
-        conn.load_extension(sqlite_spellfix.extension_path())
-        # now use as described in https://www.sqlite.org/spellfix1.html
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# sqlite-spellfix
+
+This python package includes a loadable `spellfix1` extension module for sqlite. This allows other python packages to use this extension without requiring dependencies outside of the python ecosystem. For more details on the extension itself, see [the official documentation](https://www.sqlite.org/spellfix1.html).
+
+## Installation
+
+### Latest Release
+
+Install the `sqlite-spellfix` package from pypi.
+
+### Current Development Version
+
+Install via pip
+
+```sh
+pip install git+https://github.com/karlb/sqlite-spellfix
+```
+
+or add this to you requirements.txt:
+
+```
+git+https://github.com/karlb/sqlite-spellfix
+```
+
+
+## Usage
+
+
+```python
+import sqlite3
+import sqlite_spellfix
+
+conn = sqlite3.connect(":memory:")
+conn.enable_load_extension(True)
+conn.load_extension(sqlite_spellfix.extension_path())
+# now use as described in https://www.sqlite.org/spellfix1.html
+```
+
+## See Also
+* [sqlite-icu python package](https://github.com/karlb/sqlite-icu)
```

