create a working folder with vbscript 
=======
Const ForReading = 1, ForWriting = 2
  Set WshShell = WScript.CreateObject("WScript.Shell")
   Dim fso, f
   	Set fso = CreateObject("Scripting.FileSystemObject")
    Set fs = CreateObject("Scripting.FileSystemObject" ) 
	fs.CreateFolder ("path" )
	fs.CreateFolder ("path/css" )
	Set f = fso.OpenTextFile("path/css/style.css", ForWriting,true)
	fs.CreateFolder ("path/js" )
	Set f = fso.OpenTextFile("pathjquiry.js", ForWriting,true)
	fs.CreateFolder ("path/images" )
	Set f = fso.OpenTextFile("path/index.html", ForWriting,true)
   	f.writeline("<!DOCTYPE HTML>")
   	f.writeline("<html>")
   	f.writeline("<head>")
   	f.writeline("<meta charset='utf-8'>")
   	f.writeline("<title>Motivation website</title")
   	f.writeline("<link rel='stylesheet' type='text/css' href='style/style.css'>")
   	f.writeline("</head>")
   	f.writeline("<body></body>")
   	f.writeline("</html> ")
