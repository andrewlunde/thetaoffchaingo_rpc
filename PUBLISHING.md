```
git add .
git commit -m "rpc: changes for v0.1.1"
git tag v0.1.1
git push origin v0.1.1
GOPROXY=proxy.golang.org go list -m github.com/andrewlunde/thetaoffchaingo_rpc@v0.1.1

go get github.com/andrewlunde/thetaoffchaingo_rpc@v0.1.1

  
// in go.mod of application using this module
require github.com/thetatoken/theta/rpc/lib/rpc-codec/jsonrpc2 v0.0.0
replace github.com/thetatoken/theta/rpc/lib/rpc-codec/jsonrpc2 v0.0.0 => github.com/andrewlunde/thetaoffchaingo_rpc v0.1.1

```

