### download file
```
certutil -urlcache -split -f http://<rhost>/<file>
```

### decode base64 file
```
certutil -decode <base64File> <decodedFile>
```

### get CA host
```
certutil -TCAInfo
```
