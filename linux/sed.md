### remove comments from powershell script
```
sed '/<#/,/#>/d' <file>.ps1
```

### delete lines containing string
```
sed '/string/d' <file>
```

### add string to each line
```
sed 's/$/<string>/g' <file>
```

### print lines between 2 patterns
```
sed -n '/<pattern1>/,/<pattern2>/p' <file>
```

### print only words longer than 3 chars
```
sed -r '/^.{,3}$/d' <file>
```

### remove leading chars
```
echo "00123" | sed 's/^0*//'
```
