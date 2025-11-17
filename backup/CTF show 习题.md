# web3
从容器里面看出是php伪协议，存在文件包含漏洞，参数是url,在地址栏后面加/?url=php://input利用伪协议读取发送过去的post数据包并执行，用bp代理进行抓包，在bp中将GET类型改为POST类型，并在最后一行空一行后写入php代码，用ls指令查看目录，发现ctf_go_go_go的文件，最后再写入cat ctf_go_go_go 命令就得到了flag