# Udacity Server Configuration Project

## Server info
* IP Address: 52.10.134.69
* SSH Port: 2200
* URL to app: http://gallery.randomlysa.com/

## Software Installed
* ufw
* postgresql-9.3
* apache2
* libapache2-mod-wsgi 
* python-dev
* python-psycopg2
* git
* python-imaging (for my app, to create thumbnails)
* python-pip

## Python packages
* mod_wsgi
* sqlalchemy
* flask==0.9
* Flask-SQLAlchemy
* Flask-Login==0.1.3
* oauth2client
* werkzeug==0.8.3

## Resources:
* https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
* https://www.linode.com/docs/getting-started
* https://www.linode.com/docs/security/securing-your-server
* http://www.ducea.com/2006/08/11/apache-tips-tricks-deny-access-to-some-folders/
* https://help.ubuntu.com/community/UFW

# Configuration
* Set firewall to allow only 2200 (ssh), 80 (http), and 123 (ntp).
* Added photogallery.conf to sites-enabled for apache2
* Set .git directory to `Deny from all` in photogallery.conf.
* Create postgres user 'catalog' and set as owner of database 'catalog.'
