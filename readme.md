
name: gopath_init
clone 下来之后直接把文件复制到gopath目录即可,如果已经配置好了gopath,那么直接 git clone github.com/amandayi/gopath_init %GOPATH%
```go
    git clone github.com/amandayi/gopath_init
```


## 说明

###  第一步,需要把只需要下载不需要编辑的包,重新建立文件夹的包,全部下载
```
git clone github.com/golang/tools // 重建文件夹为 golang.org/x/tools
git clone github.com/karrick/godirwalk
git clone github.com/pkg/errors
git clone github.com/mattn/go-runewidth
go install github.com/karrick/godirwalk
go install github.com/pkg/errors
go install github.com/mattn/go-runewidth
git clone github.com/nsf/gocode // 过时的gocode, git clone github.com/mdempsky/gocode
git clone github.com/sqs/goreturns 
git clone github.com/rogpeppe/godef
git clone github.com/golang/lint/ // 重建为 golang.org/x/lint/
git clone github.com/ramya-rao-a/go-outline
git clone github.com/uudashr/gopkgs
git clone github.com/peterh/liner
git clone github.com/derekparker/delve
```
### 下面的需要哪个是安装哪个,一般安装两个即可 gocode代码提示,goreturns格式化 
```
go install github.com/nsf/gocode // 过时的gocode, go install github.com/mdempsky/gocode
go install github.com/sqs/goreturns 
go install github.com/rogpeppe/godef
go install golang.org/x/lint/golint
go install github.com/ramya-rao-a/go-outline
go install github.com/uudashr/gopkgs/cmd/gopkgs
go install github.com/peterh/liner
go install github.com/derekparker/delve/cmd/dlv
```