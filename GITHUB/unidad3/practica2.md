# UD3. Gestió d'arxius web · Pràctica G1
**Alumne/a:** Anthony Hernandez 

## 1. Variació
- Port:
- Projecte:
- Adreça de la MV:

## 2. Pràctica: Pràctica G1 · NEXTCLOUD
amb Compose (30 min)
(ordres i les seues eixides)

Al diari: L'eixida de docker compose config --quiet && echo 'compose OK' 
![Captura 1](capturas/1.practica2)

Al diari: L'eixida de docker compose ps.
![Captura 2](capturas/2.practica2)

Al diari: L'eixida de docker compose exec -u www-data app php occ status.
![Captura 3](capturas/3.practica)

Al diari: El missatge exacte que apareix.
![Captura 4](capturas/4.practica2)

Al diari: L'eixida de docker compose exec -u www-data app php occ
config:system....
![Captura 5](capturas/5.practica2)

Al diari: Captura de la pàgina d'inici de sessió amb la teua IP i port, el missatge
de domini no fiable, eixida de docker compose ps i de occ status (sense
contrasenyes).
![Captura 6](capturas/6.practica2)



## 3. Errors i com els he resolt
Ha ido toda la practica bien, no he tenido problemas

## 4. Respostes
a) ${NC_PORT}:80 indica que el puerto definido en la variable NC_PORT de nuestro ordenador se conecta al puerto 80 del contenedor, donde funciona Nextcloud.

b) Los archivos se guardan en un volumen de Docker. Así no se pierden aunque eliminemos el contenedor, porque los datos están guardados fuera de él.

c) Porque los dos contenedores necesitan acceder a la misma base de datos. La contraseña la leen del archivo .env.

d) Porque .env contiene datos privados, como contraseñas y configuraciones, y no queremos que se publiquen en GitHub.

e) Para evitar que personas accedan a Nextcloud desde dominios desconocidos o no autorizados. Así solo permite conexiones desde dominios de confianza.





## 5. Estat final
(eixida de docker compose ps)

![Captura 6](capturas/7.practica2)