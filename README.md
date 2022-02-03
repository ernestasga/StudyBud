<div align="center">
<img width="30%" src="https://user-images.githubusercontent.com/72341453/134747028-7e2d90cc-a92f-4f66-815e-54a0d50cca54.PNG">

# Portfolio App with Django framework
</div>
<hr>

I built this app by following a video tutorial in order to familiarize myself Django framework.
https://www.youtube.com/watch?v=PtQiiknWUcI

### My changes to the oiginal project:
 > * Using postgress database instead of SQLite
 > * Dockerized the project

 ### What I learnt:
 > * Basic structure of django application
 > * MVT architecture model
 > * Install an html theme to django
 > * Writing an API with django

 ### What could be improved:
 > * Implement redis caching

 ## Setup
 1. Clone the repository
 > git clone https://github.com/ernestasga/StudyBud
 
 > cd ./StudyBud
 2. Build and start docker image
 > docker-compose up

 3. Open a session withthe app container
 >  docker exec -it studybud-studybud-1 bash

 4. Migrate the database
 > python manage.py migrate

 5. Create superuser
 > python manage.py createsuperuser

 6. Access the app at http://127.0.0.1 or admin panel at http://127.0.0.1/admin

 ### App Preview :

<table width="100%"> 
<tr>
<td width="50%">      
&nbsp; 
<br>
<p align="center">
  Feed Home
</p>
<img src="https://user-images.githubusercontent.com/72341453/134747262-0a92233d-8010-40f8-84c5-8d94895aac44.PNG">
</td> 
<td width="50%">
<br>
<p align="center">
  Room Conversation Preview
</p>
<img src="https://user-images.githubusercontent.com/72341453/134747155-3ca5b55f-b064-4741-aeae-abe90bddf41e.PNG">  
</td>
</table>
