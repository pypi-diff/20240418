# Comparing `tmp/winpcapy-1.0.2.tar.gz` & `tmp/winpcapy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\winpcapy-1.0.2.tar", last modified: Wed Jan 25 21:12:58 2017, max compression
+gzip compressed data, was "winpcapy-1.0.3.tar", last modified: Thu Apr 18 12:53:19 2024, max compression
```

## Comparing `winpcapy-1.0.2.tar` & `winpcapy-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2017-01-25 21:12:58.000000 winpcapy-1.0.2/
--rw-rw-rw-   0        0        0    15436 2016-12-29 19:38:43.000000 winpcapy-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       21 2016-12-30 17:21:05.000000 winpcapy-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5303 2017-01-25 21:12:58.000000 winpcapy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3302 2017-01-25 21:10:58.000000 winpcapy-1.0.2/README.rst
--rw-rw-rw-   0        0        0      134 2017-01-25 21:12:58.000000 winpcapy-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2551 2016-12-30 17:26:43.000000 winpcapy-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2017-01-25 21:12:58.000000 winpcapy-1.0.2/winpcapy/
--rw-rw-rw-   0        0        0     8218 2017-01-25 21:10:58.000000 winpcapy-1.0.2/winpcapy/winpcapy.py
--rw-rw-rw-   0        0        0    27326 2016-12-29 19:22:48.000000 winpcapy-1.0.2/winpcapy/winpcapy_types.py
--rw-rw-rw-   0        0        0      663 2017-01-25 21:10:58.000000 winpcapy-1.0.2/winpcapy/__init__.py
-drwxrwxrwx   0        0        0        0 2017-01-25 21:12:58.000000 winpcapy-1.0.2/winpcapy.egg-info/
--rw-rw-rw-   0        0        0        1 2017-01-25 21:12:58.000000 winpcapy-1.0.2/winpcapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5303 2017-01-25 21:12:58.000000 winpcapy-1.0.2/winpcapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2017-01-25 21:12:58.000000 winpcapy-1.0.2/winpcapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2017-01-25 21:12:58.000000 winpcapy-1.0.2/winpcapy.egg-info/top_level.txt
+drwxr-xr-x   0 orweis     (501) staff       (20)        0 2024-04-18 12:53:19.073983 winpcapy-1.0.3/
+-rw-r--r--   0 orweis     (501) staff       (20)    15173 2024-04-18 12:41:17.000000 winpcapy-1.0.3/LICENSE
+-rw-r--r--   0 orweis     (501) staff       (20)       21 2024-04-18 12:41:17.000000 winpcapy-1.0.3/MANIFEST.in
+-rw-r--r--   0 orweis     (501) staff       (20)     4382 2024-04-18 12:53:19.073913 winpcapy-1.0.3/PKG-INFO
+-rw-r--r--   0 orweis     (501) staff       (20)     3208 2024-04-18 12:41:17.000000 winpcapy-1.0.3/README.rst
+-rw-r--r--   0 orweis     (501) staff       (20)      102 2024-04-18 12:53:19.074196 winpcapy-1.0.3/setup.cfg
+-rw-r--r--   0 orweis     (501) staff       (20)     2469 2024-04-18 12:52:35.000000 winpcapy-1.0.3/setup.py
+drwxr-xr-x   0 orweis     (501) staff       (20)        0 2024-04-18 12:53:19.072561 winpcapy-1.0.3/winpcapy/
+-rw-r--r--   0 orweis     (501) staff       (20)      639 2024-04-18 12:52:10.000000 winpcapy-1.0.3/winpcapy/__init__.py
+-rw-r--r--   0 orweis     (501) staff       (20)    10701 2024-04-18 12:41:17.000000 winpcapy-1.0.3/winpcapy/winpcapy.py
+-rw-r--r--   0 orweis     (501) staff       (20)    26668 2024-04-18 12:41:17.000000 winpcapy-1.0.3/winpcapy/winpcapy_types.py
+drwxr-xr-x   0 orweis     (501) staff       (20)        0 2024-04-18 12:53:19.073638 winpcapy-1.0.3/winpcapy.egg-info/
+-rw-r--r--   0 orweis     (501) staff       (20)     4382 2024-04-18 12:53:19.000000 winpcapy-1.0.3/winpcapy.egg-info/PKG-INFO
+-rw-r--r--   0 orweis     (501) staff       (20)      246 2024-04-18 12:53:19.000000 winpcapy-1.0.3/winpcapy.egg-info/SOURCES.txt
+-rw-r--r--   0 orweis     (501) staff       (20)        1 2024-04-18 12:53:19.000000 winpcapy-1.0.3/winpcapy.egg-info/dependency_links.txt
+-rw-r--r--   0 orweis     (501) staff       (20)        9 2024-04-18 12:53:19.000000 winpcapy-1.0.3/winpcapy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `winpcapy-1.0.2/LICENSE` & `winpcapy-1.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-The GNU General Public License, Version 2, June 1991 (GPLv2)
-============================================================
-
-> Copyright (C) 1989, 1991 Free Software Foundation, Inc.
-> 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA
-
-Everyone is permitted to copy and distribute verbatim copies of this license
-document, but changing it is not allowed.
-
-
-Preamble
---------
-
-The licenses for most software are designed to take away your freedom to share
-and change it. By contrast, the GNU General Public License is intended to
-guarantee your freedom to share and change free software--to make sure the
-software is free for all its users. This General Public License applies to most
-of the Free Software Foundation's software and to any other program whose
-authors commit to using it. (Some other Free Software Foundation software is
-covered by the GNU Lesser General Public License instead.) You can apply it to
-your programs, too.
-
-When we speak of free software, we are referring to freedom, not price. Our
-General Public Licenses are designed to make sure that you have the freedom to
-distribute copies of free software (and charge for this service if you wish),
-that you receive source code or can get it if you want it, that you can change
-the software or use pieces of it in new free programs; and that you know you can
-do these things.
-
-To protect your rights, we need to make restrictions that forbid anyone to deny
-you these rights or to ask you to surrender the rights. These restrictions
-translate to certain responsibilities for you if you distribute copies of the
-software, or if you modify it.
-
-For example, if you distribute copies of such a program, whether gratis or for a
-fee, you must give the recipients all the rights that you have. You must make
-sure that they, too, receive or can get the source code. And you must show them
-these terms so they know their rights.
-
-We protect your rights with two steps: (1) copyright the software, and (2) offer
-you this license which gives you legal permission to copy, distribute and/or
-modify the software.
-
-Also, for each author's protection and ours, we want to make certain that
-everyone understands that there is no warranty for this free software. If the
-software is modified by someone else and passed on, we want its recipients to
-know that what they have is not the original, so that any problems introduced by
-others will not reflect on the original authors' reputations.
-
-Finally, any free program is threatened constantly by software patents. We wish
-to avoid the danger that redistributors of a free program will individually
-obtain patent licenses, in effect making the program proprietary. To prevent
-this, we have made it clear that any patent must be licensed for everyone's free
-use or not licensed at all.
-
-The precise terms and conditions for copying, distribution and modification
-follow.
-
-
-Terms And Conditions For Copying, Distribution And Modification
----------------------------------------------------------------
-
-**0.** This License applies to any program or other work which contains a notice
-placed by the copyright holder saying it may be distributed under the terms of
-this General Public License. The "Program", below, refers to any such program or
-work, and a "work based on the Program" means either the Program or any
-derivative work under copyright law: that is to say, a work containing the
-Program or a portion of it, either verbatim or with modifications and/or
-translated into another language. (Hereinafter, translation is included without
-limitation in the term "modification".) Each licensee is addressed as "you".
-
-Activities other than copying, distribution and modification are not covered by
-this License; they are outside its scope. The act of running the Program is not
-restricted, and the output from the Program is covered only if its contents
-constitute a work based on the Program (independent of having been made by
-running the Program). Whether that is true depends on what the Program does.
-
-**1.** You may copy and distribute verbatim copies of the Program's source code
-as you receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice and
-disclaimer of warranty; keep intact all the notices that refer to this License
-and to the absence of any warranty; and give any other recipients of the Program
-a copy of this License along with the Program.
-
-You may charge a fee for the physical act of transferring a copy, and you may at
-your option offer warranty protection in exchange for a fee.
-
-**2.** You may modify your copy or copies of the Program or any portion of it,
-thus forming a work based on the Program, and copy and distribute such
-modifications or work under the terms of Section 1 above, provided that you also
-meet all of these conditions:
-
-*   **a)** You must cause the modified files to carry prominent notices stating
-    that you changed the files and the date of any change.
-
-*   **b)** You must cause any work that you distribute or publish, that in whole
-    or in part contains or is derived from the Program or any part thereof, to
-    be licensed as a whole at no charge to all third parties under the terms of
-    this License.
-
-*   **c)** If the modified program normally reads commands interactively when
-    run, you must cause it, when started running for such interactive use in the
-    most ordinary way, to print or display an announcement including an
-    appropriate copyright notice and a notice that there is no warranty (or
-    else, saying that you provide a warranty) and that users may redistribute
-    the program under these conditions, and telling the user how to view a copy
-    of this License. (Exception: if the Program itself is interactive but does
-    not normally print such an announcement, your work based on the Program is
-    not required to print an announcement.)
-
-These requirements apply to the modified work as a whole. If identifiable
-sections of that work are not derived from the Program, and can be reasonably
-considered independent and separate works in themselves, then this License, and
-its terms, do not apply to those sections when you distribute them as separate
-works. But when you distribute the same sections as part of a whole which is a
-work based on the Program, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the entire whole,
-and thus to each and every part regardless of who wrote it.
-
-Thus, it is not the intent of this section to claim rights or contest your
-rights to work written entirely by you; rather, the intent is to exercise the
-right to control the distribution of derivative or collective works based on the
-Program.
-
-In addition, mere aggregation of another work not based on the Program with the
-Program (or with a work based on the Program) on a volume of a storage or
-distribution medium does not bring the other work under the scope of this
-License.
-
-**3.** You may copy and distribute the Program (or a work based on it, under
-Section 2) in object code or executable form under the terms of Sections 1 and 2
-above provided that you also do one of the following:
-
-*   **a)** Accompany it with the complete corresponding machine-readable source
-    code, which must be distributed under the terms of Sections 1 and 2 above on
-    a medium customarily used for software interchange; or,
-
-*   **b)** Accompany it with a written offer, valid for at least three years, to
-    give any third party, for a charge no more than your cost of physically
-    performing source distribution, a complete machine-readable copy of the
-    corresponding source code, to be distributed under the terms of Sections 1
-    and 2 above on a medium customarily used for software interchange; or,
-
-*   **c)** Accompany it with the information you received as to the offer to
-    distribute corresponding source code. (This alternative is allowed only for
-    noncommercial distribution and only if you received the program in object
-    code or executable form with such an offer, in accord with Subsection b
-    above.)
-
-The source code for a work means the preferred form of the work for making
-modifications to it. For an executable work, complete source code means all the
-source code for all modules it contains, plus any associated interface
-definition files, plus the scripts used to control compilation and installation
-of the executable. However, as a special exception, the source code distributed
-need not include anything that is normally distributed (in either source or
-binary form) with the major components (compiler, kernel, and so on) of the
-operating system on which the executable runs, unless that component itself
-accompanies the executable.
-
-If distribution of executable or object code is made by offering access to copy
-from a designated place, then offering equivalent access to copy the source code
-from the same place counts as distribution of the source code, even though third
-parties are not compelled to copy the source along with the object code.
-
-**4.** You may not copy, modify, sublicense, or distribute the Program except as
-expressly provided under this License. Any attempt otherwise to copy, modify,
-sublicense or distribute the Program is void, and will automatically terminate
-your rights under this License. However, parties who have received copies, or
-rights, from you under this License will not have their licenses terminated so
-long as such parties remain in full compliance.
-
-**5.** You are not required to accept this License, since you have not signed
-it. However, nothing else grants you permission to modify or distribute the
-Program or its derivative works. These actions are prohibited by law if you do
-not accept this License. Therefore, by modifying or distributing the Program (or
-any work based on the Program), you indicate your acceptance of this License to
-do so, and all its terms and conditions for copying, distributing or modifying
-the Program or works based on it.
-
-**6.** Each time you redistribute the Program (or any work based on the
-Program), the recipient automatically receives a license from the original
-licensor to copy, distribute or modify the Program subject to these terms and
-conditions. You may not impose any further restrictions on the recipients'
-exercise of the rights granted herein. You are not responsible for enforcing
-compliance by third parties to this License.
-
-**7.** If, as a consequence of a court judgment or allegation of patent
-infringement or for any other reason (not limited to patent issues), conditions
-are imposed on you (whether by court order, agreement or otherwise) that
-contradict the conditions of this License, they do not excuse you from the
-conditions of this License. If you cannot distribute so as to satisfy
-simultaneously your obligations under this License and any other pertinent
-obligations, then as a consequence you may not distribute the Program at all.
-For example, if a patent license would not permit royalty-free redistribution of
-the Program by all those who receive copies directly or indirectly through you,
-then the only way you could satisfy both it and this License would be to refrain
-entirely from distribution of the Program.
-
-If any portion of this section is held invalid or unenforceable under any
-particular circumstance, the balance of the section is intended to apply and the
-section as a whole is intended to apply in other circumstances.
-
-It is not the purpose of this section to induce you to infringe any patents or
-other property right claims or to contest validity of any such claims; this
-section has the sole purpose of protecting the integrity of the free software
-distribution system, which is implemented by public license practices. Many
-people have made generous contributions to the wide range of software
-distributed through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing to
-distribute software through any other system and a licensee cannot impose that
-choice.
-
-This section is intended to make thoroughly clear what is believed to be a
-consequence of the rest of this License.
-
-**8.** If the distribution and/or use of the Program is restricted in certain
-countries either by patents or by copyrighted interfaces, the original copyright
-holder who places the Program under this License may add an explicit
-geographical distribution limitation excluding those countries, so that
-distribution is permitted only in or among countries not thus excluded. In such
-case, this License incorporates the limitation as if written in the body of this
-License.
-
-**9.** The Free Software Foundation may publish revised and/or new versions of
-the General Public License from time to time. Such new versions will be similar
-in spirit to the present version, but may differ in detail to address new
-problems or concerns.
-
-Each version is given a distinguishing version number. If the Program specifies
-a version number of this License which applies to it and "any later version",
-you have the option of following the terms and conditions either of that version
-or of any later version published by the Free Software Foundation. If the
-Program does not specify a version number of this License, you may choose any
-version ever published by the Free Software Foundation.
-
-**10.** If you wish to incorporate parts of the Program into other free programs
-whose distribution conditions are different, write to the author to ask for
-permission. For software which is copyrighted by the Free Software Foundation,
-write to the Free Software Foundation; we sometimes make exceptions for this.
-Our decision will be guided by the two goals of preserving the free status of
-all derivatives of our free software and of promoting the sharing and reuse of
-software generally.
-
-
-No Warranty
------------
-
-**11.** BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY FOR
-THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE
-STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM
-"AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING,
-BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
-PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-**12.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR REDISTRIBUTE
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR
-INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA
-BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
-FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER
+The GNU General Public License, Version 2, June 1991 (GPLv2)
+============================================================
+
+> Copyright (C) 1989, 1991 Free Software Foundation, Inc.
+> 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA
+
+Everyone is permitted to copy and distribute verbatim copies of this license
+document, but changing it is not allowed.
+
+
+Preamble
+--------
+
+The licenses for most software are designed to take away your freedom to share
+and change it. By contrast, the GNU General Public License is intended to
+guarantee your freedom to share and change free software--to make sure the
+software is free for all its users. This General Public License applies to most
+of the Free Software Foundation's software and to any other program whose
+authors commit to using it. (Some other Free Software Foundation software is
+covered by the GNU Lesser General Public License instead.) You can apply it to
+your programs, too.
+
+When we speak of free software, we are referring to freedom, not price. Our
+General Public Licenses are designed to make sure that you have the freedom to
+distribute copies of free software (and charge for this service if you wish),
+that you receive source code or can get it if you want it, that you can change
+the software or use pieces of it in new free programs; and that you know you can
+do these things.
+
+To protect your rights, we need to make restrictions that forbid anyone to deny
+you these rights or to ask you to surrender the rights. These restrictions
+translate to certain responsibilities for you if you distribute copies of the
+software, or if you modify it.
+
+For example, if you distribute copies of such a program, whether gratis or for a
+fee, you must give the recipients all the rights that you have. You must make
+sure that they, too, receive or can get the source code. And you must show them
+these terms so they know their rights.
+
+We protect your rights with two steps: (1) copyright the software, and (2) offer
+you this license which gives you legal permission to copy, distribute and/or
+modify the software.
+
+Also, for each author's protection and ours, we want to make certain that
+everyone understands that there is no warranty for this free software. If the
+software is modified by someone else and passed on, we want its recipients to
+know that what they have is not the original, so that any problems introduced by
+others will not reflect on the original authors' reputations.
+
+Finally, any free program is threatened constantly by software patents. We wish
+to avoid the danger that redistributors of a free program will individually
+obtain patent licenses, in effect making the program proprietary. To prevent
+this, we have made it clear that any patent must be licensed for everyone's free
+use or not licensed at all.
+
+The precise terms and conditions for copying, distribution and modification
+follow.
+
+
+Terms And Conditions For Copying, Distribution And Modification
+---------------------------------------------------------------
+
+**0.** This License applies to any program or other work which contains a notice
+placed by the copyright holder saying it may be distributed under the terms of
+this General Public License. The "Program", below, refers to any such program or
+work, and a "work based on the Program" means either the Program or any
+derivative work under copyright law: that is to say, a work containing the
+Program or a portion of it, either verbatim or with modifications and/or
+translated into another language. (Hereinafter, translation is included without
+limitation in the term "modification".) Each licensee is addressed as "you".
+
+Activities other than copying, distribution and modification are not covered by
+this License; they are outside its scope. The act of running the Program is not
+restricted, and the output from the Program is covered only if its contents
+constitute a work based on the Program (independent of having been made by
+running the Program). Whether that is true depends on what the Program does.
+
+**1.** You may copy and distribute verbatim copies of the Program's source code
+as you receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice and
+disclaimer of warranty; keep intact all the notices that refer to this License
+and to the absence of any warranty; and give any other recipients of the Program
+a copy of this License along with the Program.
+
+You may charge a fee for the physical act of transferring a copy, and you may at
+your option offer warranty protection in exchange for a fee.
+
+**2.** You may modify your copy or copies of the Program or any portion of it,
+thus forming a work based on the Program, and copy and distribute such
+modifications or work under the terms of Section 1 above, provided that you also
+meet all of these conditions:
+
+*   **a)** You must cause the modified files to carry prominent notices stating
+    that you changed the files and the date of any change.
+
+*   **b)** You must cause any work that you distribute or publish, that in whole
+    or in part contains or is derived from the Program or any part thereof, to
+    be licensed as a whole at no charge to all third parties under the terms of
+    this License.
+
+*   **c)** If the modified program normally reads commands interactively when
+    run, you must cause it, when started running for such interactive use in the
+    most ordinary way, to print or display an announcement including an
+    appropriate copyright notice and a notice that there is no warranty (or
+    else, saying that you provide a warranty) and that users may redistribute
+    the program under these conditions, and telling the user how to view a copy
+    of this License. (Exception: if the Program itself is interactive but does
+    not normally print such an announcement, your work based on the Program is
+    not required to print an announcement.)
+
+These requirements apply to the modified work as a whole. If identifiable
+sections of that work are not derived from the Program, and can be reasonably
+considered independent and separate works in themselves, then this License, and
+its terms, do not apply to those sections when you distribute them as separate
+works. But when you distribute the same sections as part of a whole which is a
+work based on the Program, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the entire whole,
+and thus to each and every part regardless of who wrote it.
+
+Thus, it is not the intent of this section to claim rights or contest your
+rights to work written entirely by you; rather, the intent is to exercise the
+right to control the distribution of derivative or collective works based on the
+Program.
+
+In addition, mere aggregation of another work not based on the Program with the
+Program (or with a work based on the Program) on a volume of a storage or
+distribution medium does not bring the other work under the scope of this
+License.
+
+**3.** You may copy and distribute the Program (or a work based on it, under
+Section 2) in object code or executable form under the terms of Sections 1 and 2
+above provided that you also do one of the following:
+
+*   **a)** Accompany it with the complete corresponding machine-readable source
+    code, which must be distributed under the terms of Sections 1 and 2 above on
+    a medium customarily used for software interchange; or,
+
+*   **b)** Accompany it with a written offer, valid for at least three years, to
+    give any third party, for a charge no more than your cost of physically
+    performing source distribution, a complete machine-readable copy of the
+    corresponding source code, to be distributed under the terms of Sections 1
+    and 2 above on a medium customarily used for software interchange; or,
+
+*   **c)** Accompany it with the information you received as to the offer to
+    distribute corresponding source code. (This alternative is allowed only for
+    noncommercial distribution and only if you received the program in object
+    code or executable form with such an offer, in accord with Subsection b
+    above.)
+
+The source code for a work means the preferred form of the work for making
+modifications to it. For an executable work, complete source code means all the
+source code for all modules it contains, plus any associated interface
+definition files, plus the scripts used to control compilation and installation
+of the executable. However, as a special exception, the source code distributed
+need not include anything that is normally distributed (in either source or
+binary form) with the major components (compiler, kernel, and so on) of the
+operating system on which the executable runs, unless that component itself
+accompanies the executable.
+
+If distribution of executable or object code is made by offering access to copy
+from a designated place, then offering equivalent access to copy the source code
+from the same place counts as distribution of the source code, even though third
+parties are not compelled to copy the source along with the object code.
+
+**4.** You may not copy, modify, sublicense, or distribute the Program except as
+expressly provided under this License. Any attempt otherwise to copy, modify,
+sublicense or distribute the Program is void, and will automatically terminate
+your rights under this License. However, parties who have received copies, or
+rights, from you under this License will not have their licenses terminated so
+long as such parties remain in full compliance.
+
+**5.** You are not required to accept this License, since you have not signed
+it. However, nothing else grants you permission to modify or distribute the
+Program or its derivative works. These actions are prohibited by law if you do
+not accept this License. Therefore, by modifying or distributing the Program (or
+any work based on the Program), you indicate your acceptance of this License to
+do so, and all its terms and conditions for copying, distributing or modifying
+the Program or works based on it.
+
+**6.** Each time you redistribute the Program (or any work based on the
+Program), the recipient automatically receives a license from the original
+licensor to copy, distribute or modify the Program subject to these terms and
+conditions. You may not impose any further restrictions on the recipients'
+exercise of the rights granted herein. You are not responsible for enforcing
+compliance by third parties to this License.
+
+**7.** If, as a consequence of a court judgment or allegation of patent
+infringement or for any other reason (not limited to patent issues), conditions
+are imposed on you (whether by court order, agreement or otherwise) that
+contradict the conditions of this License, they do not excuse you from the
+conditions of this License. If you cannot distribute so as to satisfy
+simultaneously your obligations under this License and any other pertinent
+obligations, then as a consequence you may not distribute the Program at all.
+For example, if a patent license would not permit royalty-free redistribution of
+the Program by all those who receive copies directly or indirectly through you,
+then the only way you could satisfy both it and this License would be to refrain
+entirely from distribution of the Program.
+
+If any portion of this section is held invalid or unenforceable under any
+particular circumstance, the balance of the section is intended to apply and the
+section as a whole is intended to apply in other circumstances.
+
+It is not the purpose of this section to induce you to infringe any patents or
+other property right claims or to contest validity of any such claims; this
+section has the sole purpose of protecting the integrity of the free software
+distribution system, which is implemented by public license practices. Many
+people have made generous contributions to the wide range of software
+distributed through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing to
+distribute software through any other system and a licensee cannot impose that
+choice.
+
+This section is intended to make thoroughly clear what is believed to be a
+consequence of the rest of this License.
+
+**8.** If the distribution and/or use of the Program is restricted in certain
+countries either by patents or by copyrighted interfaces, the original copyright
+holder who places the Program under this License may add an explicit
+geographical distribution limitation excluding those countries, so that
+distribution is permitted only in or among countries not thus excluded. In such
+case, this License incorporates the limitation as if written in the body of this
+License.
+
+**9.** The Free Software Foundation may publish revised and/or new versions of
+the General Public License from time to time. Such new versions will be similar
+in spirit to the present version, but may differ in detail to address new
+problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies
+a version number of this License which applies to it and "any later version",
+you have the option of following the terms and conditions either of that version
+or of any later version published by the Free Software Foundation. If the
+Program does not specify a version number of this License, you may choose any
+version ever published by the Free Software Foundation.
+
+**10.** If you wish to incorporate parts of the Program into other free programs
+whose distribution conditions are different, write to the author to ask for
+permission. For software which is copyrighted by the Free Software Foundation,
+write to the Free Software Foundation; we sometimes make exceptions for this.
+Our decision will be guided by the two goals of preserving the free status of
+all derivatives of our free software and of promoting the sharing and reuse of
+software generally.
+
+
+No Warranty
+-----------
+
+**11.** BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY FOR
+THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE
+STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM
+"AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING,
+BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
+PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+**12.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR REDISTRIBUTE
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR
+INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA
+BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
+FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER
 OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
```

