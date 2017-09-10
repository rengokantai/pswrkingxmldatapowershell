# pswrkingxmldatapowershell

## 3. Exporting Information to XML
```
Get-Process | Export-Clixml C:\file.xml
```


Convert to xml
```
(Get-ChildItem C:\folder | ConvertTo-XML).Save("C:\test.xml")
```


#### 06:27
```
(Get-ChildItem C:\folder | ConvertTo-XML -NoTypeInformation).Save("C:\test.xml")
```


### 4. Real Life Examples
```
$hostname = $env:computername
$IPAddress = Get-NetIPAddress | Select IPAddress, AddressFamily
$Path = "C:\in.xml"
```

```
Get-Process | Export-Clixml proc.xml
$Process = Import-Clixml proc.xml
```
