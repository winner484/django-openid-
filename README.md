django获得openid的种种

给制定地址发送请求：urlopen3.0的用法和2.0不一样。

from urllib.request import urlopen

with urlopen('https://...') as url:
    r = url.read()
    
    
django接收到json数据后的处理

r2 = simplejson.loads(r.decode('utf-8'))  注意这个utf-8，没有的话就报错。

openid = r2['openid']   #从json中获得某一项内容openid
