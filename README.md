# windows-terminal-commands-in-use
### Search
  tip: "" works,'' doesn't work
  
  filtering .py files and display
  
    dir | find ".py"
  
  file with specific extension or name
  
    dir /b/s *.txt
    dir /b/s *idf*
    
  check if a folder named "tmp" exists
  
    dir tmp /AD /s
    
  display line numbers of a file
  
    type config.py | find "" /v /c
  
  filtering tasks named "chrome"
  
    tasklist | find "chrome"
    
  recursive content search 
    
    for /r %a in (\*.*) do find "search_text" %a
    for /f %G in ('dir *.cpp *.h /s/b') do  ( find /i "what you search"  "%G") >> out_file.txt
    findstr /spin /c:"string" [files]
    
### Clean

  remove files with extension named 'pyd'
  
    del /Q /S *.pyd

  remove dir called 'dist' and delete all files in it
  
    rmdir /Q /S dist
    
### Copy

  Copy a file:

    echo F| XCOPY C:\utils\MyFile.txt D:\Backup\CopyFile.txt

  Copy a folder:

    XCOPY C:\utils D:\Backup\utils /i

  Copy a folder including all subfolders.

    XCOPY C:\utils\* D:\Backup\utils /s /i
    
### Loop

   Loop through several strings
   
    FOR %G IN (extract split fillin merge) DO (
      pyinstaller --nowindow %G.py
      pyinstaller %G.spec)
    
  
### Comment

   Single-Line Comment
    
    rem pyinstaller extract.spec
   
### Set Variable

   Set
   
    set target="split"
    echo %target%
