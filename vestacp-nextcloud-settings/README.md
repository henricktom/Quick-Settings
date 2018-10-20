## vestacp-nextcloud-template both stpl and tpl
Web templates for Vesta Control Panel to run Nextcloud or Owncloud under Apache. Works with nginx proxy too. 

Download these files into /usr/local/vesta/data/templates/web/apache2 

Follow the steps and these files 
```
cd /usr/local/vesta/data/templates/web/apache2
wget https://raw.githubusercontent.com/plutocrat/vestacp-nextcloud-template/master/nextcloud.tpl
wget https://raw.githubusercontent.com/plutocrat/vestacp-nextcloud-template/master/nextcloud.stpl
```

Reuse - every time.
Then select them from the Control Panel > Domains > yourdomainname.com > Templates

```
Force to use SSL - if enabled

use any method described in this folder 
https://github.com/dewDrive/Quick-Settings/tree/master/dot-htaccess-files - 3 Methods availble. 
I have tested it with method 3 - its is confirmed to work .
```
