```
import requests
r = requests.get('https://pass')
print(r.headers)
print(r.headers['server'])
```
