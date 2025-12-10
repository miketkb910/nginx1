# nginx1
[nginx service + docker_con( node(port 8443:8080) + mongo(28443:27017) on ec2] , generated certificate for domain ecom.boldviewers.com using certbot, configured cloudflare pointing to ec2 server with aname record, inside the node we need to provide 27017 port for mongo only and not other than that because both container is in one network.
