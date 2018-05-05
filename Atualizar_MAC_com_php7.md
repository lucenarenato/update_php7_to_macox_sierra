# Como atualizar sua versão do PHP para 7.0 no macOS Sierra
## Você tem duas opções:brew or curl install

``
	Brew

	brew update && brew upgrade
	brew tap homebrew/dupes
	brew tap homebrew/versions
	brew tap homebrew/homebrew-php
	brew unlink php56 
	brew install php70

	You might get an error if PHP 5.6 has not been installed by brew previously, but don't worry, you can simply continue``

# CURL

$ curl -s http://php-osx.liip.ch/install.sh | bash -s 7.0

## Você pode substituir 7.0 por 7.1 no comando acima para obter a versão 7.1 do PHP

## Se a saída do php -v ainda não ecoa a versão 7, simplesmente digite este comando para 
## atualizar o seu caminho, ele deve fazer a mágica, como indicado no site php-osx.liip.ch

$ export PATH=/usr/local/php5/bin:$PATH

## Aparentemente, o env var pode ter mudado dependendo do seu ambiente.

## Se o acima não funcionar, você pode tentar 

$ export PATH=”$(brew — prefix homebrew/php/php70)/bin:$PATH”

## Site Official:

- https://php-osx.liip.ch/