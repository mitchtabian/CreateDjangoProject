# CreateDjangoProject
How to start a Django project from scratch
<h4>Starting a new Django Project (Windows)</h4>
<ol>
<li>
Installing Python
<ol>
<li>Download the version of Python you need <a href='https://www.python.org/downloads/'>here</a></li>
<li>After Python is finished installing, make sure the path to the Scripts folder is added to Environment Variables PATH. It should do it
automatically but it's better to double check. My path looks like this: 'F:\Python\Python35\Scripts'</li>
<li>Check to see if Python installed correctly by opening a command prompt and typing: "python3 –version". You should see something like
this: 
<pre><code>Python 3.6.1</code></pre></li>
</ol>
</li>
<li>
Update Pip
<ol>
<li>Pip should be installed already but you'll have to update it. Open a command prompt and type: 
<pre><code>python -m pip install -U pip setuptools</pre></code></li>
</ol>
</li>
<li>
Install Virtual Environment
<ol>
<li>You need to install a virtual environment tool for developing. In the command prompt type: 
<pre><code>pip install virtualenv</pre></code></li>
</ol>
</li>
<li>
Install Django Web Framework
<ol>
<li>For documentation check out "https://docs.djangoproject.com". To install Django type: 
<pre><code>pip install django==1.10</pre></code>
Use 1.10 since thats what I'm using and it will be a long-standing version. </li>
</ol>
</li>
<li>
Create Virual Environment
<ol>
<li>Navigate to the directory you want to keep your django projects. I just use: "F:\PyCharmProjects" because the IDE I use to
write code is PyCharm. There are many code editors but PyCharm has a free version so I use that.<br/>
To create a Virtual Environment navigate to the directory where you want your project and open a command prompt there.Type:
<pre><code>virtualenv {project_name}</pre></code> Obviously without the '<' and '>'.</li>
</ol>
</li>
<li>
Start the Virtual Environment
<ol>
<li>To activate the virtual environement first navigate into it by typing: <pre><code>cd project_name</pre></code> Then start
the Virtual Environment by typing: <pre><code>Scripts/activate</pre></code>  You'll see the name of it encapsulated in brackets 
in the command prompt if you did it correctly. Now we have an isolated environment to develop in.</li>
</ol>
</li>
<li>
Create the django project
<ol>
<li>To create a new Django Project type: <pre><code>django-admin startproject django_project</pre></code> It might take 30 
seconds or so to start the project. Once it's done open the directory in PyCharm or whatever code editor your using.</li>
</ol>
</li>
<li>
Run the Server
<ol>
<li> navigate into the 'django_project' directory by typing <pre><code>cd django_project</pre></code><br/>Once inside type: 
<pre><code>python manage.py runserver</pre></code> Your server will start. Now open a web browser and type: 
"http://127.0.0.1:8000/" in the URL bar. If it's working it will say: "It worked! Congratulations on your direct Django-powered
page." in the web browser.</li>
</ol>
</li>
</ol>
