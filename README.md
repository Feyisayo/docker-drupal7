This is the base docker-compose I use for Drupal 7 sites. It contains images for apache-php, mysql and mailhog.

**How To Use**

- Install docker-compose. See https://docs.docker.com/compose/
- Download the latest version of Drupal 7 from https://drupal.org and put the Drupal files in the `src` folder
- Run `docker-compose up -d` and voila!! you're good to go
- In your browser go to http://localhost
- During the Drupal installation the specify `mysql-server` as the database server
- You can also add an entry to your hosts files (that's at `/etc/hosts` on debian-based systems) to customize the URL for the Drupal site. The default friendly name is `drupal7.local`. You can change this from the apache configuration file at `includes/000-default.conf`
- Access the mailhog app by going to http://localhost:8025

