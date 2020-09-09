## NGINX reverse proxy and SSL

The NGINX reverse proxy is the key to this whole setup. Its job is to listen on external ports 80 and 443 and connect requests to corresponding
Docker containers, without exposing their inner workings or ports directly to the outside world. Additionally, with the SSL companion container 
the proxy also automatically redirects all HTTP requests to HTTPS and handles SSL encryption for all traffic, including certificate management.

## Reference: 
**[Hosting multiple sites or applications using Docker and NGINX reverse proxy with Letsencrypt SSL](https://olex.biz/2019/09/hosting-with-docker-nginx-reverse-proxy-letsencrypt/)
