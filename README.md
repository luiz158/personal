Arquivos e dicas para facilitar configurações de ambiente de desenvolvimento

===
### Windows Hack para facilitar o uso do django-admin
> * Criar um arquivo django-admin.bat para chaamr o django-admin.py
> * Criar essa .bat dentro do diretório "%VIRTUAL_ENV%"\Scripts
```
@python "c:\Python27\path\venv\Scripts\django-admin.py" %* 
```   
exemplo:      
```
$ django-admin startproject project_name .
```

===

### Executar o manage.py de qualquer diretório dentro do virtualenv
> No Windows
* Crie o arquivo "%VIRTUAL_ENV%"\Scripts\manage.bat    
```
@python "c:\Python27\path_project\manage.py" %* 
```       
> exemplo:               
```
$ manage help
```      

---
> No Mac ou Linux
* Crie um alias no seu ~/.bashrc ou ~/.profile       
```
alias manage='python $VIRTUAL_ENV/manage.py'
```       
> exemplo:               
```
$ manage help
```
