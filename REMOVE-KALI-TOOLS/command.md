LIST ::
dpkg --get-selections
or dpkg --get-selections | grep something

REMOVE ::
try   :
sudo apt-get purge <package-name>
catch :
sudo apt --fix-broken install
sudo apt-get purge <package-name>

CLEAN ::
sudo apt-get autoremove
sudo apt-get autoclean
