# Comparing `tmp/ASnake-0.13.37.tar.gz` & `tmp/asnake-0.13.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASnake-0.13.37.tar", last modified: Wed Apr 10 19:33:12 2024, max compression
+gzip compressed data, was "asnake-0.13.38.tar", last modified: Thu Apr 18 16:22:45 2024, max compression
```

## Comparing `ASnake-0.13.37.tar` & `asnake-0.13.38.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/
--rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 ASnake-0.13.37/LICENSE.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-10 19:33:12.597394 ASnake-0.13.37/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 ASnake-0.13.37/README.md
--rw-r--r--   0 ahri      (1002) ahri      (1002)     1495 2024-04-10 19:24:02.000000 ASnake-0.13.37/pyproject.toml
--rw-r--r--   0 ahri      (1002) ahri      (1002)       38 2024-04-10 19:33:12.597394 ASnake-0.13.37/setup.cfg
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/src/
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/src/ASnake/
--rwxr-xr-x   0 ahri      (1002) ahri      (1002)   517000 2024-04-10 19:16:27.000000 ASnake-0.13.37/src/ASnake/ASnake.py
--rw-r--r--   0 ahri      (1002) ahri      (1002)        0 2024-04-10 18:46:25.000000 ASnake-0.13.37/src/ASnake/__init__.py
--rw-r--r--   0 ahri      (1002) ahri      (1002)    19469 2024-04-10 19:29:33.000000 ASnake-0.13.37/src/ASnake/__main__.py
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/src/ASnake/data/
--rw-r--r--   0 ahri      (1002) ahri      (1002)       58 2024-04-10 18:07:02.000000 ASnake-0.13.37/src/ASnake/data/ASnakeAlias.bat
--rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8841 2024-04-10 18:07:02.000000 ASnake-0.13.37/src/ASnake/data/megaTest.asnake
--rw-r--r--   0 ahri      (1002) ahri      (1002)     3398 2024-04-10 18:07:02.000000 ASnake-0.13.37/src/ASnake/data/setAlias.asnake
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/src/ASnake.egg-info/
--rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      405 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/SOURCES.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/dependency_links.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       46 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/entry_points.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/requires.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)        7 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/top_level.txt
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.694346 asnake-0.13.38/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 asnake-0.13.38/LICENSE.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-18 16:22:45.694346 asnake-0.13.38/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 asnake-0.13.38/README.md
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     1495 2024-04-10 19:24:02.000000 asnake-0.13.38/pyproject.toml
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       38 2024-04-18 16:22:45.694346 asnake-0.13.38/setup.cfg
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.691013 asnake-0.13.38/src/
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.691013 asnake-0.13.38/src/ASnake/
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)   526027 2024-04-18 16:12:15.000000 asnake-0.13.38/src/ASnake/ASnake.py
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        0 2024-04-10 18:46:25.000000 asnake-0.13.38/src/ASnake/__init__.py
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    19572 2024-04-11 22:48:22.000000 asnake-0.13.38/src/ASnake/__main__.py
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.694346 asnake-0.13.38/src/ASnake/data/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       58 2024-04-10 18:07:02.000000 asnake-0.13.38/src/ASnake/data/ASnakeAlias.bat
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8841 2024-04-10 18:07:02.000000 asnake-0.13.38/src/ASnake/data/megaTest.asnake
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     3398 2024-04-10 18:07:02.000000 asnake-0.13.38/src/ASnake/data/setAlias.asnake
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.694346 asnake-0.13.38/src/ASnake.egg-info/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      405 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/SOURCES.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/dependency_links.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       46 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/entry_points.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/requires.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        7 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/top_level.txt
```

### Comparing `ASnake-0.13.37/LICENSE.txt` & `asnake-0.13.38/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.37/PKG-INFO` & `asnake-0.13.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASnake
-Version: 0.13.37
+Version: 0.13.38
 Summary: Python optimizing compiler for the ASnake programming language.
 Author: Ahri Fox
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ASnake-0.13.37/README.md` & `asnake-0.13.38/README.md`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.37/pyproject.toml` & `asnake-0.13.38/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.37/src/ASnake/ASnake.py` & `asnake-0.13.38/src/ASnake/ASnake.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from re import compile as REcompile
 from re import search as REsearch
 from re import findall as REfindall
 from re import MULTILINE as REMULTILINE
 from keyword import iskeyword
 from unicodedata import category as unicodeCategory
 
-ASnakeVersion = 'v0.13.37'
+ASnakeVersion = 'v0.13.38'
 __version__ = ASnakeVersion[1:]
 
 def AS_SyntaxError(text=None,suggestion=None,lineNumber=0,code='',errorType='Syntax error'):
     showError=[]
     if text != None:
         showError.append(f'{errorType}:\n\t{text}')
     else:
@@ -118,15 +118,15 @@
     NRANGE  = r'(-?(\d+|\w+(\(.\))?)\.\.\.?(-?\d+|\w+(\(.\))?))|-?\d+ ?to ?-?\d+'
     BUILTINF= r"""(([a-zA-Z_]+\d*|[^\s\d='";()+\-*[\],{}]*|(f|u)?\"[^\"]*\"|(f|u)?\'[^\"\']*\')\.([^\u0000-\u007F\s]|[a-zA-Z_])+([^\u0000-\u007F\s]|[a-zA-Z0-9_])*)+"""
     #COMMAGRP= """(?!\[)(([\[\w\d\]=.-]|(((f|r)?\"[^\"]*\")|((f|r)?\'[^\']*\')))+ ?,)+([\[\]\w\d=.-]|((f|r)?\"[^\"]*\")|((f|r)?\'[^\']*\'))+"""
     TRY     = r'(((try)|(except +([A-Z]\w+|\w+\.\w+)( +as +\w*)?)|(except)|(finally))(( *:?)|( +(do|then))))'
     TYPEWRAP= fr'({"|".join(defaultTypes)})( ?\[\w*\])? *: *(#.*)?(?=\n)'
     TYPE    = '\\s%s\\s'%f'({"|".join(defaultTypes)})'
     LAMBDA  = r'lambda ?(\w* *,?)*:'
-    FSTRFRMT = r': *(?:\=?[><^|%.])?\d+(?:\.\d+)?[dfxsn]?'  # for formatting at end of fstrings brackets
+    FSTRFRMT = r':,? *(?:\=?[><^|%.])?\d+(?:\.\d+)?[dfxsn]?'  # for formatting at end of fstrings brackets
     LISTCOMP= r'\-?\w*: ([^\u0000-\u007F\s]|[a-zA-Z_])([^\u0000-\u007F\s]|[a-zA-Z0-9_])*'
     STRING  = r'((f|u|b)?\"(?:\\\\|\\\"|[^\"])*\")|((f|u|b)?\'(?:\\\\|\\\'|[^\'])*\')'
     #SET    = r'{.+?}'
     LBRACKET= r'{'
     RBRACKET= r'}'
     STRRAW  = r"""f?r((f?\"(\\"|.)+?\")|(f?\'(\\'|.)+?\'))"""
     IMPORT  = r"""(^|(?! )|from +[^'"\n ]*) ?c?import [^\n;]*"""
@@ -210,14 +210,16 @@
     'ELIF':'elif','ELSE':'else','IF':'if','WHILE':'while','GREATEQ':'>=','GREATER':'>','LESS':'<',
     'LESSEQ':'<=','EQUAL':'==','ASSIGN':'=','NOTHING':'pass','NOTEQ':'!=','BUILTINF':'.','OF':'elif',
     'AND':'and','OR':'or','RETURN':'return','FOR':'for','MODULO':'%','EXPONENT':'**','COMMA':',',
     'LISTEND':']','ELLIPSIS':'...','constLPAREN':'(','COLON':':','LINDEX':'[','RINDEX':']',
     "DQUOTE":'"',"SQUOTE":"'", 'LBRACKET':'{','RBRACKET':'}'}
 
     convertType={'int':'NUMBER','float':'NUMBER','Py_ssize_t':'NUMBER','bool':'BOOL','bint':'BOOL','str':'STRING','list':'LIST','dict':'DICT','type':'TYPE','tuple':'TUPLE','set':'SET','bytes':'STRING','object':'ID','range':'FUNCTION','complex':'NUMBER','frozenset':'FUNCTION','bytearray':'STRING','memoryview':'FUNCTION'}
+    cythonConvertType = {'int': 'long long int', 'bool': 'bint', 'float': 'double'}
+    for t in cythonConvertType: convertType[cythonConvertType[t]]=convertType[t]
     typeTypes=tuple([t for t in convertType])
 
     # useful types of sets of tokens or other things
     typeAssignables=('STRING','NUMBER','ID','LIST','LISTEND','DICT','BINARY','LBRACKET','BOOL')
     typeOperators=('PLUS','MINUS','TIMES','DIVIDE','RDIVIDE','EXPONENT','BITWISE','MODULO')
     typeCheckers=('LESS','LESSEQ','GREATEQ','GREATER', 'EQUAL', 'PYIS','NOTEQ')
     typePrintable=typeAssignables+typeOperators+typeCheckers+('LINDEX','RINDEX','INDEX','LPAREN','RPAREN','MODULO','IGNORE','INC','INS','DIVMOD','COMMA','BITWISE')
@@ -450,14 +452,23 @@
                         if ii.type == 'LISTCOMP':
                             insertOrAppend(token,[iii for iii in miniLex(ii.value.split(':')[0])][0])
                             lex[tmpLI].lineno = lineNumber
                             insertOrAppend(token,makeToken(tok, ':', 'COLON'))
                             lex[tmpLI].lineno = lineNumber
                             insertOrAppend(token,[iii for iii in miniLex(ii.value.split(':')[-1])][0])
                             lex[tmpLI].lineno = lineNumber
+                        elif ii.type == 'INDEX':
+                            for iii in miniLex(ii.value[:-1]):
+                                if iii.type == 'ENDIF': iii.type = 'COLON'
+                                elif iii.type == 'LIST': iii.type = 'LINDEX'
+                                elif iii.type in {'LPAREN', 'FUNCTION'}: parenScope += 1
+                                elif iii.type == 'RPAREN': parenScope -= 1
+                                insertOrAppend(token, iii)
+                                lex[tmpLI].lineno = lineNumber
+                            insertOrAppend(token, makeToken(i, ']', 'RINDEX'))
                         else:
                             if   ii.type == 'ENDIF': ii.type = 'COLON'
                             elif ii.type == 'LIST' : ii.type = 'LINDEX'
                             elif ii.type in {'LPAREN','FUNCTION'}: parenScope += 1
                             elif ii.type == 'RPAREN': parenScope -= 1
                             insertOrAppend(token,ii)
                             lex[tmpLI].lineno = lineNumber
@@ -1686,17 +1697,65 @@
                                         tmpf=tmpf[::-1]
                                         if len(tmpf) > 1 and tmpf[-1].type!='LIST' and any(True for i in tmpf if i.type == 'LISTCOMP' )==False:
                                             tmptok=copy(lex[token]) ; tmptok.type='LPAREN' ; tmptok.value='(' ; tmpf.append(tmptok) ; del tmptok
                                             tmptok=copy(lex[token]) ; tmptok.type='RPAREN' ; tmptok.value=')' ; tmpf.insert(0,tmptok) ; del tmptok
                                         tmpListOfVarsInside=tuple([_.value for _ in tmpf if _.type == 'ID']) # for keeping track of vars inside that may change
                                     else: tmpf=[l for l in tmpf if tmpf.type != 'IGNORE']
 
-                                    search=True ; linkType=True if (enforceTyping or compileTo == 'Cython') else False ; ignores=[] ; inDef=False ; wasInDefs=False ; inFrom=False ; inCase=False
+                                    tmpindent = 0  # keeping track if constant is in indented block
+                                    tmpFoundIndent = tmpFoundThen = tmpInTypeWrap = tmpCheckForDef = False
+                                    # tmpCheckForDef when not False, checks to see if inside function before canceling optimization
+                                    tmptmpIndent = 0  # keeping track of backwards current indent
+                                    for tmpi in range(token - 1, 0, -1):
+                                        # checks backwards to make sure its valid, also gets indent
+                                        if lex[tmpi].type == 'TAB':
+                                            if not tmpFoundIndent:
+                                                tmptmpIndent = tmpindent = lex[tmpi].value.replace('\t', ' ').count(' ')
+                                                if lex[tmpi + 1].type in typeConditionals:
+                                                    tmpindent += 1
+                                                tmpFoundIndent = True
+                                            elif lex[tmpi].value.replace('\t', ' ').count(' ') < tmpindent:
+                                                if lex[tmpi + 1].type == 'TYPEWRAP':
+                                                    tmptmpIndent -= 1
+                                        elif lex[tmpi].type == 'NEWLINE':
+                                            if not tmpFoundIndent:
+                                                if lex[tmpi + 1].type == 'TYPEWRAP':
+                                                    tmpindent -= 1
+                                                elif lex[tmpi + 1].type in typeConditionals:
+                                                    tmpindent += 1
+                                                else: tmpindent = 0
+                                                tmpFoundIndent = True
+                                            tmptmpIndent = 0
+                                            if tmpCheckForDef: search = False; break
+                                        # don't check THENs for indent
+                                        elif lex[tmpi].type == 'THEN' and lex[tmpi - 1].type not in {'TAB', 'NEWLINE'}:
+                                            tmpFoundThen = True
+                                        elif lex[tmpi].type == 'TYPEWRAP':
+                                            tmpInTypeWrap = True
+                                        elif tmpindent > tmptmpIndent and lex[tmpi].type == 'ID' and lex[tmpi].value == lex[token].value:
+                                            tmpCheckForDef = True  # previous version of self found on previous indent, bail!
+                                        elif tmpCheckForDef and lex[tmpi].type in {'PYDEF', 'DEFFUNCT'}:
+                                            tmpCheckForDef = False
+                                        #print(lex[token].value, lex[tmpi].type, tmptmpIndent, tmpindent)
+
+                                    def handleIgnoreOnNL():
+                                        nonlocal tmpAddToIgnoresWhenNL, ignores, tmpi
+                                        if tmpAddToIgnoresWhenNL > 0:
+                                            ignores.append(tmpAddToIgnoresWhenNL)
+                                            tmpAddToIgnoresWhenNL = 0
+                                        elif tmpAddToIgnoresWhenNL < 0:
+                                            # when tmpAddToIgnoresWhenNL is negative, use postive version as start and current tmpi as end
+                                            ignores.append((-tmpAddToIgnoresWhenNL,tmpi))
+                                            tmpAddToIgnoresWhenNL = 0
+
+                                    search=True ; linkType=True if (enforceTyping or compileTo == 'Cython') else False ; ignores=[] ; inDef=wasInDefs=inFrom=inCase=tmpInConditionalStatement=False
                                     # wasInDefs is for determining if a later define could break behaviour inside of functions
+                                    # inDef i think is for determining if its the name of a function??
                                     tmpIDshow=0 ; tmpAddToIgnoresWhenNL = 0
+                                    #print('-----')
                                     for tmpi in range(valueStop+1,len(lex)): # check if we can determine its a constant
                                         #print(lex[token].value,search,lex[tmpi].type,lex[tmpi].value,tmpIDshow)
                                         if not search and (enforceTyping and not linkType): break
                                         if lex[tmpi].type=='INC' or (tmpi+1 < len(lex) and lex[tmpi+1].type=='LINDEX' and lex[tmpi].value in (lex[token].value,)+tmpListOfVarsInside) \
                                         or ((lex[tmpi].type in {'ID','INC'} and lex[tmpi].value.replace('++','').replace('--','') in (lex[token].value,)+tmpListOfVarsInside and (lex[tmpi-1].type not in {'ELIF','OF','IF','OR','AND','FSTR'})  ) and lex[tmpi+1].type in typeAssignables+('ASSIGN',) ):
                                             if (lex[tmpi+1].type == 'ASSIGN' and lex[tmpi+2].type == vartype) or lex[tmpi+1].type == vartype or (vartype=='NUMBER' and lex[tmpi].type=='INC'):
                                                 pass
@@ -1723,20 +1782,22 @@
                                                     else:
                                                         # set ignore point at end of line, so that it may still fold onto expression
                                                         for ii in range(tmpi,len(lex)-1):
                                                             if lex[ii].type in typeNewline:
                                                                 tmpAddToIgnoresWhenNL = ii
                                                                 break
 
-                                            if wasInDefs and lex[tmpi+1].type in typeAssignables+('ASSIGN',):
+                                            if not wasInDefs and lex[tmpi+1].type in typeAssignables+('ASSIGN',):
+                                                # wasInDefs used to not have the `not`, I think saying "if we are not in (another) function" makes sense.
+                                                # but because the prior intent is not clear, just be aware of this as a suspect if something breaks later.
                                                 tmpSafe=False
                                                 if lex[tmpi+1].type == 'ASSIGN' and 'is' in lex[tmpi+1].value and determineIfAssignOrEqual(tmpi+1):
                                                     tmpSafe=True ; tmpAddToIgnoresWhenNL=0
                                                 if not tmpSafe:
-                                                    search = False
+                                                    tmpAddToIgnoresWhenNL = tmpi
                                             if lex[token].value == lex[tmpi].value and lex[tmpi+1].type not in typeAssignables+('ASSIGN',): tmpIDshow+=1
 
                                         elif inFrom and lex[tmpi].type == 'ID' and lex[token].value == lex[tmpi].value:
                                             search = False
                                         elif lex[tmpi].type == 'ID' and lex[token].value == lex[tmpi].value and lex[tmpi+1].type == 'COMMA' and lex[tmpi-1].type in typeNewline:
                                             tmptmpParenScope = 0
                                             for tt in range(tmpi,len(lex)-1):
@@ -1768,25 +1829,21 @@
                                         elif lex[tmpi].type == 'BUILTINF' and lex[tmpi].value.split('.')[0] == lex[token].value and '.'+lex[tmpi].value.split('.')[1] in listMods+setUpdateMethods:
                                             search=False ; linkType=False ; break # discards list mods like .append()
                                         elif lex[tmpi].type == 'SCOPE' and lex[token].value in lex[tmpi].value:
                                             search=False ; break # no global var pls
                                         elif lex[tmpi].type == 'META' and lex[token].value in '='.join(lex[tmpi].value.split('=')[1:]):
                                             search=False
                                         elif lex[tmpi].type == 'DEFFUNCT':
-                                            if tmpAddToIgnoresWhenNL > 0:
-                                                ignores.append(tmpAddToIgnoresWhenNL)
-                                                tmpAddToIgnoresWhenNL = 0
+                                            handleIgnoreOnNL()
                                             wasInDefs = True
                                             if lex[tmpi-1].value == lex[token].value:
                                                 inDef=True ; search=False
                                                 ignores.append([tmpi-1])
                                         elif lex[tmpi].type == 'PYDEF':
-                                            if tmpAddToIgnoresWhenNL > 0:
-                                                ignores.append(tmpAddToIgnoresWhenNL)
-                                                tmpAddToIgnoresWhenNL = 0
+                                            handleIgnoreOnNL()
                                             wasInDefs = True
                                             if lex[token].value.strip()+'(' in lex[tmpi].value.strip():
                                                 inDef = True ; search = False
                                                 ignores.append([tmpi])
                                         elif lex[tmpi].type in typeLoop:
                                             if lex[tmpi-1].type == 'TAB':
                                                 tmptmpIndent = lex[tmpi-1].value.count(' ')
@@ -1812,71 +1869,52 @@
                                                 elif lex[tmpii].type == 'INC' and lex[tmpii].value.replace('--','').replace('++','') == lex[token].value:
                                                     ignores.append(tmpi) ; break
                                         elif lex[tmpi].type == 'FROM' and inDef:
                                             search=inFrom=True ; inDef=False
                                             ignores[-1].append(tmpi)
                                         elif lex[tmpi-1].type == 'INS' and lex[tmpi].type == 'ID' and lex[tmpi].value == lex[token].value and vartype == 'DICT':
                                             search=False # dicts don't seem to play well with stuff like enumerate
-                                        elif (not inFrom and not inCase ) and lex[tmpi].type == 'ID' and lex[tmpi].value == lex[token].value and lex[tmpi+1].type != 'ASSIGN':
+                                        elif (not inFrom and not inCase) and lex[tmpi].type == 'ID' and lex[tmpi].value == lex[token].value \
+                                        and (lex[tmpi+1].type != 'ASSIGN' or tmpInConditionalStatement):
                                             tmpIDshow+=1
                                         elif lex[tmpi].type in typeNewline:
-                                            if tmpAddToIgnoresWhenNL > 0:
-                                                ignores.append(tmpAddToIgnoresWhenNL)
-                                                tmpAddToIgnoresWhenNL = 0
+                                            handleIgnoreOnNL()
                                             if inFrom: inFrom=False
                                             inCase=False
+                                            if lex[tmpi].type in {'NEWLINE','TAB'} or (lex[tmpi].type == 'THEN' and tmpInConditionalStatement):
+                                                if lex[tmpi].type == 'THEN' and tmpInConditionalStatement:
+                                                    tttIndent = tmpindent+1
+                                                else:
+                                                    tttIndent = 0 if lex[tmpi].type == 'NEWLINE' else lex[tmpi].value.count(' ')
+                                                #print(tmpindent, tttIndent, ignores)
+                                                if tmpindent > tttIndent: ignores.append(tmpi) ; break
+                                            tmpInConditionalStatement = False
                                         elif lex[tmpi].type == 'IF':
-                                            inCase=False
+                                            inCase=False ; tmpInConditionalStatement=True
                                         elif lex[tmpi].type == 'OF' and 'case' in lex[tmpi].value:
-                                            inCase=True
+                                            inCase=True  ; tmpInConditionalStatement=True
                                         elif lex[tmpi].type == 'FOR' and lex[tmpi-1].type not in {'LINDEX','LIST'} and lex[tmpi+1].value == lex[token].value:
                                             search=False
+                                        elif lex[tmpi].type == 'LAMBDA' and lex[tmpi].value[7:-1] == lex[token].value:
+                                            tmpAddToIgnoresWhenNL=-tmpi
                                     if search:
-                                        if len([True for tmpi in range(token,0,-1) if lex[tmpi].type in {'SCOPE','META'} and lex[token].value in lex[tmpi].value])>0: search=False
+                                        if len([True for tmpi in range(token,0,-1) if lex[tmpi].type == 'SCOPE' and lex[token].value in lex[tmpi].value])>0: search=False
                                         # ^^ no global var pls
                                         elif len([True for tmpi in range(token,0,-1) if lex[tmpi].type == 'TRY' and 'try' in lex[tmpi].value])>len([True for tmpi in range(token,0,-1) if lex[tmpi].type == 'TRY' and 'except' in lex[tmpi].value]): search=False
                                         # ^^ fixes it in cases where the constant is defined in the except
                                         elif tmpIDshow > 1 and not isinstance(tmpf[0],str) and len(tmpf)>1 and (len(tmpf)-2 > 1 and not(len(tmpf)-2==2 and tmpf[2].type=='MINUS' and tmpf[1].type=='NUMBER') ) and vartype!="LIST": search=False
                                         # ^^ when a constant involves operations, its better to compute it once and share the value rather than compute the value in many places.
                                         #if not isinstance(tmpf[0],str): print(search,lex[token].value,[_.value for _ in tmpf],len(tmpf),tmpIDshow)
                                     if search or linkType:
                                         inFrom=False # dont replace constants inside of FROM (function args)
-                                        tmpindent=0 # keeping track if constant is in indented block
                                         ignore=False # ignoring function blocks
                                         inLoop=[False,0]
                                         inCase=False # similar to inFrom ; do not replace constants in OF case statements
 
-                                        tmpFoundIndent=tmpFoundThen=tmpInTypeWrap=False
-                                        tmptmpIndent=0 # keeping track of backwards current indent
-                                        for tmpi in range(token-1,0,-1):
-                                            #print(lex[token].value,lex[tmpi].type,tmptmpIndent,tmpindent)
-                                            # checks backwards to make sure its valid, also gets indent
-                                            if lex[tmpi].type == 'TAB':
-                                                if not tmpFoundIndent:
-                                                    tmptmpIndent=tmpindent=lex[tmpi].value.replace('\t',' ').count(' ')
-                                                    if lex[tmpi+1].type in typeConditionals:
-                                                        tmpindent+=1
-                                                    tmpFoundIndent=True
-                                                elif lex[tmpi].value.replace('\t',' ').count(' ') < tmpindent:
-                                                    if lex[tmpi+1].type == 'TYPEWRAP':
-                                                        tmpindent-=1
-
-                                            elif lex[tmpi].type == 'NEWLINE':
-                                                if not tmpFoundIndent:
-                                                    if lex[tmpi+1].type == 'TYPEWRAP':
-                                                        tmpindent -= 1
-                                                    elif lex[tmpi+1].type in typeConditionals:
-                                                        tmpindent += 1
-                                                tmptmpIndent=0
-                                            # don't check THENs for indent
-                                            elif lex[tmpi].type == 'THEN' and lex[tmpi-1].type not in {'TAB','NEWLINE'}:
-                                                tmpFoundThen=True
-                                            elif lex[tmpi].type == 'TYPEWRAP': tmpInTypeWrap = True
-                                            elif tmpindent > tmptmpIndent and lex[tmpi].type == 'ID' and lex[tmpi].value == lex[token].value:
-                                                search=False ; break # previous version of self found on previous indent, bail!
+
 
                                         if len([True for tmpi in range(token,0,-1) if lex[tmpi].type == 'TYPEWRAP' and (lex[tmpi-1].type=='NEWLINE' or (lex[tmpi-1].type in typeNewline and lex[tmpi-1].value.count(' ')<tmpindent))])>0:
                                             linkType=False # if there is a typewrap defining the types, then we shouldnt mess with it
 
 
                                         if debug and search:
                                             print('constant-propagation:',lex[token].value)
@@ -1890,15 +1928,15 @@
                                                 if lex[tmpi].type in typeNewline: inFrom=inCase=False
                                                 elif inCase and lex[tmpi].type == 'IF': inCase=False # its fine on a conditional guard
                                             elif not search and not linkType: break # if linktype and search are false, why are we here? leave
                                             else:
                                                 if search and ignores!=[]:
                                                     if isinstance(ignores[0], int) and ignores[0] == tmpi:
                                                         search=False
-                                                    elif isinstance(ignores[0], list) and tmpi == ignores[0][0]:
+                                                    elif (isinstance(ignores[0], list) or isinstance(ignores[0], tuple)) and tmpi == ignores[0][0]:
                                                         ignore=True
                                                     if ignore and tmpi == ignores[0][1]:
                                                         ignore=False ; del ignores[0]
                                                     #if debug: print(tmpi,lex[tmpi].type,f'ignore={ignore}',f'skip/end={ignores}')
 
                                                 if search and ignore == False:
                                                     #print(lex[token].value,lex[tmpi].type,lex[tmpi].value,search,linkType,ignores,tmpi, tmpLastIndent,tmpindent)
@@ -2006,15 +2044,20 @@
                                                                                 if   t.value[-1] == lex[tmpFSTRcheck].value[1]: t.value = t.value[:-1]+tmpFSTRq
                                                                                 elif t.value[ 1] == lex[tmpFSTRcheck].value[1]: t.value = 'f'+tmpFSTRq+t.value[2:]
                                                                 
                                                                 if len(tmpf)>=2 and tmpf[1].type == 'FSTR' and lex[tmpi+1].type == 'FSTR':
                                                                     # a ID and FSTR with nothing inbetween implies comparison,
                                                                     # whereas FSTR + FSTR implies addition
                                                                     # so we insert comparison to not break behaviour
-                                                                    lex.insert(tmpi+1,makeToken(lex[token],'==','EQUAL'))
+                                                                    tmpInFString = False
+                                                                    for t in range(tmpi,0,-1): # check to make sure we are not in fstring first
+                                                                        if lex[t].type == 'FSTR' and lex[t].value.endswith('{'):
+                                                                            tmpInFString = True ; break
+                                                                        elif lex[t].type in {'TAB','NEWLINE'}: break
+                                                                    if not tmpInFString: lex.insert(tmpi+1,makeToken(lex[token],'==','EQUAL'))
                                                                 if lex[tmpi+1].type == 'PIPE' and tmpf[0].type == 'RPAREN' and tmpf[-1].type == 'LPAREN':
                                                                     # when folding tuple onto pipe, add another paren as to not inherit the tuple.
                                                                     tmpf.append(makeToken(tmpf[0], '(', 'LPAREN'))
                                                                     tmpf.insert(0, makeToken(tmpf[0], ')', 'RPAREN'))
                                                                 lex[tmpi].type='IGNORE'
                                                                 for t in tmpf:
                                                                     lex.insert(tmpi,copy(t))
@@ -3082,14 +3125,15 @@
                                         lex.insert(tmpi+1,makeToken(tok,'(','LPAREN'))
                                 del importcheck ; del assignCheck
 
 
                                 if len(tmpf) > 0:
                                     lexAdd=0
                                     tmp=[]
+                                    tmpInsertHere = token # all prealloc in the same spot
                                     for t in tmpf:
                                         tmpval=t[0].split('.')
                                         check=False
                                         if tmpval[-1] in listMods or '.'+tmpval[-1] in listMods:
                                             for ii in range(token-1,0,-1):
                                                 if lex[ii].type == 'ID' and lex[ii].value == tmpval[0]:
                                                     check=True ; break
@@ -3097,42 +3141,68 @@
                                         else: check=True
                                         if check == False : break
 
                                         if '.' in t[0]: tmpname=t[0].split('.')[0]+'_'+t[0].split('.')[1]
                                         else: tmpname=t[0]
                                         subBy=1
                                         tmpASname = f'AS{tmpname}'
+                                        if t[0] in pyBuiltinFunctions:
+                                            # check backward for better assign point, incase already used.
+                                            # sometimes can make use of the function before the loop
+                                            tmptmpIndent=tmpCurrentIndent=None ; tmpFound=False
+                                            tmpChangeTheseIfFound=[]
+                                            for ii in range(token - 1, 0, -1):
+                                                #print(tmpASname,lex[ii].type,lex[ii].value,tmpFound,tmpCurrentIndent,tmptmpIndent)
+                                                if lex[ii].type == 'TAB':
+                                                    if tmptmpIndent == None: tmptmpIndent=lex[ii].value.count(' ')
+                                                    tmpCurrentIndent = lex[ii].value.count(' ')
+                                                    if tmpCurrentIndent < tmptmpIndent: break
+                                                    if tmpCurrentIndent > tmptmpIndent and tmpFound: tmpFound=False ; break
+                                                    if tmpFound and lex[ii+1].type not in {'ELIF','OF','ELSE'}: tmpInsertHere = ii + 1; break
+                                                elif lex[ii].type == 'NEWLINE':
+                                                    if tmptmpIndent == None: tmptmpIndent = 0
+                                                    tmpCurrentIndent = 0
+                                                    if tmpCurrentIndent < tmptmpIndent: break
+                                                    if tmpCurrentIndent > tmptmpIndent and tmpFound: tmpFound = False; break
+                                                    if tmpFound and lex[ii+1].type not in {'ELIF','OF','ELSE'}: tmpInsertHere = ii + 1; break
+                                                elif lex[ii].type == 'FUNCTION' and lex[ii].value == t[0]+'(' and tmpCurrentIndent == tmptmpIndent:
+                                                    tmpFound=True ; tmpChangeTheseIfFound.append(ii)
+                                            if tmpFound:
+                                                for f in tmpChangeTheseIfFound: lex[f].value = tmpASname+'('
+
+
                                         if tmpASname not in tmp and (tmpindent,tmpASname) not in preAllocated \
                                         and (not preAllocated or all(True if pa[1] != tmpASname or pa[0] > tmpindent else False for pa in preAllocated) ):
+                                            #print(tmpASname,tmpInsertHere,lex[tmpInsertHere].value,lex[tmpInsertHere+1].value,)
                                             preAllocated.add((tmpindent,tmpASname))
-                                            if lex[token - 1].type == 'DEFFUNCT': subBy = 0
+                                            if lex[tmpInsertHere - 1].type == 'DEFFUNCT': subBy = 0
                                             #
-                                            tmptok=copy(lex[token])
+                                            tmptok=copy(lex[tmpInsertHere])
                                             tmptok.value=t[0]
                                             tmptok.type='BUILTINF'
-                                            lex.insert(token-subBy,tmptok)
+                                            lex.insert(tmpInsertHere-subBy,tmptok)
                                             #
-                                            tmptok=copy(lex[token])
+                                            tmptok=copy(lex[tmpInsertHere])
                                             tmptok.value='='
                                             tmptok.type='ASSIGN'
-                                            lex.insert(token-subBy,tmptok)
+                                            lex.insert(tmpInsertHere-subBy,tmptok)
                                             #
-                                            tmptok=copy(lex[token])
+                                            tmptok=copy(lex[tmpInsertHere])
                                             tmptok.value=tmpASname
                                             tmptok.type='ID'
-                                            lex.insert(token-subBy,tmptok)
+                                            lex.insert(tmpInsertHere-subBy,tmptok)
                                             #
                                             if subBy > 0: # not in def
-                                                tmptok=copy(lex[token])
+                                                tmptok=copy(lex[tmpInsertHere])
                                                 tmptok.value=f'\n{" "*tmpindent}' if tmpindent > 0 else '\n'
                                                 tmptok.type='TAB' if tmpindent > 0 else 'NEWLINE'
                                                 tmptok.lineno=0 # to not mess up lineNumber for errors
-                                                lex.insert(token-subBy,tmptok)
+                                                lex.insert(tmpInsertHere-subBy,tmptok)
                                             else: # in def
-                                                lex.insert(token+3,makeToken(tok,'then','THEN'))
+                                                lex.insert(tmpInsertHere+3,makeToken(tok,'then','THEN'))
                                             #
                                             lexIndex+=4
                                             lexAdd+=4
                                             tmp.append(tmpASname)
                                             if debug: print(f'! attrs: {t[0]} --> {tmp[-1]}')
                                             newOptimization = True
                                         lex[t[1]+lexAdd].value=tmpASname
@@ -3740,15 +3810,15 @@
                                     if lex[token].value[c] in ('"',"'"):
                                         quotes=lex[token].value[c] ; break
                                 for c in range(len(lex[token+2].value)):
                                     if lex[token+2].value[c] in ('"',"'"):
                                         lex[token].value=lex[token].value[:-1]+lex[token+2].value[c+1:]
                                         lex[token].value=lex[token].value[:-1]+quotes
                                         break
-                                if debug: print(f'! merging into {lex[token].value}')
+                                if debug: print(f'! string merging into {lex[token].value}')
                                 newOptimization=True
                                 lex[token+1].type=lex[token+2].type='IGNORE'
                             if lex[token+1].type == 'TIMES' and ((lex[token].type == 'STRING' and lex[token+2].type == 'NUMBER') or (lex[token].type == 'NUMBER' and lex[token+2].type == 'STRING')):
                                 tmpSafe = True
                                 if lex[token].type == 'STRING':
                                       tmpS = token   ; tmpN = token+2
                                 else: tmpS = token+2 ; tmpN = token
@@ -3852,130 +3922,160 @@
                                         lex.insert(token+1, makeToken(tok, ';', 'THEN'))
                                 lex[token].value='from %s import %s'%(importedName[:-1], ', '.join([tmpImportThese[i] for i in range(0,len(tmpImportThese))]))
                             else: lex[token].value=f'from {importedName} import *'
                             del wasImported[importedName]
                     
                 elif optDeadVariableElimination and lex[token].type == 'ID' and lex[token].value != 'print':
                     if ((lex[token + 1].type in typeAssignables and lex[token+1].type!='LIST') or (lex[token + 1].type=='ASSIGN' and lex[token + 1].value in ('=','is','is '))) and lex[token - 1].type in typeNewline + ('CONSTANT', 'TYPE'):
-                        delPoint = tmpIndent = None ; check = True ; tmpReplaceWithPass = inCase = isConstant = outOfBlock= False
+                        delPoint = tmpIndent = None ; check = True ; tmpReplaceWithPass = inCase = isConstant = outOfBlock = False
                         tmpCurrentIndent = 0 ; tmpParenScope=0
                         # tmpIndent is var's indent, tmpCurrentIndent is iterations indent
                         # outOfBlock signifies that if we are in a function or class, we are safe from previous classes
                         tmpSkipCheck = lex[token] in varWasFolded # bypasses checking if the var is dead, assumes it is dead
+                        tmpInsideFunction = False # determine if inside a function. outOfBlock seems to be pretty much the same thing.
+                        tmpLowestIndent=(None,0) # track lowest indent 1st: in func 2nd: lowest indent
                         for tmpi in range(token-1, -1, -1):
-                            #print(lex[token].value, '-!', lex[tmpi].value, lex[tmpi].type, tmpIndent,check)
+                            #print(lex[token].value, '-!', lex[tmpi].value, lex[tmpi].type, tmpIndent,check,tmpInsideFunction)
                             if tmpSkipCheck and delPoint != None: check=True ; break
                             if lex[tmpi].type == 'TAB':
                                 if tmpIndent==None: tmpIndent = lex[tmpi].value.replace('\t', ' ').count(' ')
                                 if delPoint==None: delPoint=tmpi
                                 tmpCurrentIndent = lex[tmpi].value.replace('\t', ' ').count(' ')
                                 inCase=False
+                                if tmpCurrentIndent < tmpLowestIndent[1]: tmpLowestIndent = (tmpLowestIndent[0], tmpCurrentIndent)
                             elif lex[tmpi].type == 'NEWLINE':
                                 if tmpIndent==None:
                                     if isConstant: check = False ; break # constants on global scope should not be eliminated
                                     tmpIndent = 0
-                                if delPoint==None: delPoint=tmpi
+                                if delPoint==None: delPoint = tmpi
                                 tmpCurrentIndent = 0
                                 inCase=False
+                                if tmpLowestIndent[0] in {True,False}: tmpLowestIndent = (tmpLowestIndent[0], 0)
+                                else: tmpLowestIndent = (False, 0)
                             elif lex[tmpi].type == 'THEN':
                                 if delPoint==None: delPoint=tmpi
                                 inCase=False
                             elif lex[tmpi].type == 'SCOPE' and lex[token].value in lex[tmpi].value :
                                 check=False ; break
                             elif lex[tmpi].type == 'FROM' and not delPoint: break
                             elif not inCase and lex[tmpi].type in {'ID', 'INC', 'BUILTINF','FUNCTION'} and (lex[tmpi].value.replace('(','').replace('+','').replace('-', '') == lex[token].value or lex[token].value+'.' in lex[tmpi].value):
                                 check = False ; break
                             elif lex[tmpi].type in {'PYDEF','DEFFUNCT'} and not outOfBlock and tmpIndent:
                                 if lex[tmpi].type == 'PYDEF':
-                                    if lex[tmpi-1].type == 'NEWLINE':
-                                        outOfBlock=True
+                                    if lex[tmpi-1].type == 'NEWLINE' or (lex[tmpi-1].type in {'ASYNC','FUNCMOD'} and lex[tmpi-2].type == 'NEWLINE') or (lex[tmpi-1].type == 'ASYNC' and lex[tmpi-2].type == 'FUNCMOD' and lex[tmpi-3].type == 'NEWLINE'):
+                                        tmpInsideFunction = outOfBlock = True
                                     elif lex[tmpi-1].type == 'TAB' and lex[tmpi-1].value.count(' ') < tmpIndent:
-                                        outOfBlock = True
+                                        tmpInsideFunction = outOfBlock = True
+                                if tmpLowestIndent[0] == None:
+                                    tmpFuncNLPlacement=1 if lex[tmpi].type == 'PYDEF' else 2
+                                    if   lex[tmpi - tmpFuncNLPlacement].type == 'NEWLINE' and tmpLowestIndent[1] > 0:
+                                        tmpInsideFunction = True
+                                    elif lex[tmpi - tmpFuncNLPlacement].type == 'TAB' and lex[tmpi - 1].value.count(' ') < tmpLowestIndent[1]:
+                                        tmpInsideFunction = True
+                                    if tmpInsideFunction:
+                                        tmpLowestIndent = (True, tmpLowestIndent[1])
                             elif (lex[tmpi].type in typeConditionals or (lex[tmpi].type == 'TRY' and 'try' in lex[tmpi].value)) and delPoint:
                                 # prevents dead variables defined in conditionals from breaking syntax
                                 tmpReplaceWithPass = True
                                 if lex[tmpi].type == 'IF':
                                     inCase = False
                             elif lex[tmpi].type == 'PYCLASS' and delPoint and tmpIndent:
                                 if not outOfBlock and ((lex[tmpi-1].type == 'NEWLINE' and tmpIndent > 0) \
                                 or (lex[tmpi-1].type == 'TAB' and lex[tmpi-1].value.count(' ') < tmpIndent)):
                                     check=False ; break
-
-                            elif lex[tmpi].type == 'TYPEWRAP':
+                            elif lex[tmpi].type == 'TYPEWRAP' and not outOfBlock:
                                 if lex[tmpi-1].type == 'TAB':
                                     tmpIndent = lex[tmpi-1].value.replace('\t', ' ').count(' ')
                                 elif lex[tmpi-1].type == 'NEWLINE': tmpIndent=0
                                 else: tmpIndent=None
                             elif lex[tmpi].type == 'OF' and 'case' in lex[tmpi].value:
                                 inCase=True
                             elif lex[tmpi].type == 'LPAREN': tmpParenScope+=1
                             elif lex[tmpi].type == 'FUNCTION' and '(' in lex[tmpi].value: tmpParenScope+=1
                             elif lex[tmpi].type == 'RPAREN': tmpParenScope-=1
                             elif lex[tmpi].type == 'CONSTANT' and not delPoint: isConstant = True
                         if tmpParenScope > 0: check=False
                         if delPoint == None or tmpIndent == None: check=False
                         if (token-1<=0): check=True ; delPoint = tmpIndent = 0
                         if check:
-                            breakOnNextNL=ttenary=inCase=tmpCallsFunction=tmpOutOfAssign=tmpInConditional=tmpOutOfStartingBlock=False
-                            tmpCurrentIndent=tmpIndent # tmpIndent is indent of OG var, tmpCurrentIndent is current
+                            breakOnNextNL = ttenary = inCase = tmpCallsFunction = tmpOutOfAssign = tmpInConditional = tmpOutOfStartingBlock = tmpInOtherFunction = False
+                            tmpCurrentIndent = tmpIndent  # tmpIndent is indent of OG var, tmpCurrentIndent is current
                             for tmpi in range(token + 1, len(lex) - 1):
-                                #print(lex[token].value,'+!',lex[tmpi].value,lex[tmpi].type,ttenary,tmpIndent,check,tmpCallsFunction,tmpCurrentIndent,tmpIndent)
-                                if not inCase and lex[tmpi].type in {'ID', 'INC', 'BUILTINF','FUNCTION'} and (lex[tmpi].value.replace('(','').replace('+','').replace('-', '') == lex[token].value or lex[token].value+'.' in lex[tmpi].value):
-                                    if lex[tmpi+1].type != 'ASSIGN' or (lex[tmpi+1].value.strip() not in {'=','is'} or determineIfAssignOrEqual(tmpi+1)):
-                                        check=False ; break
-                                    elif pyIs and lex[tmpi+1].type == 'ASSIGN' and '=' not in lex[tmpi+1].value:
-                                        check = False ; break
-                                    elif not tmpOutOfStartingBlock and tmpCurrentIndent == tmpIndent and not tmpCallsFunction: breakOnNextNL=True
+                                #print(lex[token].value,'+!',lex[tmpi].value,lex[tmpi].type,ttenary,tmpCallsFunction,tmpCurrentIndent,tmpIndent)
+                                if not inCase and lex[tmpi].type in {'ID', 'INC', 'BUILTINF', 'FUNCTION'} and (lex[tmpi].value.replace('(', '').replace('+', '').replace('-', '') == lex[token].value or lex[token].value + '.' in lex[tmpi].value) and (not tmpInOtherFunction or not tmpInsideFunction):
+                                    if lex[tmpi + 1].type != 'ASSIGN' or (lex[tmpi + 1].value.strip() not in {'=', 'is'} or determineIfAssignOrEqual(tmpi + 1)):
+                                        check = False
+                                    elif pyIs and lex[tmpi + 1].type == 'ASSIGN' and '=' not in lex[tmpi + 1].value:
+                                        check = False
+                                    elif not tmpOutOfStartingBlock and tmpCurrentIndent == tmpIndent and not tmpCallsFunction:
+                                        breakOnNextNL = True
                                 elif not inCase and lex[tmpi].type == 'NRANGE':
-                                    tmp=False
+                                    tmp = False
                                     if '...' in lex[tmpi].value:
-                                        tmp=lex[tmpi].value.split('...')
+                                        tmp = lex[tmpi].value.split('...')
                                     elif '..' in lex[tmpi].value:
-                                        tmp=lex[tmpi].value.split('..')
+                                        tmp = lex[tmpi].value.split('..')
                                     elif 'to' in lex[tmpi].value:
-                                        tmp=lex[tmpi].value.split('to',1)
+                                        tmp = lex[tmpi].value.split('to', 1)
                                     if tmp:
-                                        tmp=[i.strip() for i in tmp]
+                                        tmp = [i.strip() for i in tmp]
                                         if lex[token].value in tmp:
-                                            check=False ; break
-                                elif lex[tmpi].type == 'INDEX' and lex[tmpi].value.startswith(lex[token].value):
-                                    check=False ; break
-                                elif lex[tmpi].type == 'LISTCOMP' and lex[tmpi].value.split(':')[0] == lex[token].value: check=False ; break
+                                            check = False
+                                elif lex[tmpi].type == 'INDEX' and (lex[tmpi].value.startswith(lex[token].value) or REsearch(fr'.+\[.*{lex[token].value}.*\]', lex[tmpi].value)):
+                                    check = False
+                                elif lex[tmpi].type == 'LISTCOMP' and lex[tmpi].value.split(':')[0] == lex[token].value:
+                                    check = False
                                 elif lex[tmpi].type == 'FROM':
                                     for tmpii in range(tmpi, 0, -1):
                                         if lex[tmpii].type == 'TAB':
-                                            tmp = lex[tmpii].value.replace('\t', ' ').count(' ');break
+                                            tmp = lex[tmpii].value.replace('\t', ' ').count(' ')
+                                            break
                                         elif lex[tmpii].type == 'NEWLINE':
-                                            tmp = 0;break
+                                            tmp = 0 ; break
                                     if tmp < tmpIndent:
-                                        breakOnNextNL=True
-                                elif lex[tmpi].type == 'ASSIGN' and ':' not in lex[tmpi].value and lex[tmpi+1].type == 'IF':
-                                    ttenary=True
-                                elif lex[tmpi].type == 'ELSE' and ttenary: ttenary=False
-                                elif breakOnNextNL and not ttenary and lex[tmpi].type in typeNewline: break
+                                        breakOnNextNL = True
+                                elif lex[tmpi].type == 'ASSIGN' and ':' not in lex[tmpi].value and lex[
+                                    tmpi + 1].type == 'IF':
+                                    ttenary = True
+                                elif lex[tmpi].type == 'ELSE' and ttenary:
+                                    ttenary = False
+                                elif breakOnNextNL and not ttenary and lex[tmpi].type in typeNewline:
+                                    break
                                 elif lex[tmpi].type == 'INDEX' and f" {lex[token].value} " in lex[tmpi].value:
-                                    check = False ; break
+                                    check = False
                                 elif lex[tmpi].type == 'OF' and 'case' in lex[tmpi].value:
                                     inCase = True
                                 elif lex[tmpi].type == 'IF':
-                                    inCase = False ; tmpInConditional=True
-                                elif lex[tmpi].type in {'ELIF','OF'}: tmpInConditional=True
+                                    inCase = False;
+                                    tmpInConditional = True
+                                elif lex[tmpi].type in {'ELIF', 'OF'}:
+                                    tmpInConditional = True
                                 elif lex[tmpi].type == 'PYDEF' and REfindall(f'=.*?{lex[token].value}',lex[tmpi].value):
                                     # if var is in function default argument like:
                                     # def thing(arg=var)
-                                    check = False ; break
+                                    check = False;
                                 elif lex[tmpi].type in typeNewline:
-                                    if not ttenary: tmpOutOfAssign=True
-                                    if lex[tmpi].type == 'NEWLINE': tmpCurrentIndent = 0
-                                    elif lex[tmpi].type == 'TAB': tmpCurrentIndent = lex[tmpi].value.count(' ')
-                                    elif lex[tmpi].type == 'THEN' and tmpInConditional: tmpCurrentIndent+=prettyIndent
-                                    if tmpCurrentIndent < tmpIndent: tmpOutOfStartingBlock=True
-                                    tmpInConditional=False
+                                    if not ttenary: tmpOutOfAssign = True
+                                    if lex[tmpi].type == 'NEWLINE':
+                                        tmpCurrentIndent = 0
+                                    elif lex[tmpi].type == 'TAB':
+                                        tmpCurrentIndent = lex[tmpi].value.count(' ')
+                                    elif lex[tmpi].type == 'THEN' and tmpInConditional:
+                                        tmpCurrentIndent += prettyIndent
+                                    if tmpCurrentIndent < tmpIndent:
+                                        tmpOutOfStartingBlock = True
+                                        if tmpi + 2 < len(lex) and (lex[tmpi + 1].type == 'PYDEF' or lex[tmpi + 2].type == 'DEFFUNCT'):
+                                            tmpInOtherFunction = True
+                                    tmpInConditional = False
                                 elif not tmpSkipCheck and not tmpOutOfAssign and lex[tmpi].type == 'FUNCTION':
-                                    tmpCallsFunction=True
+                                    tmpCallsFunction = True
+                                if not check: break
+
+                                #tmpDEBUG = 'pretemp'
+                                #if debug and lex[token].value == tmpDEBUG and lex[tmpi].type == 'ID' and lex[tmpi].value == tmpDEBUG: print(inCase,tmpInOtherFunction,tmpInsideFunction);exit()
                             if tmpSkipCheck:
                                 varWasFolded.remove(lex[token])
 
                         if check:  # remove the var
                             #print('-------', lex[token].value)
                             ttenary = tmpPass = False ; tmpEnd = tmpParenScope = tmpListScope = 0
                             for tmpi in range(delPoint+1, len(lex)*2):
@@ -4558,16 +4658,14 @@
 
                                 if not assign and i.type in {'ID','TYPE'} and (tmpLastToken.type not in {'COMMA','TMP','TYPE'} and tmpLastToken.value not in convertType):
                                     tmp=' '.join([ii.value for ii in tmpf])
                                     return AS_SyntaxError(f'{tmp}\n\tfrom syntax must have commas to seperate arguments','from thingy, str name, int number = 12,', lineNumber, data)
 
                                 elif i.value in convertType:
                                     tmptype=i
-                                    if compileTo=='Cython' and tmptype.value=='bool' and noKwargs:
-                                        insertAtTopOfCodeIfItIsNotThere(f'cdef extern from "stdbool.h":\n{" "*prettyIndent}ctypedef bint bool')
                                 elif i.type == 'ASSIGN': assign=True
                                 elif i.type in {'TIMES','EXPONENT','MINUS'}: kwargs=i.type ; continue
                                 elif assign:
                                     newtmp[-1]+=f' = {i.value}'
                                     assign=False
                                 elif tmptype!=None:
                                     storeVar(i,None,lex[0],tmptype)
@@ -5972,18 +6070,16 @@
                 else:
                     multiType=False
                     if '[' in tok.value:
                         firstType=tok.value.split('[')[0]
                         secondType=tok.value.split('[')[1].replace(']','')
                         multiType=True
                         if secondType=='bool' and compileTo=='Cython':
-                            tok.value='bool'
+                            tok.value='bint'
 
-                    if compileTo=='Cython' and tok.value=='bool':
-                        insertAtTopOfCodeIfItIsNotThere(f'cdef extern from "stdbool.h":\n{" "*prettyIndent}ctypedef bint bool')
                     if lexIndex+2 < len(lex):
                         if lex[lexIndex+2].type == 'DEFFUNCT':
                             return AS_SyntaxError('type assigned to the wrong spot',f'myFunction does {tok.value}',lineNumber,data)
                         elif lex[lexIndex+2].type == 'ASSIGN' and any(i for i in ('+','-','*','/') if lex[lexIndex+2].value.startswith(i)):
                             return AS_SyntaxError('When declaring types, you can\'t modify the variable, as it does not have a value yet.',f'{tok.value} {lex[lexIndex+1].value} = something',lineNumber,data)
                     if lastType == 'DEFFUNCT' and pythonVersion > 3.04:
                         if multiType:
@@ -6017,16 +6113,18 @@
                             if compileTo == 'Cython' and inLoop[0]==False and lex[lexIndex+1].value not in storedVarsHistory:
                                 if lex[lexIndex + 2].type == 'COMMA':
                                     tmp = []
                                     for tmpi in range(lexIndex + 1, len(lex) - 1):
                                         if lex[tmpi].type == 'ID': tmp.append(lex[tmpi].value)
                                         elif lex[tmpi].type == 'COMMA': pass
                                         else: break
-                                    for varname in tmp: code.append(f"{' ' * (indent)}cdef {tok.value} {varname}")
-                                else: line.append(decideIfIndentLine(indent,f"cdef {tok.value} "))
+                                    for varname in tmp: code.append(f"{' ' * (indent)}cdef {cythonConvertType[tok.value] if tok.value in cythonConvertType else tok.value} {varname}")
+                                else:
+                                    tok.value = cythonConvertType[tok.value] if tok.value in cythonConvertType else tok.value
+                                    line.append(decideIfIndentLine(indent,f"cdef {tok.value} "))
                             else:# compileTo == 'Python':
                                 if pythonVersion >= 3.06:
                                     if lex[lexIndex+2].type == 'COMMA':
                                         tmp=[]
                                         for tmpi in range(lexIndex+1,len(lex)-1):
                                             if lex[tmpi].type == 'ID': tmp.append(lex[tmpi].value)
                                             elif lex[tmpi].type == 'COMMA': pass
@@ -6073,14 +6171,15 @@
                                         for t in values:
                                             if ':' in t.value: t.value=t.value.split(':')[0]
                                             lex.insert(tmp-1,t)
 
                     elif lex[lexIndex+1].type == 'COMMAGRP' and '=' in lex[lexIndex+1].value and lastType in typeNewline+('CONST',):
                         tmpf = lex[lexIndex + 1].value.split('=')[0].split(',') ; tmpf=[t.replace(' ','') for t in tmpf]
                         if compileTo == 'Cython' and any(True for t in tmpf if t in storedVarsHistory)==False and inLoop[0]==False and lastIndent[2] == []:
+                            tok.value = cythonConvertType[tok.value] if tok.value in cythonConvertType else tok.value
                             line.append(decideIfIndentLine(indent, f"cdef {tok.value} {lex[lexIndex + 1].value.split('=')[0]}\n"))
                         else:
                             line.append(decideIfIndentLine(indent, ' '.join([f"{t}: {tok.value} ;" for t in tmpf])+'\n'  ))
                         startOfLine=True
                     else:
                         if startOfLine: line.append(f'{" "*indent}{tok.value}')
                         else: line.append(tok.value)
```

### Comparing `ASnake-0.13.37/src/ASnake/__main__.py` & `asnake-0.13.38/src/ASnake/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from .ASnake import build, ASnakeVersion, latestPythonVersionSupported
+try:
+    from .ASnake import build, ASnakeVersion, latestPythonVersionSupported
+except ImportError:
+    from ASnake import build, ASnakeVersion, latestPythonVersionSupported
 
 # dependencies
 from autopep8 import fix_code
 
 # standard library
 from subprocess import check_output, CalledProcessError, STDOUT
 from os import path, remove, listdir
```

### Comparing `ASnake-0.13.37/src/ASnake/data/megaTest.asnake` & `asnake-0.13.38/src/ASnake/data/megaTest.asnake`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.37/src/ASnake/data/setAlias.asnake` & `asnake-0.13.38/src/ASnake/data/setAlias.asnake`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.37/src/ASnake.egg-info/PKG-INFO` & `asnake-0.13.38/src/ASnake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASnake
-Version: 0.13.37
+Version: 0.13.38
 Summary: Python optimizing compiler for the ASnake programming language.
 Author: Ahri Fox
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

