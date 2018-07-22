# 增强右键菜单

## 以管理员权限运行CMD

按住shift再单击右键会出现。

```text
Windows Registry Editor Version 5.00

; Created by: Shawn Brink
; http://www.sevenforums.com
; Tutorial: http://www.sevenforums.com/tutorials/47415-open-command-window-here-administrator.html
 
[-HKEY_CLASSES_ROOT\Directory\shell\runas]

[HKEY_CLASSES_ROOT\Directory\shell\runas]
@="Open CMD as Admin"
"Extended"=""
"HasLUAShield"=""

[HKEY_CLASSES_ROOT\Directory\shell\runas\command]
@="cmd.exe /s /k pushd \"%V\""

[-HKEY_CLASSES_ROOT\Directory\Background\shell\runas]

[HKEY_CLASSES_ROOT\Directory\Background\shell\runas]
@="Open CMD as Admin"
"Extended"=""
"HasLUAShield"=""

[HKEY_CLASSES_ROOT\Directory\Background\shell\runas\command]
@="cmd.exe /s /k pushd \"%V\""

[-HKEY_CLASSES_ROOT\Drive\shell\runas]

[HKEY_CLASSES_ROOT\Drive\shell\runas]
@="Open CMD as Admin"
"Extended"=""
"HasLUAShield"=""

[HKEY_CLASSES_ROOT\Drive\shell\runas\command]
@="cmd.exe /s /k pushd \"%V\""

[-HKEY_CLASSES_ROOT\LibraryFolder\background\shell\runas]

[HKEY_CLASSES_ROOT\LibraryFolder\background\shell\runas]
"Extended"=""
"HasLUAShield"=""
@="Open CMD as Admin"

[HKEY_CLASSES_ROOT\LibraryFolder\background\shell\runas\command]
@="cmd.exe /s /k pushd \"%V\""
```

## 在WinRAR中打开

按住shift，右键单击文件夹空白处，即会出现此选项。

```text
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Directory\shell\在winrar中打开]
@="在winrar中打开"
"Extended"=""

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Directory\shell\在winrar中打开\command]
@=hex(2):77,00,69,00,6e,00,72,00,61,00,72,00,2e,00,65,00,78,00,65,00,20,00,22,\
  00,25,00,31,00,22,00,00,00

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Directory\Background\shell\在winrar中打开]
@="在winrar中打开"
"Extended"=""

[HKEY_LOCAL_MACHINE\SOFTWARE\Classes\Directory\Background\shell\在winrar中打开\command]
@=hex(2):77,00,69,00,6e,00,72,00,61,00,72,00,2e,00,65,00,78,00,65,00,20,00,22,\
  00,25,00,56,00,22,00,00,00
```

