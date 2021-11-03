# python-api-rest-heroku
Ejemplo api rest heroku usando python

###### DESPLIEGUE EN HEROKU
Necesitaremos 4 archivos

- index.py (código fuente de la api-restful)

- Procfile (despliega un servidor gunicorn apuntando a index.py

     

> web: gunicorn -b 0.0.0.0:$PORT index:app


- requeriments.txt (define las dependencias  a instalar en el cloud via pip)

> Flask #framework para desarrollo de la api 
> 
> gunicorn #servidor http


- runtime.txt define versión de python

> python-3.10.0
