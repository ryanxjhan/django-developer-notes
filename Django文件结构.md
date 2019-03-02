# 1.0 Django文件结构
`留言板项目`
## Defualt Files
- __init__.py
使目录模块化
- settings.py
核心配置文件：数据库，Web app，时间等
  - BASE_DIR: source root
  - SECRET_KEY
  - DEBUG
  - ALLOWED_HOSTS:
  - INSTALLED_APPS: 保存所有默认和自定义应用名字
  - MIDDLEWARE
  - ROOT_URLCONF:
  - TEMPLATES
  - DATEBASES
  - INTERNALIZATION
  - STATIC URL: 静态文件地址
- urls.py
配置URL：每个页面的地址
- wsgi.py
Python Web Server Gateway Interface
服务器网关接口
与服务器之间的接口：使服务器识别Django网站
不会用到
- templates
stores html files 
- manage.py
command-line utility for administrative tasks

## Project Files 
-  log
-  media
user-uploaded media
-  static
stores html/css js files 
-  message ([2. Create an App](:note:6a1cff1c-fd9f-4b75-aff7-4476b68deb62))
the app itself

## Tips
1. Set the app folder as source root to avoid repeated long path names
2. Also need to set this in settings.py.