# caddy-with-cloudflare-dns
How to use caddy with cloudflare dns challenge on Raspberry Pi OS

* Go to ```https://caddyserver.com/download```
* Select the preferred architecture on the upper left
* Choose a plugin (in our case ```dns.providers.cloudflare```) and download it.
* In my case, the name of the file will be ```caddy_linux_arm64_custom```
* We are not downloading **a plugin**, but an entire caddy build with that plugin!
* Do a ```chmod +x caddy_linux_arm64_custom```
* Put your Caddyfile in some directory (fon instance, ```/home/pi/caddy/Caddyfile```)
* Run ```./caddy_linux_arm64_custom start --config /home/pi/caddy/Caddyfile```
* If everything works, fix users and permissions to run caddy at boot.

