# Install dependencies.

sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev libevent-dev make unzip git redis-server g++ libjansson-dev libpython-dev expat libexpat1-dev

cd $HOME

git clone https://github.com/DaTaK-BoT/DaTaK.git

cd TeleSeed

chmod +x datakfix

chmod +x datak

./datakfix install

cd .luarocks

cd bin

./luarocks-5.2 install luafilesystem

./luarocks-5.2 install lub

./luarocks-5.2 install luaexpat

cd $HOME

cd DaTaK

./datakfix install

./datak # Enter a phone number & confirmation code.
