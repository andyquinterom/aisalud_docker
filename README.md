# Dockerfile para correr Analítica Integrada Salud.

Para compilar la imagen se debe utilizar el siguiente comando:

```bash
docker build -t aisalud:21.07.1 - < Dockerfile
```

Para correr la aplicación se deben pasar las variables de ambiente
de la siguiente manera:

```bash
docker run -p 3838:3838 -e DATABASE_USER='...' \
    -e DATABASE_NAME='...' \
    -e DATABASE_HOST='...' \
    -e DATABASE_PW='...' \
    aisalud
```
