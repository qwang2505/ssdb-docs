# getset key value

Sets a value and returns the previous entry at that key.

## 参数

* `key` - 
* `value` -

## 返回值

If the key already exists, the value related to that key is returned. Otherwise return `not_found` Status Code.

## 示例

	ssdb 127.0.0.1:8888> set a 123
	ok
	(0.000 sec)
	ssdb 127.0.0.1:8888> getset a 321
	123
	(0.000 sec)
	ssdb 127.0.0.1:8888> del a
	ok
	(0.000 sec)
	ssdb 127.0.0.1:8888> getset a 321
	not_found
	(0.000 sec)
	ssdb 127.0.0.1:8888> 
