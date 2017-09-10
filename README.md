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
