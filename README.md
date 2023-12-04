# HTTPServerWithUpload
Python3 HTTP Server with upload functionality

**Run server:**

```
python3 HTTPServerWithUpload.py 80
```

**Upload file:**

* curl:

```bash
curl -X POST http://server.com/ -H "Content-Type: multipart/form-data" -F file=@"file.zip"
```

* powershell:

```powershell
$wc=New-Object System.Net.WebClient; $resp=$wc.UploadFile('http://server.com',"C:\file.zip")
```