# Virustotal_API

### Resume :

Script for scanning suspicious file from your terminal using VirusTotal public API

### Requirements :

```
Python >= 3.3
argparse
requests
```

Dependencies can be installed via PIP or a package manager

To install all dependencies with PIP :

```
pip3 install -r requirements.txt --upgrade --user
```

### Add your VirusTotal API key :

The command below adds your API key in the Python script :

```
echo 'YOUR API KEY' | xargs -I {} sed -i "s/''/'{}'/" vt
```

### Usage :

Scan a file by sending **only** its hash to VirusTotal :

```
vt YOUR_FILE
```

Scan a file and **send your file** to VirusTotal :

```
vt --scan YOUR_FILE
```

To return the full VirusTotal report :

```
vt --verbose YOUR_FILE
```

### Licence :

This project is licensed under the terms of the GLPv3
