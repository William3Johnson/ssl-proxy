# SSL Proxy
A simple and easy to install SSL proxy. Can use different ports and standalone certificate files.

# Usage
1) First, install the dependencies using ```npm install```.
2) Then replace the files ```default.crt``` and ```default.key``` with your own SSL files, within the ```/assets/ssl``` directory.
3) You can change the proxy port (default is 80) and rename the CRT and KEY files by editing ```index.js```.
4) Change the CHMOD of the file ```stop.sh``` by using the commannd ```chmod 755 stop.sh``` in the root directory of the repository.
5) Now just run the script by using ```npm start```. You should have your SSL certificate intalled and running straight away.

You can stop the script by using the command ```npm stop```, and you will have to do it if you want to update the SSL certificate or change the port.

This is a free to use, and free to distribute repository by Nova Network, created by Paulo Baronceli.
