FInf
FIle (I)NFo 

An open source file extension and Shebang database

Support:
.fileextension
SpecialFile
File System
Shebang/Hashpling

Specialized content format (written in Pug, alternative versions will exist in XML, Mustache, and Handlebars, HTML, and CSS/Less will always be present)

Fun fact: I was actually looking into making a file info site. It wasn't until the portmanteau FINF came to me while writing Pug source code in ShareBoxLIB that I realized the potential of this idea, and also had a good name

// Start of script
extends ../_bootstrap
append styles
block FINFMain
	block FINFHome
		h1.finfhomeTitle Welcome to FINF
		h2.finfhomeSubtitle A powerful open source file extension and !#Shebang/Hashpling database
		li.navbar1Title Navigation
	block FINFHome end
	block FINFDB
		block getExtension
			// Some examples
			// Note: names are cAsE SeNsItIvE
			// This system is very verbose, but it is necessary. There are hundreds of thousands of file extensions (possibly millions) and I have to fit this into a 1000 folder/1000 item system
			// The /./ folder is used to differentiate between a file extension, and a unique file (such as MAKEFILE, CREDITS, etc.)
			fileExt.txt @/DB/File/./t/x/t/aboutfile-en.txt.htm
			fileExt.pas @/DB/File/./p/a/s/aboutfile-en.pas.htm
			fileExt.TXT @/DB/File/./T/X/T/aboutfile-en.TXT.htm
			fileExt.PAS @/DB/File/./P/A/S/aboutfile-en.PAS.htm
			fileExt.SPECIAL.MAKEFILE @/DB/File/M/A/K/E/F/I/L/E/aboutfile-en_Special_MAKEFILE.htm
			fileExt.SPECIAL.CREDITS @/DB/File/C/R/E/D/I/T/S/aboutfile-en_Special_CREDITS.htm
			fileExt.SPECIAL.makefile @/DB/File/m/a/k/e/f/i/l/e/aboutfile-en_Special_makefile.htm
			fileExt.SPECIAL.credits @/DB/File/c/r/e/d/i/t/s/aboutfile-en_Special_credits.htm
		block getExtension end
		block getBang
			// Some examples
			hpling.shell_1 @/DB/PlingBang/#/!/b/i/n/s/h/SHELL_IDENTIFIER.htm
			hpling.python_1 @/DB/PlingBang/#/!/u/s/r/b/i/n/e/n/v/p/y/t/h/o/n/PYTHON_IDENTIFIER.htm
		block getBang end
	block FINFDB end
