
#### 1.在shell运行
```
jupyter --paths
```
查看.jupyter目录下是否有
```
jupyter_notebook_config.py
```
如果没有，shell运行
```
jupyter notebook --generate-config
```
生成
```
jupyter_notebook_config.py
```
然后
```
vim jupyter_notebook_config.py
```
修改
```
#c.NotebookApp.base_url = '/'
```
为
```
c.NotebookApp.base_url = '/jupyter/{your_name}/'
```
并加入账号密码等
```
## notebook服务会监听的IP地址.
c.NotebookApp.ip = '*'
#  The string should be of the form type:salt:hashed-password.
c.NotebookApp.password = 'sha1:fcc2ed1c007d:d27f6332ba2903b2526918274dab19e230e7351e'
c.NotebookApp.open_browser = False
## notebook服务会监听的IP端口.
c.NotebookApp.port = 8187
```
#### 2.在shell运行如下命令启动jupyter即可：
```
jupyter notebook --ip 0.0.0.0 --port 8187
```
在网站：
即可看到界面
