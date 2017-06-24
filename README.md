# Linux Project
## Final project for Udacity Linux project

This repository is prepared for submission of the Linux course project.

The server is deployed in Amazon with the following details:
- IP Address: 35.158.94.64
- SSH Port: 2200
- URL: http://ec2-35-158-94-64.eu-central-1.compute.amazonaws.com/

## Summary of installed software
- Apache2
- Flask
- PostgreSQL
- Updated all the installed packages
- Mod_WSGI

## Summary of the special configuration changes
- Initially I did modifications to the UFW Firewall as required and added the Grader user as required.
- Then I installed all the software as indicated above.
- I added a virtual host to Apache and and condifured the WSGI to point to my application.
- I installed a basic sample Flask app (as indicated here) and later added my own project.
- Added a user to PostgreSQL and created a new DB.
- Modifed my Python project to use PostgreSQL instead of SQLite. As the project used SQLAlchemy this was very simple.
- Modifed all files access in my Python project to full path (/var/www/FlaskApp ...). This includes the Google secrets file, images folder and more.
- Updated the allowed URL/Server sources in both Google Oauth setup and Facebook Oauth setup to enable the looging through both of these systems.

## Third party sources I used
- The Udacity Forum and Stackoverflow (while Googling it).
- Used also turorials from DigitalOcean here https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
- Used Google several times while searching for specific Ubuntu commands which I couldn't figure out (can't really remember all sources exactly ...)


