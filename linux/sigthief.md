### source
https://raw.githubusercontent.com/secretsquirrel/SigThief/master/sigthief.py  

### take a Signature from a binary and add it to another binary
```
python3 sigthief.py -i <originalFile>.exe -t <targetFile>.exe -o <outFile>
```

### save Signature to disk for later use
```
python3 sigthief.py -i <originalFile>.exe -r
```

### use saved signature
```
python3 sigthief.py -s <signatureFile>.exe -t <targetFile>.exe
```

### check if file has a signature (does not check validity)
```
python3 sigthief.py -i <originalFile>.exe -c
```
