# proxy
proxy settings

if your apt get error causes proxy, you can use this.

in the command line, type:
sudo nano /etc/apt/apt.conf

if file is doesn't exist, do not confuse. After that add following line:
Acquire::http::proxy "http://proxyaddress:proxyport";
Acquire::https::proxy "http://proxyaddress:proxyport";
Acquire::ftp::proxy "http://proxyaddress:proxyport";

if proxy use password, change "http://proxyaddress:proxyport" with:
"http://username:password@proxyaddress:proxyport";

Hope it can help you :)
