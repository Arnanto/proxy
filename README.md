# proxy
proxy settings

if your apt get error causes proxy, you can use this.

in the command line, type:
sudo nano /etc/apt/apt.conf
if file is doesn't exist, do not confuse. After that add following line:
Acquire::http::proxy "http://yourproxyaddress:proxyport";
Acquire::https::proxy "http://yourproxyaddress:proxyport";
Acquire::ftp::proxy "http://yourproxyaddress:proxyport";

if proxy use password, change "http://yourproxyaddress:proxyport" with:
"http://username:password@yourproxyaddress:proxyport";

Hope it can help you :)
