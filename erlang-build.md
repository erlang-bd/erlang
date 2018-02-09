### [Erlang Build From Source Code](http://erlang.org/doc/installation_guide/INSTALL.html)

### Install Dependencies
```sh
sudo apt-get update
sudo apt-get dist-upgrade
sudo apt-get install build-essential
sudo apt-get install git
sudo apt-get install m4
sudo apt-get install ncurses-term
sudo apt-get install ncurses-base
sudo apt-get install ncurses-bin
sudo apt-get install sed
sudo apt-get install autoconf
sudo apt-get install installation-guide-amd64
sudo apt-get install openssl
sudo apt-get install flex
sudo apt-get install gs
sudo apt-get install wxwidget
sudo apt-get install xsltproc
sudo apt-get install fop
sudo apt-cache search libmyodbc
sudo apt-get install mysql-server
mysql_secure_installation
mysql -u root -p
sudo apt-get install libncurses5-dev libncursesw5-dev libssl-dev
sudo apt-get install libxml2-utils xsltproc
sudo apt-get install unixodbc-dev
sudo apt-get install libwxbase2.8
sudo apt-get install libwxgtk2.8-dev
sudo apt-get install libqt4-opengl-dev
sudo apt-get install libwxbase3.0-dev
sudo apt-get install libwxgtk3.0-dev
sudo apt-get install libqt5
sudo apt-get install libqt5opengl5-dev
sudo apt-get install libgtk
sudo apt-get install libxml2-dev
sudo apt-get install libxml
sudo apt-get install libxmlsec1
sudo apt-get install unixodbc-dev
```

### Build Start
```
cd /opt/erlang/
export ERL_TOP=`pwd`
./configure --with-ssl
make -j8
```

