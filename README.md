#JsonParser

##项目简介

本项目实现一个json字符串的解析，将其转化成正确的json格式进行输出，同时考虑到格式的美观，对于json的显示进行了相关换行和缩进的处理

##主要函数

```swift
func ParserNull(json: inout String,level: Int=1) -> (String?,Bool)
func ParserBool(json: inout String,level: Int=1) -> (String?,Bool)
func ParserArray(json: inout String,level: Int=1) -> (String?,Bool) 
func ParserString(json: inout String,level: Int=1) -> (String?,Bool)
func ParserNumber(json: inout String,level: Int=1) -> (String?,Bool) 
func ParserValue(json: inout String,level: Int=1) -> (String?,Bool)
func ParserObject(json: inout String,level: Int=0)->(String?,Bool)
```

1. 通过level对于json的相关换行和缩进数量进行标记
2. 通过返回的Bool值来判断json格式是否正确

