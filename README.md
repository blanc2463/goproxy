L1 Proxy:
./L1proxy http -t tcp -p :19999 -C proxy.crt -K proxy.key
L2 Proxy:
.\goproxy.exe http --always  -p :8080 -T tcp -P 47.238.236.206:19999 -C proxy.crt -K proxy.key
