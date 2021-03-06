afterlogic/docker-webmail-pro
=============================

Out-of-the-box [AfterLogic WebMail Pro](http://www.afterlogic.com/webmail-client) image

Includes Apache, MySQL and PHP setup based on [tutum/lamp package](https://github.com/tutumcloud/lamp)


Creating the image
------------------

	docker build -t afterlogic/docker-webmail-pro .


Running docker image
--------------------

Start your image binding the external port 80:

	docker run -d -p 80:80 afterlogic/docker-webmail-pro

and access the container via web browser at http://localhost/


Alternately, you can use any other port available, e.g. 800:

	docker run -d -p 800:80 afterlogic/docker-webmail-pro

and access the installation at http://localhost:800/


Accessing AdminPanel Interface
------------------------------

To configure WebMail Pro installation, log into AdminPanel interface using URL like http://localhost/adminpanel/

Default credentials are set to **mailadm** / **12345**


Licensing Terms & Conditions
----------------------------

Content of this repository is available in terms of [AGPLv3 license](http://www.gnu.org/licenses/agpl-3.0.en.html) (see `LICENSE` file)