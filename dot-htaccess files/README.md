<img src="https://global.dewdrive.com/thegreatcompany/emblem/dew_black_logo.png" align="right" />
<img src="https://global.dewdrive.com/thegreatcompany/help/github/www-or-non-www.png" align="center" />



## Why we should stick with - either www or non-www style.
Its a matter of choice mainly 
 
 - but if you choose, then stick to it no matter what.
 if not
 
 1) It will surely spoil your brand reputation in Search engine by competing with your own keywords 
 2) The site will be listed for duplicate content.
 3) It affects and gives us many broke link
 4) Redirection loops.
 5) Cache problems etc.
 
 
## Why  We choose not to use www?

1)We believe keeping consistency is very important on the web. <br>
2)its only 'three letter word less (www)' to type and save many billions of byets on a global scale.<br>
3)We belive it will look bit more nicer and should follow non-www method. <br>




"Search for Stats on what people type in the URL bar" and have better knowledge .

## How to Use the files 

Just download and  put the file in root ".htaccess" 
This file is a hidden type file so , you must enable to view hidden files .

## Tip Before you use/test the files 
```
Use R Temp Redirect flag for testing purpose and to avoid browser caching.
If you want to make the redirect Temporary , just change it to  R flag OR R=307 ( 307 = Temporary )
After testing ->
R = 301 = Tells browser/robot to do a permanent redirect( 301 Moved Permanently )


L = If the rule was processed, don't process any more.

```
To read more about flags 
https://github.com/dewDrive/Quick-Settings/blob/master/htaccess%20-Flag%20List.md


## Method - 1 Generic method all conditions meet http and non-https to non-www.


File name :- .htaccess
  
```
RewriteCond %{HTTPS} off
RewriteCond %{HTTP_HOST} ^www\.(.*)$ [NC]
RewriteRule ^(.*)$ https://%1/$1 [R=301,L]

RewriteCond %{HTTPS} on
RewriteCond %{HTTP_HOST} ^www\.(.*)$ [NC]
RewriteRule ^(.*)$ https://%1/$1 [R=301,L]

```
Works everywhere on every condition.
Note :- If you dont have SSL = Remove "s" from https for non ssl redirection.


 ## Method - 2 From www to non-www (with ssl) - Domin encoded method and most preferd with lowest over head.


File name :- .htaccess2
  
```
RewriteEngine On
RewriteCond %{HTTP_HOST} ^www\.
RewriteRule ^(.*)$ https://dewdrive.com/$1 [R=301,QSA]

```
Just change https://dewdrive.com/ with your domain. Remove "s" from https for non ssl redirection.

Need HSTS Enabled for better working in all edge cases(proper ssl redirection ) (or) Use => Method 1


 ## Method - 2 From www to non-www (with ssl) - Generic method 


File name :- .htaccess3
  
```
RewriteEngine On
RewriteBase /
RewriteCond %{HTTP_HOST} ^www\.(.*)$ [NC]
RewriteRule ^(.*)$ https://%1/$1 [R=301,L]
```

Note :- If you dont have SSL = Remove "s" from https for non ssl redirection.
Need HSTS Enabled for better working in all edge cases(proper ssl redirection ) (or) Use => Method 1

 

##choose from 

| File Name  | SSL Support  | Rediretion        | Description               | Redirection Condition |
| ---------- |   ---------- | ----------------- | -------------             | ------------------    |
| .htaccess  |    100%      |  All Case         | Download and Ready to Use |       **1**           |
| .htaccess1 |    90%       |  90%Case          | & Change to urdomain.com  |       **1**           |
| .htaccess2 |    90%       |  90%Case          | Rename to .htacceess      |      **2*2**          |

