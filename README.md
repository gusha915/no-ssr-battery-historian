# no-ssr-battery-historian

解决battery historian国内网络无ssr而无法部署问题

1. 下载go版本battery historian  
1.1 go get -d -u github.com/google/battery-historian/...  
或者  
1.2 git clone github.com/google/battery-historian.git  
2. 下载base.html 替换原码下的 battery-historian\templates\base.html
3. 下载好cdn目录 放入到battery-historian\third_party 目录
4. 进行 cd $GOPATH/src/github.com/google/battery-historian
5. 运行 go run setup.go 进行编译
6. 运行 go run cmd/battery-historian/battery-historian.go  
