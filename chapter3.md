## Chapter3

### 帮助
1. `update-help`命令用于下载（首次）和更新`PowerShell`的帮助文件
2. 使用`Get-Help(或者help，man) <cmdlet-name>`可以查看这个`cmdlet`的帮助文件
3. 查看完整模式的帮助文件：`help <cmdlet-name> -full`
4. 查看帮助文件的实例：`help <cmdlet-name> -examples`

### 参数
1. 参数分为可选参数和必选参数
    1. 可选参数：`[-ComputerName <String[]>]`，`—ComputerName`是参数名，`<String[]>`是参数值。参数名和参数值在一个方括号里表明整个参数是可选的，而且如果参数名如果再用一个方括号包裹起来，表明参数名是一个定位参数，意思是参数名占住这个位置，可以不输入参数名而直接输入参数值，但是考虑到可能会发生输入的的失误，建议坚持使用参数名。
    2. 必选参数：`[-LogName] <String>`, `[-LogName]`是参数名，`<String>`是参数值，同时`[-LogName]`也是定位参数，可以省略不输入，直接输入参数值

### 动词-名词
1. `Cmdlet-Name`多半采用动词-名词的方式，比如：
``` powershell
    Get-Process
    New-Service
```

