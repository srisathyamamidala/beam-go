# beam-go

#### All the commands should run using Powershell run as administrator.

The Beam SDK for Go requires go version **1.16 or newer**. It can be downloaded [here](https://go.dev/). Check that you have version 1.16 by running:

```
go version
```

Once you've double-checked that you have the latest **version** of Go

```
go mod init github.com/srisathyamamidala/beam-go
```

To open **VS Code** in your local environment,type in the powershell the following command: 
```
code .
```

Create the sample [hello.go](https://raw.githubusercontent.com/srisathyamamidala/beam-go/main/hello.go) file

When done, now use the command 
```
go run .
```

Create **sample.txt** with Shakespeare content from [here](https://raw.githubusercontent.com/srisathyamamidala/beam-go/main/sample.txt).

## Get the SDK and the examples

```
go get -u github.com/apache/beam/sdks/v2/go/pkg/beam
```
### Run wordcount

```
go install github.com/apache/beam/sdks/v2/go/examples/wordcount
```
To get the **output**, you must now run this command.
```
wordcount --input sample.txt --output sathya-output
```
If you don't the output run the commands below:
```
go get github.com/apache/beam/sdks/v2/go/pkg/beam/io/filesystem/gcs@v2.37.0
```

```
go build hello.go
```
```
go build wordcount.go
```

Now you can get the output : 
```
.\hello.go
```
```
.\wordcount --input sample.txt --output sathya-output
```
```
Get-Content sathya-output
```

