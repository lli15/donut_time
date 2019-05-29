# 𝓭𝓸𝓷𝓾𝓽 𝓽𝓲𝓶𝓮  🍩
Kenny Li(PM), Jiayang Chen, Dennis Chen, Johnson Li

P #05: Fin

# Donut Drawing
## Description
Donut Drawing is a layer-based web drawing program similiar to [Aggie.io](https://aggie.io/) or Adobe Photoshop. Users will have several tools such as pencil, paintbrush, paint bucket, eraser, smudge, eye dropper, ellipse, rectangle, and crop. Modifiers can be applied to these tools such as color, brush size, opacity, and brightness. Filters can also be applied to the canvas directly. Users may save their work by making an account and storing it or downloading it locally to their computer.

## Launch Codes
### Requirements
Our dependencies, as listed in requirements.txt, are as follows:

| Dependency | Version | Origin | Description | 
| --- | --- | --- | --- |
| Click | 7.0 | Flask | dependency for flask |
| Flask | 1.0.2 | Flask | microframework of choice |
| itsdangerous | 1.1.0 | Flask | dependency for flask |
| Jinja2 | 2.10 | Flask | templating language |
| MarkupSafe | 1.1.1 | Flask | dependency for flask |
| Werkzeug | 0.15.1 | Flask | dependency for flask |

### Install and run on localhost
1. Clone the repo via ssh or https
   - SSH: ```git clone git@github.com:lli15/donut_time.git```
   - HTTPS: ```git clone https://github.com/lli15/donut_time.git```
2. **(Optional)** Make and activate virtual environment
```
python3 -m venv <venv_name>
. <path-to-venv>/bin/activate
```
3. Enter the repo directory
```
cd <path-to-repo>
```
4. Install requirements
   - Python 3.7: ```pip3 install -r requirements.txt```
   - If in virtual environment with Python 3.7: ```pip install -r requirements.txt```
5. Run app.py
   - Python 3.7: ```python3 app.py```
   - If in virtual environment with Python 3.7: ```python app.py```
6. Go to http://127.0.0.1:5000/ on any browser

### Install and run on Apache2
1. SSH into your droplet:
```ssh <user>@<ip address>```
2. Move to the www directory:
```cd ../../var/www```
3. Get root access:
```sudo su```
4. Clone the repo via https:
```git clone https://github.com/lli15/donut_time.git```
5. Move into the repo, add write permisssions, and install requirements:
```
cd donut_time
chgrp -R www-data donut_time
chmod -R g+w donut_time
pip3 install -r requirements.txt
```
8. Move the conf file to the sites-enabled directory:
```mv donut_time.conf ~/../../etc/apache2/sites-enabled/```
9. Enable the site:
```a2ensite <appname>```
10. Reload and restart the server
```
service apache2 reload
service apache2 restart
```
11. Go to your ip address on any browser
