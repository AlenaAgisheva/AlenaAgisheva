import requests
from bs4 import beautifulsoup
url = ""
response = requests.get(url)
soup = beautifulsoup(response.text, "html.parser")
links = soup.find_all("a")
for link in links:
  print(link.get("href"))
