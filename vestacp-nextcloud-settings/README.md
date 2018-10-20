<img src="https://global.dewdrive.com/thegreatcompany/emblem/dew_black_logo.png" align="right" />
<img src="https://vestacp.com/img/vesta_logo.png" align="right" />
<img src="https://global.dewdrive.com/thegreatcompany/help/github/nextcloud-owncloud-logo.png" align="right" />


## vestacp-nextcloud-template both stpl and tpl - 
Web templates

# Vesta Control Panel =>  Nextcloud or Owncloud under Apache. 

Supports with nginx and Apache proxy too. 

Download these files into /usr/local/vesta/data/templates/web/apache2 

Follow the steps and these files 
```
cd /usr/local/vesta/data/templates/web/apache2
wget https://raw.githubusercontent.com/dewDrive/Quick-Settings/master/vestacp-nextcloud-settings/nextcloud.tpl
wget https://raw.githubusercontent.com/dewDrive/Quick-Settings/master/vestacp-nextcloud-settings/nextcloud.stpl
```
or uplad both files to the root of apache2

Reuse - every time.
Then select them from the Control Panel > Domains > yourdomainname.com > Templates

```
Force to use SSL - if enabled

use any method described in this folder 
https://github.com/dewDrive/Quick-Settings/tree/master/dot-htaccess-files - 3 Methods availble. 
I have tested it with method 3 - its is confirmed to work .
```