block FINFMain end
// Pug, XML, Mustache, and Handlebars will be used for keeping entries (depending on which you prefer) HTML will be used for the actual entries. CSS/Less will just be the stylesheet
/* Example entry

<!-- Start of script !-->
<!DOCTYPE html>
<HTML>
<HEAD>
<meta>
	<meta charset="UTF-16">
</meta>
<TITLE>*.txt - FINF File Info DB</TITLE>
<BODY lang="en">
<HR>
<H6><a href="aboutfile-en.txt.htm">English</a> <a href="aboutfile-eo.txt.htm">Esperanto</a></H6>
<H5>You are viewing this page in Basic HTML view <a href="?href=ABOUT-NIL">[Switch to a different view]</a></H5>
<H1>.txt</H1>
<H4 lang="en">Not to be confused with <a href="/DB/T/X/T/aboutfile.TXT.htm">.TXT</a></H4> <!-- The linked entry will be mostly a duplicate, with a small exception of explaining the difference !-->
<HR>
<p lang="en">.txt is a very common file extension. It is a plain text file. It is not associated with any programs, and can be used on any operating system.</p>
<details><summary><p lang="en">Click/tap here to expand/collapse this section</p></summary>
<p lang="en">Operating system: Any (MS-DOS, DR-DOS, Windows, Windows 9x, Windows NT, Linux, GNU/Linux, Classic MacOS, MacOS, MacOS X, OS X, iOS, Android, ChromiumOS, ChromeOS, OS/2, Solaris, FreeBSD, NetBSD, OpenBSD, DragonflyBSD, etc.)</p>
</details>
<HR>
<details><summary><p>Click/tap here to expand/collapse this section</p></summary>
<p lang="en">Opens with: Gedit, Notepad++ (GNU/Linux) Notepad, Notepad++ (Windows) ???, Notepad++ (MacOS) ???, Notepad++ (BSD) HTML Viewer (Android) ??? (iOS/iPadOS/iPhoneOS) ??? (OS/2) ??? (MS-DOS) ??? (DR-DOS) ??? (Solaris) etc.</p>
</details>
<HR>
<p lang="en">Shebang? Typically none, none required</p>
<p lang="en">Encoding: Any</p>
<p lang="en">File icon</p>
<HR>
<details><summary><p>Click/tap here to expand/collapse this section</p></summary>
<p lang="en">GNOME: <img src="TXT_GNOME.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">KDE: <img src="TXT_KDE.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">XFCE: <img src="TXT_XFCE.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">LXQT: <img src="TXT_LXQT.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">CINNAMON: <img src="TXT_CINNAMON.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">Common Desktop Environment (CDE): <img src="TXT_CDE.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">MacOS (Classic): <img src="TXT_MACOS_CLASSIC.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">MacOS (Mac OS X): <img src="TXT_MACOS_X.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">MacOS (OS X): <img src="TXT_OSX.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">MacOS (MacOS 10.10-10.12): <img src="TXT_MACOS1010.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">MacOS (Modern, pre-MacOS11): <img src="TXT_MACOS1013.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">MacOS (Modern, MacOS11): <img src="TXT_MACOS110.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">WinRAR: <img src="TXT_WINRAR.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">Android: <img src="TXT_ANDROID.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">iOS: <img src="TXT_IOS.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">Windows (DOS): <img src="TXT_WINDOWSDOS.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">Windows (9x): <img src="TXT_WINDOWS9X.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">Windows (NT): <img src="TXT_WINDOWSNT.svg" alt="File not found" width="128" height="128"></p>
<p lang="en">Solaris: <img src="TXT_SOLARIS.svg" alt="File not found" width="128" height="128"></p>
</details>
<HR>
</BODY>
</HTML>
<!-- End of script !-->

*/
/* Starter entries
cyc, exe, pug, txt, TXT, pas, C, cpp, cc, c, mkv, mp4, ogg, md, mkd, markdown, mdown, mak, mk, git, e, py, dl, dll, asm, as, rs, p, P, qml, qt, msi, dmg, img, png, jpg, svg, gif, gifv, gif_c200, rtf, uot, odt, doc, docx, ods, ott, dot, dotx, xml, xul, cs, csx, vhdl, vhd, vdi, wmv, webm, webp, kix, sh, bat, BAT, vi, vim, xhtml, html, xhtm, htm, mhtml, mhtm, swf, fla, psd, pdf, zig, zir, yaml, yml, h, ts, ss, scm, el, l, ll, m, mm, swift, go, ml, tar, zip, 7z, rar, raku, pl, pro, r, wasm, wat, fs, ipa, java, js, jar, lua, nim, oga, mov, scala, sql, vbs, vba, v, d, dat, DAT, bin, BIN, vala, vapi, tar, xz, tar.xz, deb, rpm, sb2, sb3, sb, sb1, ps, ps1, rom, sms, n64, cia, lsp, cxx, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, sqlite, torrent, rdf, rss, rpc, m4, mp3, mp2, mid, flac, alac, m4a, dib, bmp, tif, tiff, jfif, jif, jp2, hs, hdl, vbox, DS_STORE, pkg, apk, iso, lo, po, Po, pot, potx, pptx, ppt, accdb, xlsx, xls, xls, msg, rb, url, ink, json, scss, sty, tex, texshop, srt, ogv, o, woff, ttf, ttf2, sit, hqx, cfg, rtl, rst, avi, for, f99, FOR, F99, F95, f95, wim, j, less, jade, bib, toc, TOC, erl, hrl, image, tcl, key, yacc, build, BUILD, gs, qs, config, CONFIG, nt, cmd, mod, vl, sys, litcoffee, coffee, ada, alg, BAS, ALG, boo, hack, csd, diff, git
Just to name a few
*/
/* Navigation
This project is very difficult to navigate by hand. For search functions, it is recommended to search for the file with the string `aboutfile.` followed by the file you are looking for. It would be far too tedious to do it through a directory by directory search. A list should also be kept and ALWAYS updated.
*/
block fileInf
  h1.finfTitle File info
  p.finfBody1 File type: Pug source file (*.pug)
  p.finfBody2 File version: 1 (2021, Sunday, November 28th at 4:19 pm)
  p.finfBody3 Line count (including blank lines and compiler line): 119
block endFinf
// End of script
