# browser-ech

瀏覽器如何開啓ECH(Encrypted Client Hello)，保護你的隱私，防止中間人攻擊(Man-in-the-middle attack)

支援ECH的網站才有效果

測試ECH是否開啓

[https://crypto.cloudflare.com/cdn-cgi/trace/](https://crypto.cloudflare.com/cdn-cgi/trace/)

[https://defo.ie/ech-check.php](https://defo.ie/ech-check.php)

<br>
<br>
<br>

## firefox

* 1. 設定->鏈接設定->開啓DNS over HTTPS(cloudflare)

* 2. 位址欄輸入about:config

* 3. network.dns.echconfig.enabled = true

* 4. network.dns.http3_echconfig.enabled = true

* 5. network.dns.use_https_rr_as_altsvc = true

* 6. network.security.esni.enabled = true

* 7. network.trr.mode = 3 &nbsp;&nbsp;&nbsp;&nbsp;（可選）

[https://crypto.cloudflare.com/cdn-cgi/trace/](https://crypto.cloudflare.com/cdn-cgi/trace/)

結果
```
......
sni=encrypted
......
```
