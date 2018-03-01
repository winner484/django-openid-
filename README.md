django获得openid的种种

urlopen3.0的用法和2.0不一样。

from urllib.request import urlopen

with urlopen('https://...') as url:
    r = url.read()
