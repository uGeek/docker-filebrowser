# Filebrowser para ARM

```
docker run --name filebrowser \
    -v  /data:/srv \
    -v  $PWD/filebrowser.db:/database.db \
    -v  $PWD/filebrowser.json:/.filebrowser.json \
    -p  80:80 \
    filebrowser/filebrowser:pi
```


# Filebrowser para amd64

```
docker run --name filebrowser \
    -v  /data:/srv \
    -v  $PWD/filebrowser.db:/database.db \
    -v  $PWD/filebrowser.json:/.filebrowser.json \
    -p  80:80 \
    filebrowser/filebrowser
```

- Username: admin
- Password: admin

**Si da error el arranque del docker, crea una nueva base de datos en blanco filebrowser.db**

- Fuente: https://filebrowser.org/installation
