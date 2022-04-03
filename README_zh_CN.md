etag
========
[![GitHub release](https://img.shields.io/github/release/amalfra/etag.svg)](https://github.com/amalfra/etag/releases)
![Build Status](https://github.com/amalfra/etag/actions/workflows/test.yml/badge.svg?branch=main)
[![GoDoc](https://godoc.org/github.com/amalfra/etag?status.svg)](https://godoc.org/github.com/amalfra/etag)
[![Go Report Card](https://goreportcard.com/badge/github.com/amalfra/etag)](https://goreportcard.com/report/github.com/amalfra/etag)

一个用于创建 HTTP ETags 的 Go 包（基于[RFC 7232](https://www.rfc-editor.org/rfc/rfc7232.txt)），用于 HTTP 响应。

## 安装
你可以用以下方式安装软件包
```sh
go get github.com/amalfra/etag
```

## 使用
下一步，引入这个包
``` go
import (
  "github.com/amalfra/etag"
)
```
现在你可以调用 ```generate``` 方法创建 ETag。第二个参数是布尔值，用来指定生成的 ETag 是否必须是弱的。
```go
etag.Generate(body, false)
```
生成弱的 Etag
```go
etag.Generate(body, true)
```

## 开发

如果有任何疑问、难题或建议，请发布到[这里](https://github.com/amalfra/etag/issues)。

你可以通过 Fork 这个项目和提交一个 PR 来贡献项目。提交之前请确保项目运行 ```make test``` 测试是通过的。

## 基于 MIT 开源协议

The MIT License (MIT)

Copyright (c) 2017 Amal Francis

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
