# bytesconv

see https://github.com/gin-gonic/gin/blob/dda12b973129b0d3d1889586f57cea6076884783/internal/bytesconv/bytesconv.go

StringToBytes instead of []byte(s)  
BytesToString instead of string(s)

```golang
func rawStrToBytes(s string) []byte {
	return []byte(s)
}
var s  = "abcd"
var sb = rawStrToBytes(s) 
var sb2 = StringToBytes(s) 

func rawBytesToStr(b []byte) string {
	return string(b)
}

var sb = []byte{'a','b','c','d'}
var s = rawBytesToStr(sb)
var sb2 = BytesToString(sb)

```
