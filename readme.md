1. in hosts:flask-nodes we set up our enviroment for our flask application by installing os packages, python, git, pip. Then we are syncing repository with our app in /opt adding user and changing permissions. The next step is adding requrements and installing them in our virtual environment. Next step is putting config file to /etc/systemd/system and starting service.
2. in hosts: proxy_nodes we setup proxy server for our app. We have to install epel, nginx and put conf file to /etc/nginx/conf.d, then reload nginx.

app server: priv ip - 172.31.15.233 public - 3.66.121.198
proxy server: priv - 172.31.1.7 public - 3.127.236.224


to execute -> ansible-playbook setup.yml -i hosts.ini


