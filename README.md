# deploying for my local instance

- Ubuntu 18.04.2 / x86_64
- nodejs v12.0
```
 # Using Ubuntu
 curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
 sudo apt-get install -y nodejs
 npm install
```
- edit config files
 - config/caps.json
 - config/public.json
 - config/private.json
 - config/probe.json
- edit index.html
To provide by http(not https), download some *.js/*.ccs on local storage and edited index.html
```
 mkdir static/localcache
 cd static/localcache
 wget https://nodejs.org/download/release/v12.0.0/node-v12.0.0-linux-x64.tar.gz
 wget https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css
 wget https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap-theme.min.css
 wget https://cdnjs.cloudflare.com/ajax/libs/bootstrap-toggle/2.2.2/css/bootstrap-toggle.min.css
 wget https://cdnjs.cloudflare.com/ajax/libs/github-fork-ribbon-css/0.2.1/gh-fork-ribbon.min.css
 wget https://mtr.sh/css/intrace.css
 wget https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js
 wget https://cdnjs.cloudflare.com/ajax/libs/jquery-scrollTo/2.1.2/jquery.scrollTo.min.js
 wget https://cdnjs.cloudflare.com/ajax/libs/bootstrap-toggle/2.2.2/js/bootstrap-toggle.min.js
 wget https://cdnjs.cloudflare.com/ajax/libs/socket.io/1.7.3/socket.io.min.js
 wget https://cdnjs.cloudflare.com/ajax/libs/blueimp-md5/2.7.0/js/md5.min.js
```

These procedures can't follow to update origin. I should check them when pull update.

- run server
 node lg.js

- try to access
 http://myaddress:8080/

I'm enjoying now.
