## vestacp-nextcloud-template both stpl and tpl
Web templates for Vesta Control Panel to run Nextcloud or Owncloud under Apache. Works with nginx proxy too. 

Download these files into /usr/local/vesta/data/templates/web/apache2 
Follow the steps. 

```
cd /usr/local/vesta/data/templates/web/apache2
wget https://raw.githubusercontent.com/plutocrat/vestacp-nextcloud-template/master/nextcloud.tpl
wget https://raw.githubusercontent.com/plutocrat/vestacp-nextcloud-template/master/nextcloud.stpl
```

Then select them from the Control Panel > Domains > Domainname.com > Templates

If you have enabled SSL, then also put this in your .htaccess file, which will force an SSL connection. 

```
Fource SSL 

use ant methode described in this folder 
```
