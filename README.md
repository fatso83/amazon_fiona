#Reverse engineering the Kindle web management api

A utility library of functions that makes it possible to interact with
Amazon's FIONA system for administrating the titles on your Kindle.
Not yet expanded to a full program, just some examples on how to use it.

## Sample output
    Has 273 personal documents. The last one is Instapaper: Friday, Jun. 14
    Has bought 68 e-book titles from Amazon. The last one is Kindle User's Guide
    Last 15 personal documents:
    b'[WQFCJDOWZTUYD67XG4RYNXDUVNZNPOJR]  Instapaper: Friday, Jun. 14'
    b'[CASOR2TMKI2BJZZK3LCRIPSRPIYZSHQR]  Instapaper: Friday, May. 31'
    b'[ECQRQWCYWWGJ3LEBNAVHI2RCYNWVETMD]  Instapaper: Tuesday, May. 28'
    b'[G7XCGX3J7CIM6NPPVQYOE3T7LXMYD2JT]  Instapaper: Monday, May. 27'
    b'[453JXHDZ54TNOYWXUYDK2KO726WU35DZ]  Where to Start | Trent Walton'
    b'[UGA6O2GBB5AK7ARQKUIV6KIJBSQD6RUZ]  Instapaper: Monday, Apr. 29'
    b'[ZNA3TVXIEKVLFOAUMKVOEIX2ODQYT4ND]  Kan man kode en fj\xc3\xb8l? -\nAftenposten'
    b'[UNMNWZ4RMLLYNCTVCWSFP7LJE7OB7UWY]  Instapaper: Wednesday, Apr. 3'
    b'[342EV2DYXSME5AQCSNEMH657VRWCNDJT]  Instapaper: Thursday, Mar. 14'
    b'[O5ED7XM2HMRDYGFEBNZAPU4ZCV3VDNPY]  Instapaper: Saturday, Mar. 16'
    b'[IS3MO5QBISEGJLELCD6E2WIJ5S2GGBVS]  Instapaper: Monday, Mar. 11'
    b'[T3YSWNAEWN7BQINXN7QSLYPMEBRICL2Z]  Instapaper: Sunday, Mar. 10'
    b'[EWOMLNB23DJL4JULE4NZH2WCT3KT6WP7]  Instapaper: Wednesday, Mar. 6'
    b'[C3FSZOVACMBTPN5CPRXYPWFFJ6YWDPRX]  Instapaper: Tuesday, Mar. 5'
    b'[64UKAMPFTLVAEAMWKJYZNTUEIUL335M3]  Instapaper: Thursday, Feb. 28'

## Other
There are also some notes (in Norwegian and English) I jotted down while trying to
find out how Amazon's FIONA system for managing your Kindle archive is
working, and how I was supposed to use curl to get in.

Thankfully I abandened the idea of scripting this in Bash + cURL, and
starting hacking on a Python version using the Requests library and
BeautifulSoup. Some hours later I finally got in :-)

## Installing requirements
pip install --user -r requirements.txt
