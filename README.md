# nginx1

1)   [nginx service + docker_con( node(port 8443:8080) + mongo(28443:27017) on ec2] , generated certificate for domain ecom.boldviewers.com using certbot, configured cloudflare pointing to ec2 server with aname record, inside the node we need to provide 27017 port for mongo only and not other than that because both container is in one network.

2) in mongodb url that we configure inside the node url should contain auth source= admin if we have set username, password for database in docker compose file.
3) inside cloudflare for ssl/tls rules we need to provide encryption mode to be full,full strict and not flexible because cloudflare will contact nginx or origin server with http protocol in flexible mode.
