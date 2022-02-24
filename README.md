# Secret Regex List
List of regex for scraping secret API keys and juicy information.

```
Artifactory API Token

(?:\s|=|:|"|^)AKC[a-zA-Z0-9]{10,}

Artifactory Password

(?:\s|=|:|"|^)AP[\dABCDEF][a-zA-Z0-9]{8,}

Authorization Basic

basic [a-zA-Z0-9_\\-:\\.=]+

Authorization Bearer

bearer [a-zA-Z0-9_\\-\\.=]+

AWS Client ID

(A3T[A-Z0-9]|AKIA|AGPA|AIDA|AROA|AIPA|ANPA|ANVA|ASIA)[A-Z0-9]{16}

AWS MWS Key

amzn\.mws\.[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}

AWS Secret Key

(?i)aws(.{0,20})?(?-i)['\"][0-9a-zA-Z\/+]{40}['\"]

Base32

(?:[A-Z2-7]{8})*(?:[A-Z2-7]{2}={6}|[A-Z2-7]{4}={4}|[A-Z2-7]{5}={3}|[A-Z2-7]{7}=)?

Base64

(eyJ|YTo|Tzo|PD[89]|aHR0cHM6L|aHR0cDo|rO0)[a-zA-Z0-9+/]+={0,2}

Basic Auth Credentials

(?<=:\/\/)[a-zA-Z0-9]+:[a-zA-Z0-9]+@[a-zA-Z0-9]+\.[a-zA-Z]+

Cloudinary Basic Auth

cloudinary:\/\/[0-9]{15}:[0-9A-Za-z]+@[a-z]+

Facebook Access Token

EAACEdEose0cBA[0-9A-Za-z]+

Facebook Client ID

(?i)(facebook|fb)(.{0,20})?['\"][0-9]{13,17}

Facebook Oauth

[f|F][a|A][c|C][e|E][b|B][o|O][o|O][k|K].*['|\"][0-9a-f]{32}['|\"]

Facebook Secret Key

(?i)(facebook|fb)(.{0,20})?(?-i)['\"][0-9a-f]{32}

Github

(?i)github(.{0,20})?(?-i)['\"][0-9a-zA-Z]{35,40}

Google API Key

AIza[0-9A-Za-z\\-_]{35}

Google Cloud Platform API Key

(?i)(google|gcp|youtube|drive|yt)(.{0,20})?['\"][AIza[0-9a-z\\-_]{35}]['\"]

Google Drive API Key

AIza[0-9A-Za-z\\-_]{35}

Google Drive Oauth

[0-9]+-[0-9A-Za-z_]{32}\.apps\.googleusercontent\.com

Google Gmail API Key

AIza[0-9A-Za-z\\-_]{35}

Google Gmail Oauth

[0-9]+-[0-9A-Za-z_]{32}\.apps\.googleusercontent\.com

Google Oauth Access Token

ya29\\.[0-9A-Za-z\\-_]+

Google Youtube API Key

AIza[0-9A-Za-z\\-_]{35}

Google Youtube Oauth

[0-9]+-[0-9A-Za-z_]{32}\.apps\.googleusercontent\\.com

Heroku API Key

[h|H][e|E][r|R][o|O][k|K][u|U].{0,30}[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12}

IPv4

\b(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)){3}\b

IPv6

(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,5}(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:){1,4}(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|([0-9a-fA-F]{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]{1,4}){1,7}|:)|fe80:(:[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(ffff(:0{1,4}){0,1}:){0,1}((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])|([0-9a-fA-F]{1,4}:){1,4}:((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9]))

Javascript Variables

(?:const|let|var)\s+\K(\w+?)(?=[;.=\s])

LinkedIn Client ID

(?i)linkedin(.{0,20})?(?-i)['\"][0-9a-z]{12}['\"]

LinkedIn Secret Key

(?i)linkedin(.{0,20})?['\"][0-9a-z]{16}['\"]

Mailchamp API Key

[0-9a-f]{32}-us[0-9]{1,2}

Mailgun API Key

key-[0-9a-zA-Z]{32}

Mailto:

(?<=mailto:)[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9.-]+

MD5 Hash

[a-f0-9]{32}

Picatic API Key

sk_live_[0-9a-z]{32}

Slack Token

xox[baprs]-([0-9a-zA-Z]{10,48})?

Slack Webhook

https://hooks.slack.com/services/T[a-zA-Z0-9_]{10}/B[a-zA-Z0-9_]{10}/[a-zA-Z0-9_]{24}

Stripe API Key

(?:r|s)k_live_[0-9a-zA-Z]{24}

Square Access Token

sqOatp-[0-9A-Za-z\\-_]{22}

Square Oauth Secret

sq0csp-[ 0-9A-Za-z\\-_]{43}

Twilio API Key

SK[0-9a-fA-F]{32}

Twitter Client ID

(?i)twitter(.{0,20})?['\"][0-9a-z]{18,25}

Twitter Oauth

[t|T][w|W][i|I][t|T][t|T][e|E][r|R].{0,30}['\"\\s][0-9a-zA-Z]{35,44}['\"\\s]

Twitter Secret Key

(?i)twitter(.{0,20})?['\"][0-9a-z]{35,44}

Vault Token

[sb]\.[a-zA-Z0-9]{24}

URL Parameter

(?<=\?|\&)[a-zA-Z0-9_]+(?=\=)

URLs

With HTTP Protocol:

https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)

Without Protocol:

[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)

```
