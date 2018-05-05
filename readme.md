atualizar php do macos sierra

o meu estava php 5.6.30
Terminal

executei este comando
curl -s https://php-osx.liip.ch/install.sh | bash -s 7.0

aguarde

apos vc entra na pasta no terminal 
cd /usr/local

veja que no meu tem duas versoes agora do php

mas para funcionar voce tem executar outro comando

export PATH=/usr/local/php5/bin:$PATH

altere para nome que esitiver o php 7

o meu estava assim
export PATH=/usr/local/php5-7.0.24-20171002-092027/bin:$PATH

apos e so verificar a versao 
php -v

PHP 7.0.24

sudo apachectl stop
