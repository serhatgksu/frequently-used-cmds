# windows-terminal-commands-in-use
### Search
  tip: "" works,'' doesn't work
  
  filtering .py files and display
  
    dir | find ".py"
  
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
  
