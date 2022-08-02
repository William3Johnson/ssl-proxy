# SSL Proxy
A simple and easy to install SSL proxy. Can use different ports and standalone certificate files.

# Usage
1) First, install the dependencies using ```npm install```.
2) Then replace the files ```default.crt``` and ```default.key``` with your own SSL files, within the ```/assets/ssl``` directory.
3) You can change the proxy listening port (default is 443), the proxy redirecting port (default is 80), and rename the CRT and KEY files' path by editing ```index.js```.
4) Change the CHMOD of the file ```stop.sh``` by using the commannd ```chmod 755 stop.sh``` in the root directory of the repository.
5) Now just run the script by using ```npm start```. You should have your SSL certificate intalled and running on the listening port (default is 80) straight away.

You can stop the script by using the command ```npm stop```, and you will have to do it if you want to update the SSL certificate or change the port.

## Use Root & Intermediate Certificates

We have added Root and Intermediate Certificate compatibility, using CA Bundles. Some applications will require this extra level of security to work, and to use it all you need to do is to replace the file `/assets/ssl/default.ca` with your own CA Bundle file, and run `npm start-ca` to start the proxy server.

# Compatibility
Tested on Linux Ubuntu 20.04 LTS. Should work nicely on MacOS X, but the script hasn't been tested on Windows. I believe it should work fine on Windows, aside from the ```chmode``` command, that is not available, and you will have to change the file mode some other way around.

# Credit
This is a free to use, and free to distribute repository by Nova Network, created by Paulo Baronceli. Use at your own risk, and we accept no liability from the usage of this script.
