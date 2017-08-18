
<!-- > pandoc proxy.md --include-in-header=../header.txt -s -o proxy.html -->

**プロキシの設定**

大分高専のネットワークではプロキシを通してインターネットに接続することになっているので、時々不便なことが起きます。

Windowsでは環境変数を  
- HTTP_PROXY → proxy.oita-ct.ac.jp:80
- HTTPS_PROXY → proxy.oita-ct.ac.jp:80
と設定しておきます。
