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
