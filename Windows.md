### [Side-By-Side Configuration Is Incorrect!](https://www.codeproject.com/Articles/43681/Side-by-Side-Configuration-Incorrect)

      $ sfc/scannow
      $ DISM.exe /Online /Cleanup-image /Scanhealth
      $ DISM.exe /Online /Cleanup-image /Restorehealth
      
      For running sxstrace.exe, go to Visual Studio command prompt and type sxstrace.exe. Usage is as follows:
      1.Before running your application, run sxstrace in trace mode
      $ sxstrace.exe Trace -logfile:C:\tmp\MySxSTrace.log
      2.Reproduce the error by starting your application
      3.Now stop the trace by using the below command 
      $ sxstrace.exe Parse -logfile:C:\tmp\MySxSTrace.log -outfile:C:\tmp\MySxSTrace.txt
      4.Open output file from C:\tmp\MySxSTrace.txt

### dd