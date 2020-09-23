<div align="center">

## Minimize all open windows


</div>

### Description

This code will minimize all open windows
 
### More Info
 
None known


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Neil Baker](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/neil-baker.md)
**Level**          |Beginner
**User Rating**    |4.3 (13 globes from 3 users)
**Compatibility**  |Delphi 7
**Category**       |[Windows API Call/ Explanation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/windows-api-call-explanation__7-39.md)
**World**          |[Delphi](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/delphi.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/neil-baker-minimize-all-open-windows__7-972/archive/master.zip)





### Source Code

```
// to minimize all open windows
var
  intHwnd: Integer;
begin
  intHwnd := FindWindow('Shell_TrayWnd', nil);
  PostMessage(intHwnd, WM_COMMAND, 419, 0);
end;
// end
// You can change 419 with 416 to restore the window, I know its not much but I hope it helps :)
```

