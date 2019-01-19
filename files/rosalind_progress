#!/usr/bin/python3

import re
import urllib.request

weburl = urllib.request.urlopen('http://rosalind.info/users/jake_sauter/')

data = str(weburl.read())

completed = len(re.findall('badge-success',data))

total = len(re.findall('badge',data))

percent_complete = completed / total 

print('================================================================')
print('You are now ' + str(round(percent_complete, 2)*100) + '% complete with rosalind training')
print('You have completed ' + str(completed) + ' problems out of a total ' + str(total) + ' problems')
print('================================================================')
