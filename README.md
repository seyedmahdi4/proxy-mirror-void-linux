### proxy mirror for Void Linux with Nginx and caching

###### This [gist](https://gist.github.com/cryptarch/7837e382b861e5c3633802f7bc332f0a) helped me for to write this repo.

For use with your domain and SSL (lets encrypt) change name of the ```conf.d/void.example.com.conf``` and line 3 in the same file to **your domin**.

You can use it just with IP and just change line 3 of config file to your server IP.

##### lets encrypt and ssl:
```sh
# install it in Ubuntu 18.04 and later
sudo apt-get update
sudo apt-get install certbot
sudo apt-get install python3-certbot-nginx

# test and reload your config if you don't
sudo nginx -t && sudo nginx -s reload

# certbot -- Put your domain instead of void.example.com
sudo certbot --nginx -d void.example.com
```
