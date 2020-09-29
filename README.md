# godepnotworking
A solve to "godep command not found" error


```bash
export GOPATH=$HOME/go

export PATH=$GOPATH/bin:$PATH

godep save ./..
```

If godep gives you the error ,for example
> godep: Package (github.com/boombuler/barcode) not found

while running *godep save ./...* ,head outside the $GOPATH,run *go get <package-name>* and then head over the project directory in the $GOPATH and run *godep save ./...* for it will work now.
