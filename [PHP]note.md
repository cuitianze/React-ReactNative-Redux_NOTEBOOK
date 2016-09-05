### 升级PHP7
```
cd ~
curl 'https://setup.ius.io/' -o setup-ius.sh
sudo bash setup-ius.sh

sudo yum remove php-cli mod_php php-common
sudo yum install mod_php70u php70u-cli php70u-mysqlnd php70u-json -y

```

### Yii
```
curl -sS https://getcomposer.org/installer | php
php composer.phar global require fxp/composer-asset-plugin --no-plugins
php composer.phar install
```
