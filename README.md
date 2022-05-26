# sqldatabase

**Install PostgreSQL on your machine, see https://www.postgresql.org/download/**

*[Assuming Ubuntu]*

**Basic commands**

  *Run PostgreSQL:* sudo -i -u postgres
  *Exit:* exit  
  
  *To connect to the database:* psql
  
  *Quit:* \q
  
  More: https://duckduckgo.com/?t=ffab&q=postgresql+commands&ia=answer&iax=answer
  
  **Load sample database**
  
  *Copy database zip archive to /var/lib/postgresql (or respected location on your machine; to find out necessary location use ls command while running postgres)*
  
  sudo -i -u postgres
  
  unzip dvdrental.zip
  
  psql
  
  create database dvdrental;
  
  pg_restore --dbname=dvdrental --verbose dvdrental.tar
  
  psql
  
  \c dvdrental
  
  **Test:** select * from film;
