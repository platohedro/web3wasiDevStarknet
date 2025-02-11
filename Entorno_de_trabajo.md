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
sh

sudo dnf install golan

Clonar el repositorio de ASDF:
sh

git clone https://github.com/asdf-vm/asdf.git --branch v0.16.0

Ejecutar make:
sh

cd asdf
make

Copiar el binario a un directorio en tu $PATH:
sh

sudo cp asdf /usr/local/bin/

Verificar que asdf esté en tu $PATH:
sh

type -a asdf

Debian

Instalar las dependencias necesarias:
sh

sudo apt-get install golang

Clonar el repositorio de ASDF:
sh

git clone https://github.com/asdf-vm/asdf.git --branch v0.16.0

Ejecutar make:
sh

cd asdf
make

Copiar el binario a un directorio en tu $PATH:
sh

sudo cp asdf /usr/local/bin/

Verificar que asdf esté en tu $PATH:
sh

type -a asdf

You can now update the Entorno_de_trabajo.md file with these organized instructions.
