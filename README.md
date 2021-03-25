# see-websites-code
import requests
from bs4 import BeautifulSoup as bs

github_user = input('input github user: ')
url = 'https://www.youtube.com/'+github_user
r = requests.get(url)
soup = bs(r.content, 'html.parser')
print(soup)