### Comparing `winpcapy-1.0.2/README.rst` & `winpcapy-1.0.3/README.rst`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-winpcapy
-========
-
-| A Modern Python wrapper for WinPcap
-| Access WinPcap through ctypes.
-
-Based on Massimo Ciani’s WinPcapy (https://code.google.com/p/winpcapy/)
-
-
-Install
--------
-pip install winpcapy
-
-Usage
------
-
-Quick packet live log printer
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. code:: python
-
-    >>> from winpcapy import WinPcapUtils
-    # run on the first Ethernert interface and print a log for each packet
-    >>> WinPcapUtils.capture_on_and_print("*Ethernet*")
-    16:05:49,624258 len:199
-    16:05:49,685950 len:60
-    16:05:49,686022 len:54
-    16:05:49,767311 len:66
-    16:05:49,819156 len:66
-    16:05:50,052113 len:92
-    16:05:50,128862 len:60
-
-Easy Packet live callback
-~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. code:: python
-
-    from winpcapy import WinPcapUtils
-
-    # Example Callback function to parse IP packets
-    def packet_callback(win_pcap, param, header, pkt_data):
-        # Assuming IP (for real parsing use modules like dpkt)
-        ip_frame = pkt_data[14:]
-        # Parse ips
-        src_ip = ".".join([str(ord(b)) for b in ip_frame[0xc:0x10]])
-        dst_ip = ".".join([str(ord(b)) for b in ip_frame[0x10:0x14]])
-        print("%s -> %s" % (src_ip, dst_ip))
-
-    WinPcapUtils.capture_on("*Ethernet*", packet_callback)
-
-Device/Interface enumeration
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. code:: python
-
-    >>> from winpcapy import WinPcapDevices
-    # Return a list of all the devices detected on the machine
-    >>> WinPcapDevices.list_devices()
-    {'\\Device\\NPF_{0A78B7C8-F023-1337-1337-84D448AA5126}': 'Microsoft',
-     '\\Device\\NPF_{2997B9BB-AA53-1337-1337-B862F874271C}': 'Microsoft',
-     '\\Device\\NPF_{C2EAA982-F851-1337-1337-B8D2A9BCE406}': 'Intel(R) Ethernet Connection I218-LM',
-     '\\Device\\NPF_{EAF47DBE-5B49-1337-1337-BD059E02666B}': 'Microsoft'}
-     
-     # Itearte over devices (in memory), with full details access
-    >>> with WinPcapDevices() as devices:
-    ...     for device in devices:
-    ...         print device.name, device.description, device.flags ,device.addresses.contents.netmask.contents.sa_family
-    ...         
-    "\Device\NPF_{0A78B7C8-F023-1337-1337-84D448AA5126} Microsoft 0 0"
-    "\Device\NPF_{C2EAA982-F851-1337-1337-B8D2A9BCE406} Intel(R) Ethernet Connection I218-LM 0 0"
-    "\Device\NPF_{EAF47DBE-5B49-1337-1337-BD059E02666B} Microsoft 0 0"
-    "\Device\NPF_{2997B9BB-AA53-1337-1337-B862F874271C} Microsoft 0 0"
-
-Easy Packet sending
-~~~~~~~~~~~~~~~~~~~
-
-.. code:: python
-
-    from winpcapy import WinPcapUtils
-    # Build a packet buffer
-    # This example-code is built for tutorial purposes, for actual packet crafting use modules like dpkt
-    arp_request_hex_template = "%(dst_mac)s%(src_mac)s08060001080006040001" \
-                               "%(sender_mac)s%(sender_ip)s%(target_mac)s%(target_ip)s" + "00" * 18
-    packet = arp_request_hex_template % {
-        "dst_mac": "aa"*6,
-        "src_mac": "bb"*6,
-        "sender_mac": "bb"*6,
-        "target_mac": "cc"*6,
-        # 192.168.0.1
-        "sender_ip": "c0a80001",
-        # 192.168.0.2
-        "target_ip": "c0a80002"
-    }
-    # Send the packet (ethernet frame with an arp request) on the interface
+winpcapy
+========
+
+| A Modern Python wrapper for WinPcap
+| Access WinPcap through ctypes.
+
+Based on Massimo Ciani’s WinPcapy (https://code.google.com/p/winpcapy/)
+
+
+Install
+-------
+pip install winpcapy
+
+Usage
+-----
+
+Quick packet live log printer
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    >>> from winpcapy import WinPcapUtils
+    # run on the first Ethernert interface and print a log for each packet
+    >>> WinPcapUtils.capture_on_and_print("*Ethernet*")
+    16:05:49,624258 len:199
+    16:05:49,685950 len:60
+    16:05:49,686022 len:54
+    16:05:49,767311 len:66
+    16:05:49,819156 len:66
+    16:05:50,052113 len:92
+    16:05:50,128862 len:60
+
+Easy Packet live callback
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from winpcapy import WinPcapUtils
+
+    # Example Callback function to parse IP packets
+    def packet_callback(win_pcap, param, header, pkt_data):
+        # Assuming IP (for real parsing use modules like dpkt)
+        ip_frame = pkt_data[14:]
+        # Parse ips
+        src_ip = ".".join([str(ord(b)) for b in ip_frame[0xc:0x10]])
+        dst_ip = ".".join([str(ord(b)) for b in ip_frame[0x10:0x14]])
+        print("%s -> %s" % (src_ip, dst_ip))
+
+    WinPcapUtils.capture_on("*Ethernet*", packet_callback)
+
+Device/Interface enumeration
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    >>> from winpcapy import WinPcapDevices
+    # Return a list of all the devices detected on the machine
+    >>> WinPcapDevices.list_devices()
+    {'\\Device\\NPF_{0A78B7C8-F023-1337-1337-84D448AA5126}': 'Microsoft',
+     '\\Device\\NPF_{2997B9BB-AA53-1337-1337-B862F874271C}': 'Microsoft',
+     '\\Device\\NPF_{C2EAA982-F851-1337-1337-B8D2A9BCE406}': 'Intel(R) Ethernet Connection I218-LM',
+     '\\Device\\NPF_{EAF47DBE-5B49-1337-1337-BD059E02666B}': 'Microsoft'}
+     
+     # Itearte over devices (in memory), with full details access
+    >>> with WinPcapDevices() as devices:
+    ...     for device in devices:
+    ...         print device.name, device.description, device.flags ,device.addresses.contents.netmask.contents.sa_family
+    ...         
+    "\Device\NPF_{0A78B7C8-F023-1337-1337-84D448AA5126} Microsoft 0 0"
+    "\Device\NPF_{C2EAA982-F851-1337-1337-B8D2A9BCE406} Intel(R) Ethernet Connection I218-LM 0 0"
+    "\Device\NPF_{EAF47DBE-5B49-1337-1337-BD059E02666B} Microsoft 0 0"
+    "\Device\NPF_{2997B9BB-AA53-1337-1337-B862F874271C} Microsoft 0 0"
+
+Easy Packet sending
+~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from winpcapy import WinPcapUtils
+    # Build a packet buffer
+    # This example-code is built for tutorial purposes, for actual packet crafting use modules like dpkt
+    arp_request_hex_template = "%(dst_mac)s%(src_mac)s08060001080006040001" \
+                               "%(sender_mac)s%(sender_ip)s%(target_mac)s%(target_ip)s" + "00" * 18
+    packet = arp_request_hex_template % {
+        "dst_mac": "aa"*6,
+        "src_mac": "bb"*6,
+        "sender_mac": "bb"*6,
+        "target_mac": "cc"*6,
+        # 192.168.0.1
+        "sender_ip": "c0a80001",
+        # 192.168.0.2
+        "target_ip": "c0a80002"
+    }
+    # Send the packet (ethernet frame with an arp request) on the interface
     WinPcapUtils.send_packet("*Ethernet*", packet.decode("hex"))
```

### Comparing `winpcapy-1.0.2/winpcapy/winpcapy_types.py` & `winpcapy-1.0.3/winpcapy/winpcapy_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,687 +1,687 @@
-#-------------------------------------------------------------------------------
-# Name:        winpcapy_types.py
-#
-# Author:      Massimo Ciani
-#
-# Created:     01/09/2009
-# Copyright:   (c) Massimo Ciani 2009
-#
-#-------------------------------------------------------------------------------
-
-
-from ctypes import *
-from ctypes.util import find_library
-import sys
-
-WIN32=False
-HAVE_REMOTE=False
-
-
-if sys.platform.startswith('win'):
-    WIN32=True
-    HAVE_REMOTE=True
-
-if WIN32:
-    SOCKET = c_uint
-    _lib=CDLL('wpcap.dll')
-else:
-    SOCKET = c_int
-    _lib=CDLL(find_library('pcap'))
-
-
-
-##
-## misc
-##
-u_short = c_ushort
-bpf_int32 = c_int
-u_int = c_uint
-bpf_u_int32 = u_int
-pcap = c_void_p
-pcap_dumper = c_void_p
-u_char = c_ubyte
-FILE = c_void_p
-STRING = c_char_p
-
-class bpf_insn(Structure):
-    _fields_=[("code",c_ushort),
-              ("jt",c_ubyte),
-              ("jf",c_ubyte),
-              ("k",bpf_u_int32)]
-    
-class bpf_program(Structure):
-    pass
-bpf_program._fields_ = [('bf_len', u_int),
-                        ('bf_insns', POINTER(bpf_insn))]
-
-class bpf_version(Structure):
-    _fields_=[("bv_major",c_ushort),
-              ("bv_minor",c_ushort)]
-
-
-class timeval(Structure):
-    pass
-timeval._fields_ = [('tv_sec', c_long),
-                    ('tv_usec', c_long)]
-
-## sockaddr is used by pcap_addr.
-## For exapmle if sa_family==socket.AF_INET then we need cast
-## with sockaddr_in 
-class sockaddr(Structure):
-    _fields_ = [("sa_family",c_ushort),
-                ("sa_data",c_char * 14)]
-##
-## END misc
-##
-
-##
-## Data Structures
-##
-
-## struct  	pcap_file_header
-## 	Header of a libpcap dump file.
-class pcap_file_header(Structure):
-    _fields_ = [('magic', bpf_u_int32),
-                ('version_major', u_short),
-                ('version_minor', u_short),
-                ('thiszone', bpf_int32),
-                ('sigfigs', bpf_u_int32),
-                ('snaplen', bpf_u_int32),
-                ('linktype', bpf_u_int32)]
-
-## struct  	pcap_pkthdr
-## 	Header of a packet in the dump file.
-class pcap_pkthdr(Structure):
-    _fields_ = [('ts', timeval),
-                ('caplen', bpf_u_int32),
-                ('len', bpf_u_int32)]
-
-## struct  	pcap_stat
-## 	Structure that keeps statistical values on an interface.
-class pcap_stat(Structure):
-    pass
-### _fields_ list in Structure is final.
-### We need a temp list
-_tmpList=[]
-_tmpList.append(("ps_recv",c_uint))
-_tmpList.append(("ps_drop",c_uint))
-_tmpList.append(("ps_ifdrop",c_uint))
-if HAVE_REMOTE:
-    _tmpList.append(("ps_capt",c_uint))
-    _tmpList.append(("ps_sent",c_uint))
-    _tmpList.append(("ps_netdrop",c_uint))
-pcap_stat._fields_=_tmpList
-
-## struct  	pcap_addr
-## 	Representation of an interface address, used by pcap_findalldevs().
-class pcap_addr(Structure):
-    pass
-pcap_addr._fields_ = [('next', POINTER(pcap_addr)),
-                      ('addr', POINTER(sockaddr)),
-                      ('netmask', POINTER(sockaddr)),
-                      ('broadaddr', POINTER(sockaddr)),
-                      ('dstaddr', POINTER(sockaddr))]
-
-## struct  	pcap_if
-## 	Item in a list of interfaces, used by pcap_findalldevs().
-class pcap_if(Structure):
-    pass
-pcap_if._fields_ = [('next', POINTER(pcap_if)),
-                    ('name', STRING),
-                    ('description', STRING),
-                    ('addresses', POINTER(pcap_addr)),
-                    ('flags', bpf_u_int32)]
-
-##
-## END Data Structures
-##
-
-##
-## Defines
-##
-
-##define 	PCAP_VERSION_MAJOR   2
-# 	Major libpcap dump file version.
-PCAP_VERSION_MAJOR = 2 
-##define 	PCAP_VERSION_MINOR   4
-# 	Minor libpcap dump file version.
-PCAP_VERSION_MINOR = 4 
-##define 	PCAP_ERRBUF_SIZE   256
-# 	Size to use when allocating the buffer that contains the libpcap errors.
-PCAP_ERRBUF_SIZE = 256 
-##define 	PCAP_IF_LOOPBACK   0x00000001
-# 	interface is loopback
-PCAP_IF_LOOPBACK = 1 
-##define 	MODE_CAPT   0
-# 	Capture mode, to be used when calling pcap_setmode().
-MODE_CAPT = 0
-##define 	MODE_STAT   1
-# 	Statistical mode, to be used when calling pcap_setmode().
-MODE_STAT = 1
-
-##
-## END Defines
-##
-
-##
-## Typedefs
-##
-
-#typedef int 	bpf_int32 (already defined)
-# 	32-bit integer
-#typedef u_int 	bpf_u_int32 (already defined)
-# 	32-bit unsigned integer
-#typedef struct pcap 	pcap_t
-# 	Descriptor of an open capture instance. This structure is opaque to the user, that handles its content through the functions provided by wpcap.dll.
-pcap_t = pcap
-#typedef struct pcap_dumper 	pcap_dumper_t
-# 	libpcap savefile descriptor.
-pcap_dumper_t = pcap_dumper
-#typedef struct pcap_if 	pcap_if_t
-# 	Item in a list of interfaces, see pcap_if.
-pcap_if_t = pcap_if
-#typedef struct pcap_addr 	pcap_addr_t
-# 	Representation of an interface address, see pcap_addr.
-pcap_addr_t = pcap_addr
-
-##
-## END Typedefs
-##
-
-
-
-
-
-# values for enumeration 'pcap_direction_t'
-#pcap_direction_t = c_int # enum
-
-##
-## Unix-compatible Functions
-## These functions are part of the libpcap library, and therefore work both on Windows and on Linux. 
-##
-
-#typedef void(* pcap_handler )(u_char *user, const struct pcap_pkthdr *pkt_header, const u_char *pkt_data)
-# 	Prototype of the callback function that receives the packets.
-## This one is defined from programmer
-pcap_handler=CFUNCTYPE(None,POINTER(c_ubyte),POINTER(pcap_pkthdr),POINTER(c_ubyte))
-
-#pcap_t *   pcap_open_live (const char *device, int snaplen, int promisc, int to_ms, char *ebuf)
-# 	Open a live capture from the network.
-pcap_open_live = _lib.pcap_open_live
-pcap_open_live.restype = POINTER(pcap_t)
-pcap_open_live.argtypes = [STRING, c_int, c_int, c_int, STRING]
-
-#pcap_t *   pcap_open_dead (int linktype, int snaplen)
-# 	Create a pcap_t structure without starting a capture.
-pcap_open_dead = _lib.pcap_open_dead
-pcap_open_dead.restype = POINTER(pcap_t)
-pcap_open_dead.argtypes = [c_int, c_int]
-
-#pcap_t *   pcap_open_offline (const char *fname, char *errbuf)
-# 	Open a savefile in the tcpdump/libpcap format to read packets.
-pcap_open_offline = _lib.pcap_open_offline
-pcap_open_offline.restype = POINTER(pcap_t)
-pcap_open_offline.argtypes = [STRING, STRING]
-
-#pcap_dumper_t *   pcap_dump_open (pcap_t *p, const char *fname)
-# 	Open a file to write packets.
-pcap_dump_open = _lib.pcap_dump_open
-pcap_dump_open.restype = POINTER(pcap_dumper_t)
-pcap_dump_open.argtypes = [POINTER(pcap_t), STRING]
-
-#int pcap_setnonblock (pcap_t *p, int nonblock, char *errbuf)
-# 	Switch between blocking and nonblocking mode.
-pcap_setnonblock = _lib.pcap_setnonblock
-pcap_setnonblock.restype = c_int
-pcap_setnonblock.argtypes = [POINTER(pcap_t), c_int, STRING]
-
-#int pcap_getnonblock (pcap_t *p, char *errbuf)
-# 	Get the "non-blocking" state of an interface.
-pcap_getnonblock = _lib.pcap_getnonblock
-pcap_getnonblock.restype = c_int
-pcap_getnonblock.argtypes = [POINTER(pcap_t), STRING]
-
-#int pcap_findalldevs (pcap_if_t **alldevsp, char *errbuf)
-# 	Construct a list of network devices that can be opened with pcap_open_live().
-pcap_findalldevs = _lib.pcap_findalldevs
-pcap_findalldevs.restype = c_int
-pcap_findalldevs.argtypes = [POINTER(POINTER(pcap_if_t)), STRING]
-
-#void pcap_freealldevs (pcap_if_t *alldevsp)
-# 	Free an interface list returned by pcap_findalldevs().
-pcap_freealldevs = _lib.pcap_freealldevs
-pcap_freealldevs.restype = None
-pcap_freealldevs.argtypes = [POINTER(pcap_if_t)]
-
-#char *   pcap_lookupdev (char *errbuf)
-# 	Return the first valid device in the system.
-pcap_lookupdev = _lib.pcap_lookupdev
-pcap_lookupdev.restype = STRING
-pcap_lookupdev.argtypes = [STRING]
-
-#int pcap_lookupnet (const char *device, bpf_u_int32 *netp, bpf_u_int32 *maskp, char *errbuf)
-# 	Return the subnet and netmask of an interface.
-pcap_lookupnet = _lib.pcap_lookupnet
-pcap_lookupnet.restype = c_int
-pcap_lookupnet.argtypes = [STRING, POINTER(bpf_u_int32), POINTER(bpf_u_int32), STRING]
-
-#int pcap_dispatch (pcap_t *p, int cnt, pcap_handler callback, u_char *user)
-# 	Collect a group of packets.
-pcap_dispatch = _lib.pcap_dispatch
-pcap_dispatch.restype = c_int
-pcap_dispatch.argtypes = [POINTER(pcap_t), c_int, pcap_handler, POINTER(u_char)]
-
-#int pcap_loop (pcap_t *p, int cnt, pcap_handler callback, u_char *user)
-# 	Collect a group of packets.
-pcap_loop = _lib.pcap_loop
-pcap_loop.restype = c_int
-pcap_loop.argtypes = [POINTER(pcap_t), c_int, pcap_handler, POINTER(u_char)]
-
-#u_char *   pcap_next (pcap_t *p, struct pcap_pkthdr *h)
-# 	Return the next available packet.
-pcap_next = _lib.pcap_next
-pcap_next.restype = POINTER(u_char)
-pcap_next.argtypes = [POINTER(pcap_t), POINTER(pcap_pkthdr)]
-
-#int pcap_next_ex (pcap_t *p, struct pcap_pkthdr **pkt_header, const u_char **pkt_data)
-# 	Read a packet from an interface or from an offline capture.
-pcap_next_ex = _lib.pcap_next_ex
-pcap_next_ex.restype = c_int
-pcap_next_ex.argtypes = [POINTER(pcap_t), POINTER(POINTER(pcap_pkthdr)), POINTER(POINTER(u_char))]
-
-#void pcap_breakloop (pcap_t *)
-# 	set a flag that will force pcap_dispatch() or pcap_loop() to return rather than looping.
-pcap_breakloop = _lib.pcap_breakloop
-pcap_breakloop.restype = None
-pcap_breakloop.argtypes = [POINTER(pcap_t)]
-
-#int pcap_sendpacket (pcap_t *p, u_char *buf, int size)
-# 	Send a raw packet.
-pcap_sendpacket = _lib.pcap_sendpacket
-pcap_sendpacket.restype = c_int
-pcap_sendpacket.argtypes = [POINTER(pcap_t), POINTER(u_char), c_int]
-
-#void pcap_dump (u_char *user, const struct pcap_pkthdr *h, const u_char *sp)
-# 	Save a packet to disk.
-pcap_dump = _lib.pcap_dump
-pcap_dump.restype = None
-pcap_dump.argtypes = [POINTER(pcap_dumper_t), POINTER(pcap_pkthdr), POINTER(u_char)]
-
-#long pcap_dump_ftell (pcap_dumper_t *)
-# 	Return the file position for a "savefile".
-pcap_dump_ftell = _lib.pcap_dump_ftell
-pcap_dump_ftell.restype = c_long
-pcap_dump_ftell.argtypes = [POINTER(pcap_dumper_t)]
-
-#int pcap_compile (pcap_t *p, struct bpf_program *fp, char *str, int optimize, bpf_u_int32 netmask)
-# 	Compile a packet filter, converting an high level filtering expression (see Filtering expression syntax) in a program that can be interpreted by the kernel-level filtering engine.
-pcap_compile = _lib.pcap_compile
-pcap_compile.restype = c_int
-pcap_compile.argtypes = [POINTER(pcap_t), POINTER(bpf_program), STRING, c_int, bpf_u_int32]
-
-#int pcap_compile_nopcap (int snaplen_arg, int linktype_arg, struct bpf_program *program, char *buf, int optimize, bpf_u_int32 mask)
-# 	Compile a packet filter without the need of opening an adapter. This function converts an high level filtering expression (see Filtering expression syntax) in a program that can be interpreted by the kernel-level filtering engine.
-pcap_compile_nopcap = _lib.pcap_compile_nopcap
-pcap_compile_nopcap.restype = c_int
-pcap_compile_nopcap.argtypes = [c_int, c_int, POINTER(bpf_program), STRING, c_int, bpf_u_int32]
-
-#int pcap_setfilter (pcap_t *p, struct bpf_program *fp)
-# 	Associate a filter to a capture.
-pcap_setfilter = _lib.pcap_setfilter
-pcap_setfilter.restype = c_int
-pcap_setfilter.argtypes = [POINTER(pcap_t), POINTER(bpf_program)]
-
-#void pcap_freecode (struct bpf_program *fp)
-# 	Free a filter.
-pcap_freecode = _lib.pcap_freecode
-pcap_freecode.restype = None
-pcap_freecode.argtypes = [POINTER(bpf_program)]
-
-#int pcap_datalink (pcap_t *p)
-# 	Return the link layer of an adapter.
-pcap_datalink = _lib.pcap_datalink
-pcap_datalink.restype = c_int
-pcap_datalink.argtypes = [POINTER(pcap_t)]
-
-#int pcap_list_datalinks (pcap_t *p, int **dlt_buf)
-# 	list datalinks
-pcap_list_datalinks = _lib.pcap_list_datalinks
-pcap_list_datalinks.restype = c_int
-#pcap_list_datalinks.argtypes = [POINTER(pcap_t), POINTER(POINTER(c_int))]
-
-#int pcap_set_datalink (pcap_t *p, int dlt)
-# 	Set the current data link type of the pcap descriptor to the type specified by dlt. -1 is returned on failure.
-pcap_set_datalink = _lib.pcap_set_datalink
-pcap_set_datalink.restype = c_int
-pcap_set_datalink.argtypes = [POINTER(pcap_t), c_int]
-
-#int pcap_datalink_name_to_val (const char *name)
-# 	Translates a data link type name, which is a DLT_ name with the DLT_ removed, to the corresponding data link type value. The translation is case-insensitive. -1 is returned on failure.
-pcap_datalink_name_to_val = _lib.pcap_datalink_name_to_val
-pcap_datalink_name_to_val.restype = c_int
-pcap_datalink_name_to_val.argtypes = [STRING]
-
-#const char * 	pcap_datalink_val_to_name (int dlt)
-# 	Translates a data link type value to the corresponding data link type name. NULL is returned on failure.
-pcap_datalink_val_to_name = _lib.pcap_datalink_val_to_name
-pcap_datalink_val_to_name.restype = STRING
-pcap_datalink_val_to_name.argtypes = [c_int]
-
-#const char * 	pcap_datalink_val_to_description (int dlt)
-# 	Translates a data link type value to a short description of that data link type. NULL is returned on failure.
-pcap_datalink_val_to_description = _lib.pcap_datalink_val_to_description
-pcap_datalink_val_to_description.restype = STRING
-pcap_datalink_val_to_description.argtypes = [c_int]
-
-#int pcap_snapshot (pcap_t *p)
-# 	Return the dimension of the packet portion (in bytes) that is delivered to the application.
-pcap_snapshot = _lib.pcap_snapshot
-pcap_snapshot.restype = c_int
-pcap_snapshot.argtypes = [POINTER(pcap_t)]
-
-#int pcap_is_swapped (pcap_t *p)
-# 	returns true if the current savefile uses a different byte order than the current system.
-pcap_is_swapped = _lib.pcap_is_swapped
-pcap_is_swapped.restype = c_int
-pcap_is_swapped.argtypes = [POINTER(pcap_t)]
-
-#int pcap_major_version (pcap_t *p)
-# 	return the major version number of the pcap library used to write the savefile.
-pcap_major_version = _lib.pcap_major_version
-pcap_major_version.restype = c_int
-pcap_major_version.argtypes = [POINTER(pcap_t)]
-
-#int pcap_minor_version (pcap_t *p)
-# 	return the minor version number of the pcap library used to write the savefile.
-pcap_minor_version = _lib.pcap_minor_version
-pcap_minor_version.restype = c_int
-pcap_minor_version.argtypes = [POINTER(pcap_t)]
-
-#FILE *   pcap_file (pcap_t *p)
-# 	Return the standard stream of an offline capture.
-pcap_file=_lib.pcap_file
-pcap_file.restype = FILE
-pcap_file.argtypes = [POINTER(pcap_t)]
-
-#int pcap_stats (pcap_t *p, struct pcap_stat *ps)
-# 	Return statistics on current capture.
-pcap_stats = _lib.pcap_stats
-pcap_stats.restype = c_int
-pcap_stats.argtypes = [POINTER(pcap_t), POINTER(pcap_stat)]
-
-#void pcap_perror (pcap_t *p, char *prefix)
-# 	print the text of the last pcap library error on stderr, prefixed by prefix.
-pcap_perror = _lib.pcap_perror
-pcap_perror.restype = None
-pcap_perror.argtypes = [POINTER(pcap_t), STRING]
-
-#char *   pcap_geterr (pcap_t *p)
-# 	return the error text pertaining to the last pcap library error.
-pcap_geterr = _lib.pcap_geterr
-pcap_geterr.restype = STRING
-pcap_geterr.argtypes = [POINTER(pcap_t)]
-
-#char *   pcap_strerror (int error)
-# 	Provided in case strerror() isn't available.
-pcap_strerror = _lib.pcap_strerror
-pcap_strerror.restype = STRING
-pcap_strerror.argtypes = [c_int]
-
-#const char *   pcap_lib_version (void)
-# 	Returns a pointer to a string giving information about the version of the libpcap library being used; note that it contains more information than just a version number.
-pcap_lib_version = _lib.pcap_lib_version
-pcap_lib_version.restype = STRING
-pcap_lib_version.argtypes = []
-
-#void pcap_close (pcap_t *p)
-# 	close the files associated with p and deallocates resources.
-pcap_close = _lib.pcap_close
-pcap_close.restype = None
-pcap_close.argtypes = [POINTER(pcap_t)]
-
-#FILE *   pcap_dump_file (pcap_dumper_t *p)
-# 	return the standard I/O stream of the 'savefile' opened by pcap_dump_open().
-pcap_dump_file=_lib.pcap_dump_file
-pcap_dump_file.restype=FILE
-pcap_dump_file.argtypes= [POINTER(pcap_dumper_t)]
-
-#int pcap_dump_flush (pcap_dumper_t *p)
-# 	Flushes the output buffer to the ``savefile,'' so that any packets written with pcap_dump() but not yet written to the ``savefile'' will be written. -1 is returned on error, 0 on success.
-pcap_dump_flush = _lib.pcap_dump_flush
-pcap_dump_flush.restype = c_int
-pcap_dump_flush.argtypes = [POINTER(pcap_dumper_t)]
-
-#void pcap_dump_close (pcap_dumper_t *p)
-# 	Closes a savefile. 
-pcap_dump_close = _lib.pcap_dump_close
-pcap_dump_close.restype = None
-pcap_dump_close.argtypes = [POINTER(pcap_dumper_t)]
-
-###########################################
-## Windows-specific Extensions
-## The functions in this section extend libpcap to offer advanced functionalities
-## (like remote packet capture, packet buffer size variation or high-precision packet injection).
-## Howerver, at the moment they can be used only in Windows.
-###########################################
-if WIN32:
-    HANDLE = c_void_p
-    
-    ##############
-    ## Identifiers related to the new source syntax
-    ##############
-    #define 	PCAP_SRC_FILE   2
-    #define 	PCAP_SRC_IFLOCAL   3
-    #define 	PCAP_SRC_IFREMOTE   4
-    #Internal representation of the type of source in use (file, remote/local interface).
-    PCAP_SRC_FILE = 2
-    PCAP_SRC_IFLOCAL = 3
-    PCAP_SRC_IFREMOTE = 4
-    
-    ##############
-    ## Strings related to the new source syntax
-    ##############
-    #define 	PCAP_SRC_FILE_STRING   "file://"
-    #define 	PCAP_SRC_IF_STRING   "rpcap://"
-    #String that will be used to determine the type of source in use (file, remote/local interface).
-    PCAP_SRC_FILE_STRING="file://"
-    PCAP_SRC_IF_STRING="rpcap://"
-    
-    ##############
-    ## Flags defined in the pcap_open() function
-    ##############
-    # define 	PCAP_OPENFLAG_PROMISCUOUS   1
-    # 	Defines if the adapter has to go in promiscuous mode.
-    PCAP_OPENFLAG_PROMISCUOUS=1
-    # define 	PCAP_OPENFLAG_DATATX_UDP   2
-    # 	Defines if the data trasfer (in case of a remote capture) has to be done with UDP protocol.
-    PCAP_OPENFLAG_DATATX_UDP=2
-    # define 	PCAP_OPENFLAG_NOCAPTURE_RPCAP   4
-    PCAP_OPENFLAG_NOCAPTURE_RPCAP=4
-    # 	Defines if the remote probe will capture its own generated traffic.
-    # define 	PCAP_OPENFLAG_NOCAPTURE_LOCAL   8
-    PCAP_OPENFLAG_NOCAPTURE_LOCAL = 8
-    # define 	PCAP_OPENFLAG_MAX_RESPONSIVENESS   16
-    # 	This flag configures the adapter for maximum responsiveness.
-    PCAP_OPENFLAG_MAX_RESPONSIVENESS=16
-    
-    ##############
-    ## Sampling methods defined in the pcap_setsampling() function
-    ##############
-    # define 	PCAP_SAMP_NOSAMP   0
-    # No sampling has to be done on the current capture.
-    PCAP_SAMP_NOSAMP=0
-    # define 	PCAP_SAMP_1_EVERY_N   1
-    # It defines that only 1 out of N packets must be returned to the user.
-    PCAP_SAMP_1_EVERY_N=1
-    #define 	PCAP_SAMP_FIRST_AFTER_N_MS   2
-    # It defines that we have to return 1 packet every N milliseconds.
-    PCAP_SAMP_FIRST_AFTER_N_MS=2
-    
-    ##############
-    ## Authentication methods supported by the RPCAP protocol
-    ##############
-    # define 	RPCAP_RMTAUTH_NULL   0
-    # It defines the NULL authentication.
-    RPCAP_RMTAUTH_NULL=0
-    # define 	RPCAP_RMTAUTH_PWD   1
-    # It defines the username/password authentication.
-    RPCAP_RMTAUTH_PWD=1
-    
-
-    ##############
-    ## Remote struct and defines
-    ##############
-    # define 	PCAP_BUF_SIZE   1024
-    # Defines the maximum buffer size in which address, port, interface names are kept.
-    PCAP_BUF_SIZE = 1024
-    # define 	RPCAP_HOSTLIST_SIZE   1024
-    # Maximum lenght of an host name (needed for the RPCAP active mode).
-    RPCAP_HOSTLIST_SIZE = 1024
-    
-    class pcap_send_queue(Structure):
-        _fields_=[("maxlen",c_uint),
-                  ("len",c_uint),
-                  ("buffer",c_char_p)]
-        
-    ## struct  	pcap_rmtauth
-    ## This structure keeps the information needed to autheticate the user on a remote machine
-    class pcap_rmtauth(Structure):
-        _fields_=[("type",c_int),
-                  ("username",c_char_p),
-                  ("password",c_char_p)]
-    
-    ## struct  	pcap_samp
-    ## This structure defines the information related to sampling    
-    class pcap_samp(Structure):
-        _fields_=[("method",c_int),
-                  ("value",c_int)]
-
-    #PAirpcapHandle 	pcap_get_airpcap_handle (pcap_t *p)
-    # 	Returns the AirPcap handler associated with an adapter. This handler can be used to change the wireless-related settings of the CACE Technologies AirPcap wireless capture adapters.
-    
-    #bool pcap_offline_filter (struct bpf_program *prog, const struct pcap_pkthdr *header, const u_char *pkt_data)
-    # 	Returns if a given filter applies to an offline packet.
-    pcap_offline_filter = _lib.pcap_offline_filter
-    pcap_offline_filter.restype = c_bool
-    pcap_offline_filter.argtypes = [POINTER(bpf_program),POINTER(pcap_pkthdr),POINTER(u_char)]
-    
-    #int pcap_live_dump (pcap_t *p, char *filename, int maxsize, int maxpacks)
-    # 	Save a capture to file.
-    pcap_live_dump = _lib.pcap_live_dump
-    pcap_live_dump.restype = c_int
-    pcap_live_dump.argtypes = [POINTER(pcap_t), POINTER(c_char), c_int,c_int]
-    
-    #int pcap_live_dump_ended (pcap_t *p, int sync)
-    # 	Return the status of the kernel dump process, i.e. tells if one of the limits defined with pcap_live_dump() has been reached.
-    pcap_live_dump_ended = _lib.pcap_live_dump_ended
-    pcap_live_dump_ended.restype = c_int
-    pcap_live_dump_ended.argtypes = [POINTER(pcap_t), c_int]
-    
-    #struct pcap_stat *  pcap_stats_ex (pcap_t *p, int *pcap_stat_size)
-    # 	Return statistics on current capture.
-    pcap_stats_ex = _lib.pcap_stats_ex
-    pcap_stats_ex.restype = POINTER(pcap_stat)
-    pcap_stats_ex.argtypes = [POINTER(pcap_t), POINTER(c_int)]
-    
-    #int pcap_setbuff (pcap_t *p, int dim)
-    # 	Set the size of the kernel buffer associated with an adapter.
-    pcap_setbuff = _lib.pcap_setbuff
-    pcap_setbuff.restype = c_int
-    pcap_setbuff.argtypes = [POINTER(pcap_t), c_int]
-    
-    #int pcap_setmode (pcap_t *p, int mode)
-    # 	Set the working mode of the interface p to mode.
-    pcap_setmode = _lib.pcap_setmode
-    pcap_setmode.restype = c_int
-    pcap_setmode.argtypes = [POINTER(pcap_t), c_int]
-    
-    #int pcap_setmintocopy (pcap_t *p, int size)
-    # 	Set the minumum amount of data received by the kernel in a single call.
-    pcap_setmintocopy = _lib.pcap_setmintocopy
-    pcap_setmintocopy.restype = c_int
-    pcap_setmintocopy.argtype = [POINTER(pcap_t), c_int]
-    
-    #HANDLE pcap_getevent (pcap_t *p)
-    # 	Return the handle of the event associated with the interface p.
-    pcap_getevent = _lib.pcap_getevent
-    pcap_getevent.restype = HANDLE
-    pcap_getevent.argtypes = [POINTER(pcap_t)]
-
-    #pcap_send_queue * 	pcap_sendqueue_alloc (u_int memsize)
-    # 	Allocate a send queue.
-    pcap_sendqueue_alloc = _lib.pcap_sendqueue_alloc
-    pcap_sendqueue_alloc.restype = POINTER(pcap_send_queue)
-    pcap_sendqueue_alloc.argtypes = [c_uint]
-    
-    #void pcap_sendqueue_destroy (pcap_send_queue *queue)
-    # 	Destroy a send queue.
-    pcap_sendqueue_destroy = _lib.pcap_sendqueue_destroy
-    pcap_sendqueue_destroy.restype = None
-    pcap_sendqueue_destroy.argtypes = [POINTER(pcap_send_queue)]
-    
-    #int pcap_sendqueue_queue (pcap_send_queue *queue, const struct pcap_pkthdr *pkt_header, const u_char *pkt_data)
-    # 	Add a packet to a send queue.
-    pcap_sendqueue_queue = _lib.pcap_sendqueue_queue
-    pcap_sendqueue_queue.restype = c_int
-    pcap_sendqueue_queue.argtypes = [POINTER(pcap_send_queue), POINTER(pcap_pkthdr), POINTER(u_char)]
-    
-    #u_int pcap_sendqueue_transmit (pcap_t *p, pcap_send_queue *queue, int sync)
-    # 	Send a queue of raw packets to the network.
-    pcap_sendqueue_transmit = _lib.pcap_sendqueue_transmit
-    pcap_sendqueue_transmit.retype = u_int
-    pcap_sendqueue_transmit.argtypes = [POINTER(pcap_t), POINTER(pcap_send_queue), c_int]
-    
-    #int pcap_findalldevs_ex (char *source, struct pcap_rmtauth *auth, pcap_if_t **alldevs, char *errbuf)
-    # 	Create a list of network devices that can be opened with pcap_open().
-    pcap_findalldevs_ex = _lib.pcap_findalldevs_ex
-    pcap_findalldevs_ex.retype = c_int
-    pcap_findalldevs_ex.argtypes = [STRING, POINTER(pcap_rmtauth), POINTER(POINTER(pcap_if_t)), STRING]
-    
-    #int pcap_createsrcstr (char *source, int type, const char *host, const char *port, const char *name, char *errbuf)
-    # 	Accept a set of strings (host name, port, ...), and it returns the complete source string according to the new format (e.g. 'rpcap://1.2.3.4/eth0').
-    pcap_createsrcstr = _lib.pcap_createsrcstr
-    pcap_createsrcstr.restype = c_int
-    pcap_createsrcstr.argtypes = [STRING, c_int, STRING, STRING, STRING, STRING]
-    
-    #int pcap_parsesrcstr (const char *source, int *type, char *host, char *port, char *name, char *errbuf)
-    # 	Parse the source string and returns the pieces in which the source can be split.
-    pcap_parsesrcstr = _lib.pcap_parsesrcstr
-    pcap_parsesrcstr.retype = c_int
-    pcap_parsesrcstr.argtypes = [STRING, POINTER(c_int), STRING, STRING, STRING, STRING]
-    
-    #pcap_t * 	pcap_open (const char *source, int snaplen, int flags, int read_timeout, struct pcap_rmtauth *auth, char *errbuf)
-    # 	Open a generic source in order to capture / send (WinPcap only) traffic.
-    pcap_open = _lib.pcap_open
-    pcap_open.restype = POINTER(pcap_t)
-    pcap_open.argtypes = [STRING, c_int, c_int, c_int, POINTER(pcap_rmtauth), STRING]
-    
-    #struct pcap_samp *  pcap_setsampling (pcap_t *p)
-    # 	Define a sampling method for packet capture.
-    pcap_setsampling = _lib.pcap_setsampling
-    pcap_setsampling.restype = POINTER(pcap_samp)
-    pcap_setsampling.argtypes = [POINTER(pcap_t)]
-    
-    #SOCKET pcap_remoteact_accept (const char *address, const char *port, const char *hostlist, char *connectinghost, struct pcap_rmtauth *auth, char *errbuf)
-    # 	Block until a network connection is accepted (active mode only).
-    pcap_remoteact_accept = _lib.pcap_remoteact_accept
-    pcap_remoteact_accept.restype = SOCKET
-    pcap_remoteact_accept.argtypes = [STRING, STRING, STRING, STRING, POINTER(pcap_rmtauth), STRING]
-    
-    #int pcap_remoteact_close (const char *host, char *errbuf)
-    # 	Drop an active connection (active mode only).
-    pcap_remoteact_close = _lib.pcap_remoteact_close
-    pcap_remoteact_close.restypes = c_int
-    pcap_remoteact_close.argtypes = [STRING, STRING]
-    
-    #void pcap_remoteact_cleanup ()
-    # 	Clean the socket that is currently used in waiting active connections.
-    pcap_remoteact_cleanup = _lib.pcap_remoteact_cleanup
-    pcap_remoteact_cleanup.restypes = None
-    pcap_remoteact_cleanup.argtypes = []
-    
-    #int pcap_remoteact_list (char *hostlist, char sep, int size, char *errbuf)
-    # 	Return the hostname of the host that have an active connection with us (active mode only). 
-    pcap_remoteact_list = _lib.pcap_remoteact_list
-    pcap_remoteact_list.restype = c_int
-    pcap_remoteact_list.argtypes = [STRING, c_char, c_int, STRING]
-    
+#-------------------------------------------------------------------------------
+# Name:        winpcapy_types.py
+#
+# Author:      Massimo Ciani
+#
+# Created:     01/09/2009
+# Copyright:   (c) Massimo Ciani 2009
+#
+#-------------------------------------------------------------------------------
+
+
+from ctypes import *
+from ctypes.util import find_library
+import sys
+
+WIN32=False
+HAVE_REMOTE=False
+
+
+if sys.platform.startswith('win') or sys.platform == 'cygwin' :
+    WIN32=True
+    HAVE_REMOTE=True
+
+if WIN32:
+    SOCKET = c_uint
+    _lib=CDLL('wpcap.dll')
+else:
+    SOCKET = c_int
+    _lib=CDLL(find_library('pcap'))
+
+
+
+##
+## misc
+##
+u_short = c_ushort
+bpf_int32 = c_int
+u_int = c_uint
+bpf_u_int32 = u_int
+pcap = c_void_p
+pcap_dumper = c_void_p
+u_char = c_ubyte
+FILE = c_void_p
+STRING = c_char_p
+
+class bpf_insn(Structure):
+    _fields_=[("code",c_ushort),
+              ("jt",c_ubyte),
+              ("jf",c_ubyte),
+              ("k",bpf_u_int32)]
+    
+class bpf_program(Structure):
+    pass
+bpf_program._fields_ = [('bf_len', u_int),
+                        ('bf_insns', POINTER(bpf_insn))]
+
+class bpf_version(Structure):
+    _fields_=[("bv_major",c_ushort),
+              ("bv_minor",c_ushort)]
+
+
+class timeval(Structure):
+    pass
+timeval._fields_ = [('tv_sec', c_long),
+                    ('tv_usec', c_long)]
+
+## sockaddr is used by pcap_addr.
+## For exapmle if sa_family==socket.AF_INET then we need cast
+## with sockaddr_in 
+class sockaddr(Structure):
+    _fields_ = [("sa_family",c_ushort),
+                ("sa_data",c_char * 14)]
+##
+## END misc
+##
+
+##
+## Data Structures
+##
+
+## struct  	pcap_file_header
+## 	Header of a libpcap dump file.
+class pcap_file_header(Structure):
+    _fields_ = [('magic', bpf_u_int32),
+                ('version_major', u_short),
+                ('version_minor', u_short),
+                ('thiszone', bpf_int32),
+                ('sigfigs', bpf_u_int32),
+                ('snaplen', bpf_u_int32),
+                ('linktype', bpf_u_int32)]
+
+## struct  	pcap_pkthdr
+## 	Header of a packet in the dump file.
+class pcap_pkthdr(Structure):
+    _fields_ = [('ts', timeval),
+                ('caplen', bpf_u_int32),
+                ('len', bpf_u_int32)]
+
+## struct  	pcap_stat
+## 	Structure that keeps statistical values on an interface.
+class pcap_stat(Structure):
+    pass
+### _fields_ list in Structure is final.
+### We need a temp list
+_tmpList=[]
+_tmpList.append(("ps_recv",c_uint))
+_tmpList.append(("ps_drop",c_uint))
+_tmpList.append(("ps_ifdrop",c_uint))
+if HAVE_REMOTE:
+    _tmpList.append(("ps_capt",c_uint))
+    _tmpList.append(("ps_sent",c_uint))
+    _tmpList.append(("ps_netdrop",c_uint))
+pcap_stat._fields_=_tmpList
+
+## struct  	pcap_addr
+## 	Representation of an interface address, used by pcap_findalldevs().
+class pcap_addr(Structure):
+    pass
+pcap_addr._fields_ = [('next', POINTER(pcap_addr)),
+                      ('addr', POINTER(sockaddr)),
+                      ('netmask', POINTER(sockaddr)),
+                      ('broadaddr', POINTER(sockaddr)),
+                      ('dstaddr', POINTER(sockaddr))]
+
+## struct  	pcap_if
+## 	Item in a list of interfaces, used by pcap_findalldevs().
+class pcap_if(Structure):
+    pass
+pcap_if._fields_ = [('next', POINTER(pcap_if)),
+                    ('name', STRING),
+                    ('description', STRING),
+                    ('addresses', POINTER(pcap_addr)),
+                    ('flags', bpf_u_int32)]
+
+##
+## END Data Structures
+##
+
+##
+## Defines
+##
+
+##define 	PCAP_VERSION_MAJOR   2
+# 	Major libpcap dump file version.
+PCAP_VERSION_MAJOR = 2 
+##define 	PCAP_VERSION_MINOR   4
+# 	Minor libpcap dump file version.
+PCAP_VERSION_MINOR = 4 
+##define 	PCAP_ERRBUF_SIZE   256
+# 	Size to use when allocating the buffer that contains the libpcap errors.
+PCAP_ERRBUF_SIZE = 256 
+##define 	PCAP_IF_LOOPBACK   0x00000001
+# 	interface is loopback
+PCAP_IF_LOOPBACK = 1 
+##define 	MODE_CAPT   0
+# 	Capture mode, to be used when calling pcap_setmode().
+MODE_CAPT = 0
+##define 	MODE_STAT   1
+# 	Statistical mode, to be used when calling pcap_setmode().
+MODE_STAT = 1
+
+##
+## END Defines
+##
+
+##
+## Typedefs
+##
+
+#typedef int 	bpf_int32 (already defined)
+# 	32-bit integer
+#typedef u_int 	bpf_u_int32 (already defined)
+# 	32-bit unsigned integer
+#typedef struct pcap 	pcap_t
+# 	Descriptor of an open capture instance. This structure is opaque to the user, that handles its content through the functions provided by wpcap.dll.
+pcap_t = pcap
+#typedef struct pcap_dumper 	pcap_dumper_t
+# 	libpcap savefile descriptor.
+pcap_dumper_t = pcap_dumper
+#typedef struct pcap_if 	pcap_if_t
+# 	Item in a list of interfaces, see pcap_if.
+pcap_if_t = pcap_if
+#typedef struct pcap_addr 	pcap_addr_t
+# 	Representation of an interface address, see pcap_addr.
+pcap_addr_t = pcap_addr
+
+##
+## END Typedefs
+##
+
+
+
+
+
+# values for enumeration 'pcap_direction_t'
+#pcap_direction_t = c_int # enum
+
+##
+## Unix-compatible Functions
+## These functions are part of the libpcap library, and therefore work both on Windows and on Linux. 
+##
+
+#typedef void(* pcap_handler )(u_char *user, const struct pcap_pkthdr *pkt_header, const u_char *pkt_data)
+# 	Prototype of the callback function that receives the packets.
+## This one is defined from programmer
+pcap_handler=CFUNCTYPE(None,POINTER(c_ubyte),POINTER(pcap_pkthdr),POINTER(c_ubyte))
+
+#pcap_t *   pcap_open_live (const char *device, int snaplen, int promisc, int to_ms, char *ebuf)
+# 	Open a live capture from the network.
+pcap_open_live = _lib.pcap_open_live
+pcap_open_live.restype = POINTER(pcap_t)
+pcap_open_live.argtypes = [STRING, c_int, c_int, c_int, STRING]
+
+#pcap_t *   pcap_open_dead (int linktype, int snaplen)
+# 	Create a pcap_t structure without starting a capture.
+pcap_open_dead = _lib.pcap_open_dead
+pcap_open_dead.restype = POINTER(pcap_t)
+pcap_open_dead.argtypes = [c_int, c_int]
+
+#pcap_t *   pcap_open_offline (const char *fname, char *errbuf)
+# 	Open a savefile in the tcpdump/libpcap format to read packets.
+pcap_open_offline = _lib.pcap_open_offline
+pcap_open_offline.restype = POINTER(pcap_t)
+pcap_open_offline.argtypes = [STRING, STRING]
+
+#pcap_dumper_t *   pcap_dump_open (pcap_t *p, const char *fname)
+# 	Open a file to write packets.
+pcap_dump_open = _lib.pcap_dump_open
+pcap_dump_open.restype = POINTER(pcap_dumper_t)
+pcap_dump_open.argtypes = [POINTER(pcap_t), STRING]
+
+#int pcap_setnonblock (pcap_t *p, int nonblock, char *errbuf)
+# 	Switch between blocking and nonblocking mode.
+pcap_setnonblock = _lib.pcap_setnonblock
+pcap_setnonblock.restype = c_int
+pcap_setnonblock.argtypes = [POINTER(pcap_t), c_int, STRING]
+
+#int pcap_getnonblock (pcap_t *p, char *errbuf)
+# 	Get the "non-blocking" state of an interface.
+pcap_getnonblock = _lib.pcap_getnonblock
+pcap_getnonblock.restype = c_int
+pcap_getnonblock.argtypes = [POINTER(pcap_t), STRING]
+
+#int pcap_findalldevs (pcap_if_t **alldevsp, char *errbuf)
+# 	Construct a list of network devices that can be opened with pcap_open_live().
+pcap_findalldevs = _lib.pcap_findalldevs
+pcap_findalldevs.restype = c_int
+pcap_findalldevs.argtypes = [POINTER(POINTER(pcap_if_t)), STRING]
+
+#void pcap_freealldevs (pcap_if_t *alldevsp)
+# 	Free an interface list returned by pcap_findalldevs().
+pcap_freealldevs = _lib.pcap_freealldevs
+pcap_freealldevs.restype = None
+pcap_freealldevs.argtypes = [POINTER(pcap_if_t)]
+
+#char *   pcap_lookupdev (char *errbuf)
+# 	Return the first valid device in the system.
+pcap_lookupdev = _lib.pcap_lookupdev
+pcap_lookupdev.restype = STRING
+pcap_lookupdev.argtypes = [STRING]
+
+#int pcap_lookupnet (const char *device, bpf_u_int32 *netp, bpf_u_int32 *maskp, char *errbuf)
+# 	Return the subnet and netmask of an interface.
+pcap_lookupnet = _lib.pcap_lookupnet
+pcap_lookupnet.restype = c_int
+pcap_lookupnet.argtypes = [STRING, POINTER(bpf_u_int32), POINTER(bpf_u_int32), STRING]
+
+#int pcap_dispatch (pcap_t *p, int cnt, pcap_handler callback, u_char *user)
+# 	Collect a group of packets.
+pcap_dispatch = _lib.pcap_dispatch
+pcap_dispatch.restype = c_int
+pcap_dispatch.argtypes = [POINTER(pcap_t), c_int, pcap_handler, POINTER(u_char)]
+
+#int pcap_loop (pcap_t *p, int cnt, pcap_handler callback, u_char *user)
+# 	Collect a group of packets.
+pcap_loop = _lib.pcap_loop
+pcap_loop.restype = c_int
+pcap_loop.argtypes = [POINTER(pcap_t), c_int, pcap_handler, POINTER(u_char)]
+
+#u_char *   pcap_next (pcap_t *p, struct pcap_pkthdr *h)
+# 	Return the next available packet.
+pcap_next = _lib.pcap_next
+pcap_next.restype = POINTER(u_char)
+pcap_next.argtypes = [POINTER(pcap_t), POINTER(pcap_pkthdr)]
+
+#int pcap_next_ex (pcap_t *p, struct pcap_pkthdr **pkt_header, const u_char **pkt_data)
+# 	Read a packet from an interface or from an offline capture.
+pcap_next_ex = _lib.pcap_next_ex
+pcap_next_ex.restype = c_int
+pcap_next_ex.argtypes = [POINTER(pcap_t), POINTER(POINTER(pcap_pkthdr)), POINTER(POINTER(u_char))]
+
+#void pcap_breakloop (pcap_t *)
+# 	set a flag that will force pcap_dispatch() or pcap_loop() to return rather than looping.
+pcap_breakloop = _lib.pcap_breakloop
+pcap_breakloop.restype = None
+pcap_breakloop.argtypes = [POINTER(pcap_t)]
+
+#int pcap_sendpacket (pcap_t *p, u_char *buf, int size)
+# 	Send a raw packet.
+pcap_sendpacket = _lib.pcap_sendpacket
+pcap_sendpacket.restype = c_int
+pcap_sendpacket.argtypes = [POINTER(pcap_t), POINTER(u_char), c_int]
+
+#void pcap_dump (u_char *user, const struct pcap_pkthdr *h, const u_char *sp)
+# 	Save a packet to disk.
+pcap_dump = _lib.pcap_dump
+pcap_dump.restype = None
+pcap_dump.argtypes = [POINTER(pcap_dumper_t), POINTER(pcap_pkthdr), POINTER(u_char)]
+
+#long pcap_dump_ftell (pcap_dumper_t *)
+# 	Return the file position for a "savefile".
+pcap_dump_ftell = _lib.pcap_dump_ftell
+pcap_dump_ftell.restype = c_long
+pcap_dump_ftell.argtypes = [POINTER(pcap_dumper_t)]
+
+#int pcap_compile (pcap_t *p, struct bpf_program *fp, char *str, int optimize, bpf_u_int32 netmask)
+# 	Compile a packet filter, converting an high level filtering expression (see Filtering expression syntax) in a program that can be interpreted by the kernel-level filtering engine.
+pcap_compile = _lib.pcap_compile
+pcap_compile.restype = c_int
+pcap_compile.argtypes = [POINTER(pcap_t), POINTER(bpf_program), STRING, c_int, bpf_u_int32]
+
+#int pcap_compile_nopcap (int snaplen_arg, int linktype_arg, struct bpf_program *program, char *buf, int optimize, bpf_u_int32 mask)
+# 	Compile a packet filter without the need of opening an adapter. This function converts an high level filtering expression (see Filtering expression syntax) in a program that can be interpreted by the kernel-level filtering engine.
+pcap_compile_nopcap = _lib.pcap_compile_nopcap
+pcap_compile_nopcap.restype = c_int
+pcap_compile_nopcap.argtypes = [c_int, c_int, POINTER(bpf_program), STRING, c_int, bpf_u_int32]
+
+#int pcap_setfilter (pcap_t *p, struct bpf_program *fp)
+# 	Associate a filter to a capture.
+pcap_setfilter = _lib.pcap_setfilter
+pcap_setfilter.restype = c_int
+pcap_setfilter.argtypes = [POINTER(pcap_t), POINTER(bpf_program)]
+
+#void pcap_freecode (struct bpf_program *fp)
+# 	Free a filter.
+pcap_freecode = _lib.pcap_freecode
+pcap_freecode.restype = None
+pcap_freecode.argtypes = [POINTER(bpf_program)]
+
+#int pcap_datalink (pcap_t *p)
+# 	Return the link layer of an adapter.
+pcap_datalink = _lib.pcap_datalink
+pcap_datalink.restype = c_int
+pcap_datalink.argtypes = [POINTER(pcap_t)]
+
+#int pcap_list_datalinks (pcap_t *p, int **dlt_buf)
+# 	list datalinks
+pcap_list_datalinks = _lib.pcap_list_datalinks
+pcap_list_datalinks.restype = c_int
+#pcap_list_datalinks.argtypes = [POINTER(pcap_t), POINTER(POINTER(c_int))]
+
+#int pcap_set_datalink (pcap_t *p, int dlt)
+# 	Set the current data link type of the pcap descriptor to the type specified by dlt. -1 is returned on failure.
+pcap_set_datalink = _lib.pcap_set_datalink
+pcap_set_datalink.restype = c_int
+pcap_set_datalink.argtypes = [POINTER(pcap_t), c_int]
+
+#int pcap_datalink_name_to_val (const char *name)
+# 	Translates a data link type name, which is a DLT_ name with the DLT_ removed, to the corresponding data link type value. The translation is case-insensitive. -1 is returned on failure.
+pcap_datalink_name_to_val = _lib.pcap_datalink_name_to_val
+pcap_datalink_name_to_val.restype = c_int
+pcap_datalink_name_to_val.argtypes = [STRING]
+
+#const char * 	pcap_datalink_val_to_name (int dlt)
+# 	Translates a data link type value to the corresponding data link type name. NULL is returned on failure.
+pcap_datalink_val_to_name = _lib.pcap_datalink_val_to_name
+pcap_datalink_val_to_name.restype = STRING
+pcap_datalink_val_to_name.argtypes = [c_int]
+
+#const char * 	pcap_datalink_val_to_description (int dlt)
+# 	Translates a data link type value to a short description of that data link type. NULL is returned on failure.
+pcap_datalink_val_to_description = _lib.pcap_datalink_val_to_description
+pcap_datalink_val_to_description.restype = STRING
+pcap_datalink_val_to_description.argtypes = [c_int]
+
+#int pcap_snapshot (pcap_t *p)
+# 	Return the dimension of the packet portion (in bytes) that is delivered to the application.
+pcap_snapshot = _lib.pcap_snapshot
+pcap_snapshot.restype = c_int
+pcap_snapshot.argtypes = [POINTER(pcap_t)]
+
+#int pcap_is_swapped (pcap_t *p)
+# 	returns true if the current savefile uses a different byte order than the current system.
+pcap_is_swapped = _lib.pcap_is_swapped
+pcap_is_swapped.restype = c_int
+pcap_is_swapped.argtypes = [POINTER(pcap_t)]
+
+#int pcap_major_version (pcap_t *p)
+# 	return the major version number of the pcap library used to write the savefile.
+pcap_major_version = _lib.pcap_major_version
+pcap_major_version.restype = c_int
+pcap_major_version.argtypes = [POINTER(pcap_t)]
+
+#int pcap_minor_version (pcap_t *p)
+# 	return the minor version number of the pcap library used to write the savefile.
+pcap_minor_version = _lib.pcap_minor_version
+pcap_minor_version.restype = c_int
+pcap_minor_version.argtypes = [POINTER(pcap_t)]
+
+#FILE *   pcap_file (pcap_t *p)
+# 	Return the standard stream of an offline capture.
+pcap_file=_lib.pcap_file
+pcap_file.restype = FILE
+pcap_file.argtypes = [POINTER(pcap_t)]
+
+#int pcap_stats (pcap_t *p, struct pcap_stat *ps)
+# 	Return statistics on current capture.
+pcap_stats = _lib.pcap_stats
+pcap_stats.restype = c_int
+pcap_stats.argtypes = [POINTER(pcap_t), POINTER(pcap_stat)]
+
+#void pcap_perror (pcap_t *p, char *prefix)
+# 	print the text of the last pcap library error on stderr, prefixed by prefix.
+pcap_perror = _lib.pcap_perror
+pcap_perror.restype = None
+pcap_perror.argtypes = [POINTER(pcap_t), STRING]
+
+#char *   pcap_geterr (pcap_t *p)
+# 	return the error text pertaining to the last pcap library error.
+pcap_geterr = _lib.pcap_geterr
+pcap_geterr.restype = STRING
+pcap_geterr.argtypes = [POINTER(pcap_t)]
+
+#char *   pcap_strerror (int error)
+# 	Provided in case strerror() isn't available.
+pcap_strerror = _lib.pcap_strerror
+pcap_strerror.restype = STRING
+pcap_strerror.argtypes = [c_int]
+
+#const char *   pcap_lib_version (void)
+# 	Returns a pointer to a string giving information about the version of the libpcap library being used; note that it contains more information than just a version number.
+pcap_lib_version = _lib.pcap_lib_version
+pcap_lib_version.restype = STRING
+pcap_lib_version.argtypes = []
+
+#void pcap_close (pcap_t *p)
+# 	close the files associated with p and deallocates resources.
+pcap_close = _lib.pcap_close
+pcap_close.restype = None
+pcap_close.argtypes = [POINTER(pcap_t)]
+
+#FILE *   pcap_dump_file (pcap_dumper_t *p)
+# 	return the standard I/O stream of the 'savefile' opened by pcap_dump_open().
+pcap_dump_file=_lib.pcap_dump_file
+pcap_dump_file.restype=FILE
+pcap_dump_file.argtypes= [POINTER(pcap_dumper_t)]
+
+#int pcap_dump_flush (pcap_dumper_t *p)
+# 	Flushes the output buffer to the ``savefile,'' so that any packets written with pcap_dump() but not yet written to the ``savefile'' will be written. -1 is returned on error, 0 on success.
+pcap_dump_flush = _lib.pcap_dump_flush
+pcap_dump_flush.restype = c_int
+pcap_dump_flush.argtypes = [POINTER(pcap_dumper_t)]
+
+#void pcap_dump_close (pcap_dumper_t *p)
+# 	Closes a savefile. 
+pcap_dump_close = _lib.pcap_dump_close
+pcap_dump_close.restype = None
+pcap_dump_close.argtypes = [POINTER(pcap_dumper_t)]
+
+###########################################
+## Windows-specific Extensions
+## The functions in this section extend libpcap to offer advanced functionalities
+## (like remote packet capture, packet buffer size variation or high-precision packet injection).
+## Howerver, at the moment they can be used only in Windows.
+###########################################
+if WIN32:
+    HANDLE = c_void_p
+    
+    ##############
+    ## Identifiers related to the new source syntax
+    ##############
+    #define 	PCAP_SRC_FILE   2
+    #define 	PCAP_SRC_IFLOCAL   3
+    #define 	PCAP_SRC_IFREMOTE   4
+    #Internal representation of the type of source in use (file, remote/local interface).
+    PCAP_SRC_FILE = 2
+    PCAP_SRC_IFLOCAL = 3
+    PCAP_SRC_IFREMOTE = 4
+    
+    ##############
+    ## Strings related to the new source syntax
+    ##############
+    #define 	PCAP_SRC_FILE_STRING   "file://"
+    #define 	PCAP_SRC_IF_STRING   "rpcap://"
+    #String that will be used to determine the type of source in use (file, remote/local interface).
+    PCAP_SRC_FILE_STRING="file://"
+    PCAP_SRC_IF_STRING="rpcap://"
+    
+    ##############
+    ## Flags defined in the pcap_open() function
+    ##############
+    # define 	PCAP_OPENFLAG_PROMISCUOUS   1
+    # 	Defines if the adapter has to go in promiscuous mode.
+    PCAP_OPENFLAG_PROMISCUOUS=1
+    # define 	PCAP_OPENFLAG_DATATX_UDP   2
+    # 	Defines if the data trasfer (in case of a remote capture) has to be done with UDP protocol.
+    PCAP_OPENFLAG_DATATX_UDP=2
+    # define 	PCAP_OPENFLAG_NOCAPTURE_RPCAP   4
+    PCAP_OPENFLAG_NOCAPTURE_RPCAP=4
+    # 	Defines if the remote probe will capture its own generated traffic.
+    # define 	PCAP_OPENFLAG_NOCAPTURE_LOCAL   8
+    PCAP_OPENFLAG_NOCAPTURE_LOCAL = 8
+    # define 	PCAP_OPENFLAG_MAX_RESPONSIVENESS   16
+    # 	This flag configures the adapter for maximum responsiveness.
+    PCAP_OPENFLAG_MAX_RESPONSIVENESS=16
+    
+    ##############
+    ## Sampling methods defined in the pcap_setsampling() function
+    ##############
+    # define 	PCAP_SAMP_NOSAMP   0
+    # No sampling has to be done on the current capture.
+    PCAP_SAMP_NOSAMP=0
+    # define 	PCAP_SAMP_1_EVERY_N   1
+    # It defines that only 1 out of N packets must be returned to the user.
+    PCAP_SAMP_1_EVERY_N=1
+    #define 	PCAP_SAMP_FIRST_AFTER_N_MS   2
+    # It defines that we have to return 1 packet every N milliseconds.
+    PCAP_SAMP_FIRST_AFTER_N_MS=2
+    
+    ##############
+    ## Authentication methods supported by the RPCAP protocol
+    ##############
+    # define 	RPCAP_RMTAUTH_NULL   0
+    # It defines the NULL authentication.
+    RPCAP_RMTAUTH_NULL=0
+    # define 	RPCAP_RMTAUTH_PWD   1
+    # It defines the username/password authentication.
+    RPCAP_RMTAUTH_PWD=1
+    
+
+    ##############
+    ## Remote struct and defines
+    ##############
+    # define 	PCAP_BUF_SIZE   1024
+    # Defines the maximum buffer size in which address, port, interface names are kept.
+    PCAP_BUF_SIZE = 1024
+    # define 	RPCAP_HOSTLIST_SIZE   1024
+    # Maximum lenght of an host name (needed for the RPCAP active mode).
+    RPCAP_HOSTLIST_SIZE = 1024
+    
+    class pcap_send_queue(Structure):
+        _fields_=[("maxlen",c_uint),
+                  ("len",c_uint),
+                  ("buffer",c_char_p)]
+        
+    ## struct  	pcap_rmtauth
+    ## This structure keeps the information needed to autheticate the user on a remote machine
+    class pcap_rmtauth(Structure):
+        _fields_=[("type",c_int),
+                  ("username",c_char_p),
+                  ("password",c_char_p)]
+    
+    ## struct  	pcap_samp
+    ## This structure defines the information related to sampling    
+    class pcap_samp(Structure):
+        _fields_=[("method",c_int),
+                  ("value",c_int)]
+
+    #PAirpcapHandle 	pcap_get_airpcap_handle (pcap_t *p)
+    # 	Returns the AirPcap handler associated with an adapter. This handler can be used to change the wireless-related settings of the CACE Technologies AirPcap wireless capture adapters.
+    
+    #bool pcap_offline_filter (struct bpf_program *prog, const struct pcap_pkthdr *header, const u_char *pkt_data)
+    # 	Returns if a given filter applies to an offline packet.
+    pcap_offline_filter = _lib.pcap_offline_filter
+    pcap_offline_filter.restype = c_bool
+    pcap_offline_filter.argtypes = [POINTER(bpf_program),POINTER(pcap_pkthdr),POINTER(u_char)]
+    
+    #int pcap_live_dump (pcap_t *p, char *filename, int maxsize, int maxpacks)
+    # 	Save a capture to file.
+    pcap_live_dump = _lib.pcap_live_dump
+    pcap_live_dump.restype = c_int
+    pcap_live_dump.argtypes = [POINTER(pcap_t), POINTER(c_char), c_int,c_int]
+    
+    #int pcap_live_dump_ended (pcap_t *p, int sync)
+    # 	Return the status of the kernel dump process, i.e. tells if one of the limits defined with pcap_live_dump() has been reached.
+    pcap_live_dump_ended = _lib.pcap_live_dump_ended
+    pcap_live_dump_ended.restype = c_int
+    pcap_live_dump_ended.argtypes = [POINTER(pcap_t), c_int]
+    
+    #struct pcap_stat *  pcap_stats_ex (pcap_t *p, int *pcap_stat_size)
+    # 	Return statistics on current capture.
+    pcap_stats_ex = _lib.pcap_stats_ex
+    pcap_stats_ex.restype = POINTER(pcap_stat)
+    pcap_stats_ex.argtypes = [POINTER(pcap_t), POINTER(c_int)]
+    
+    #int pcap_setbuff (pcap_t *p, int dim)
+    # 	Set the size of the kernel buffer associated with an adapter.
+    pcap_setbuff = _lib.pcap_setbuff
+    pcap_setbuff.restype = c_int
+    pcap_setbuff.argtypes = [POINTER(pcap_t), c_int]
+    
+    #int pcap_setmode (pcap_t *p, int mode)
+    # 	Set the working mode of the interface p to mode.
+    pcap_setmode = _lib.pcap_setmode
+    pcap_setmode.restype = c_int
+    pcap_setmode.argtypes = [POINTER(pcap_t), c_int]
+    
+    #int pcap_setmintocopy (pcap_t *p, int size)
+    # 	Set the minumum amount of data received by the kernel in a single call.
+    pcap_setmintocopy = _lib.pcap_setmintocopy
+    pcap_setmintocopy.restype = c_int
+    pcap_setmintocopy.argtype = [POINTER(pcap_t), c_int]
+    
+    #HANDLE pcap_getevent (pcap_t *p)
+    # 	Return the handle of the event associated with the interface p.
+    pcap_getevent = _lib.pcap_getevent
+    pcap_getevent.restype = HANDLE
+    pcap_getevent.argtypes = [POINTER(pcap_t)]
+
+    #pcap_send_queue * 	pcap_sendqueue_alloc (u_int memsize)
+    # 	Allocate a send queue.
+    pcap_sendqueue_alloc = _lib.pcap_sendqueue_alloc
+    pcap_sendqueue_alloc.restype = POINTER(pcap_send_queue)
+    pcap_sendqueue_alloc.argtypes = [c_uint]
+    
+    #void pcap_sendqueue_destroy (pcap_send_queue *queue)
+    # 	Destroy a send queue.
+    pcap_sendqueue_destroy = _lib.pcap_sendqueue_destroy
+    pcap_sendqueue_destroy.restype = None
+    pcap_sendqueue_destroy.argtypes = [POINTER(pcap_send_queue)]
+    
+    #int pcap_sendqueue_queue (pcap_send_queue *queue, const struct pcap_pkthdr *pkt_header, const u_char *pkt_data)
+    # 	Add a packet to a send queue.
+    pcap_sendqueue_queue = _lib.pcap_sendqueue_queue
+    pcap_sendqueue_queue.restype = c_int
+    pcap_sendqueue_queue.argtypes = [POINTER(pcap_send_queue), POINTER(pcap_pkthdr), POINTER(u_char)]
+    
+    #u_int pcap_sendqueue_transmit (pcap_t *p, pcap_send_queue *queue, int sync)
+    # 	Send a queue of raw packets to the network.
+    pcap_sendqueue_transmit = _lib.pcap_sendqueue_transmit
+    pcap_sendqueue_transmit.retype = u_int
+    pcap_sendqueue_transmit.argtypes = [POINTER(pcap_t), POINTER(pcap_send_queue), c_int]
+    
+    #int pcap_findalldevs_ex (char *source, struct pcap_rmtauth *auth, pcap_if_t **alldevs, char *errbuf)
+    # 	Create a list of network devices that can be opened with pcap_open().
+    pcap_findalldevs_ex = _lib.pcap_findalldevs_ex
+    pcap_findalldevs_ex.retype = c_int
+    pcap_findalldevs_ex.argtypes = [STRING, POINTER(pcap_rmtauth), POINTER(POINTER(pcap_if_t)), STRING]
+    
+    #int pcap_createsrcstr (char *source, int type, const char *host, const char *port, const char *name, char *errbuf)
+    # 	Accept a set of strings (host name, port, ...), and it returns the complete source string according to the new format (e.g. 'rpcap://1.2.3.4/eth0').
+    pcap_createsrcstr = _lib.pcap_createsrcstr
+    pcap_createsrcstr.restype = c_int
+    pcap_createsrcstr.argtypes = [STRING, c_int, STRING, STRING, STRING, STRING]
+    
+    #int pcap_parsesrcstr (const char *source, int *type, char *host, char *port, char *name, char *errbuf)
+    # 	Parse the source string and returns the pieces in which the source can be split.
+    pcap_parsesrcstr = _lib.pcap_parsesrcstr
+    pcap_parsesrcstr.retype = c_int
+    pcap_parsesrcstr.argtypes = [STRING, POINTER(c_int), STRING, STRING, STRING, STRING]
+    
+    #pcap_t * 	pcap_open (const char *source, int snaplen, int flags, int read_timeout, struct pcap_rmtauth *auth, char *errbuf)
+    # 	Open a generic source in order to capture / send (WinPcap only) traffic.
+    pcap_open = _lib.pcap_open
+    pcap_open.restype = POINTER(pcap_t)
+    pcap_open.argtypes = [STRING, c_int, c_int, c_int, POINTER(pcap_rmtauth), STRING]
+    
+    #struct pcap_samp *  pcap_setsampling (pcap_t *p)
+    # 	Define a sampling method for packet capture.
+    pcap_setsampling = _lib.pcap_setsampling
+    pcap_setsampling.restype = POINTER(pcap_samp)
+    pcap_setsampling.argtypes = [POINTER(pcap_t)]
+    
+    #SOCKET pcap_remoteact_accept (const char *address, const char *port, const char *hostlist, char *connectinghost, struct pcap_rmtauth *auth, char *errbuf)
+    # 	Block until a network connection is accepted (active mode only).
+    pcap_remoteact_accept = _lib.pcap_remoteact_accept
+    pcap_remoteact_accept.restype = SOCKET
+    pcap_remoteact_accept.argtypes = [STRING, STRING, STRING, STRING, POINTER(pcap_rmtauth), STRING]
+    
+    #int pcap_remoteact_close (const char *host, char *errbuf)
+    # 	Drop an active connection (active mode only).
+    pcap_remoteact_close = _lib.pcap_remoteact_close
+    pcap_remoteact_close.restypes = c_int
+    pcap_remoteact_close.argtypes = [STRING, STRING]
+    
+    #void pcap_remoteact_cleanup ()
+    # 	Clean the socket that is currently used in waiting active connections.
+    pcap_remoteact_cleanup = _lib.pcap_remoteact_cleanup
+    pcap_remoteact_cleanup.restypes = None
+    pcap_remoteact_cleanup.argtypes = []
+    
+    #int pcap_remoteact_list (char *hostlist, char sep, int size, char *errbuf)
+    # 	Return the hostname of the host that have an active connection with us (active mode only). 
+    pcap_remoteact_list = _lib.pcap_remoteact_list
+    pcap_remoteact_list.restype = c_int
+    pcap_remoteact_list.argtypes = [STRING, c_char, c_int, STRING]
+
```

