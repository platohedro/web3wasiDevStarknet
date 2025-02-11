### Instalación de Go

Fedora
~~~

wget https://go.dev/dl/go1.23.6.linux-amd64.tar.gz
tar -xvf go1.23.6.linux-amd64.tar.gz 
sudo mv go /usr/local/
rm -rf go
ls
cd ~

export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

nano .bashrc
~~~
Agregar al final del archivo .bashrc:

~~~
export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
~~~
Aplicar los cambios del archivo .bashrc:
~~~

source ~/.bashrc
~~~

Debian

~~~
wget https://go.dev/dl/go1.23.6.linux-amd64.tar.gz
tar -xvf go1.23.6.linux-amd64.tar.gz 
sudo mv go /usr/local/
rm -rf go
ls
cd ~

export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

nano .bashrc
~~~
Agregar al final del archivo .bashrc:
~~~

export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
~~~
Aplicar los cambios del archivo .bashrc:
~~~

source ~/.bashrc
~~~


### Instalación de ASDF


Fedora

Instalar las dependencias necesarias:

~~~
sudo dnf install golan
~~~
Clonar el repositorio de ASDF:
~~~

git clone https://github.com/asdf-vm/asdf.git --branch v0.16.0
~~~

Ejecutar make:
~~~

cd asdf
make
~~~
Copiar el binario a un directorio en tu $PATH:

~~~
sudo cp asdf /usr/local/bin/
~~~
Verificar que asdf esté en tu $PATH:

~~~
type -a asdf
~~~
Debian

Instalar las dependencias necesarias:
~~~

sudo apt-get install golang
~~~

Clonar el repositorio de ASDF:
~~~

git clone https://github.com/asdf-vm/asdf.git --branch v0.16.0
~~~

Ejecutar make:
~~~

cd asdf
make
~~~

Copiar el binario a un directorio en tu $PATH:
~~~

sudo cp asdf /usr/local/bin/
~~~

Verificar que asdf esté en tu $PATH:

~~~
type -a asdf
~~~

Instala los plugins asdf Scarb, Starknet Foundry y Starknet Devnet:

~~~
asdf plugin add scarb
asdf plugin add starknet-foundry
asdf plugin add starknet-devnet

~~~

Instala las últimas versiones de Scarb, Starknet Foundry y Starknet Devnet:

~~~
asdf install scarb latest
asdf install starknet-foundry latest
asdf install starknet-devnet latest
~~~

Establecer versiones globales para Scarb, Starknet Foundry y Starknet Devnet:

~~~
asdf global scarb latest
asdf global starknet-foundry latest
asdf global starknet-devnet latest
~~~

Reinicie el terminal y compruebe que Scarb, Starknet Foundry y Starknet Devnet están instalados correctamente:

~~~
scarb --version
snforge --version && sncast --version
starknet-devnet --version
~~~
