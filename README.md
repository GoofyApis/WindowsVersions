# WindowsVersions

originally planned on making a api to download ios files but thats kind of illegal so isntead a api to fetch all of the windows versions that existed

- [x] Main Windows Versions
- [ ] Other Editions of the Main Windows Versions (Home, Pro, Entreprise, Education etc)
- [ ] Other goofy windows versions like windows server and stuff and windows tablets/phones
- [ ] Maybe support for their codenames too :/

## How do i use this "api"

You need to make a request to https://raw.githubusercontent.com/GoofyApis/WindowsVersions/main/winverlist.json and then find the windows version you need from the json data. Heres an example of how you can get a list of the windows versions in *Python*

```python

import requests

url = "https://raw.githubusercontent.com/GoofyApis/WindowsVersions/main/winverlist.json"
versions = requests.get(url).json()["versions"]
print(versions)

```

### Source of the information
https://en.wikipedia.org/wiki/List_of_Microsoft_Windows_versions
