# EVIDENCIAS DE JOEL

## ENCARGO 1: PAGINA ESTATICA

### INSTALAR APACHE 2

```bash
sudo apt install apache2

sudo systemctl status apache2

apache2.service - The Apache HTTP Server
    Loaded: loaded (/usr/lib/systemd/system/apache2.service; enabled; preset: enabled)
    Active: active (running) since Mon 2026-10-26 16:28:49 CET; 29s ago

sudo ufw allow 'Apache'
Rule added
Rule added (v6)
```

## ENCARGO 2: PORTAL DINAMICO CON PHP

### EJECUTAR PHP

```bash
sudo apt install php-fpm

php -S localhost:8090
```

## ENCARGO 3: DATOS Y CLASIFICACION

### INSTALAR MARIA DB

```bash
sudo apt install mariadb-server

sudo mariadb-secure-installation

sudo systemctl start mariadb
sudo systemctl status mariadb

mariadb -u root -p
```

### BBDD

He descargado la extension de MySQL en VSCode

Despues se ha creado la bbdd en el mariadb

Se han introducido las tablas y valores

Y se ha creado la conexion a la bbdd desde la extension

## ENCARGO 4: APLICACION JAVA

### INSTALAR TOMCAT

```bash
sudo apt install -y openjdk-21-jdk

java -version

sudo useradd -m -U -d /opt/tomcat -s /bin/false tomcat
```

#### CREAMOS UN USUARIO ESPECIFICO PARA TOMCAT

```sql
CREATE USER 'java_user' @'localhost' IDENTIFIED BY 'Java1234';
GRANT ALL PRIVILEGES ON puntdejoc.* TO 'java_user' @'localhost';
FLUSH PRIVILEGES;
```
