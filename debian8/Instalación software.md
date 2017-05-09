## Sublime Text 3
<http://docs.sublimetext.info/en/latest/getting_started/install.html>

Versión de 64 bits

1. Bajamos el software de https://www.sublimetext.com/3 o mediante el comando wget:
```
joseliza@PC-Lizana:~$ wget http://c758482.r82.cf2.rackcdn.com/sublime_text_3_build_3083_x64.tar.bz2
```

2. Descomprimimos.
```
joseliza@PC-Lizana:~$ tar vxjf sublime_text_3_build_3083_x64.tar.bz2
```

3. Now we should move the uncompressed files to an appropriate location.
```
joseliza@PC-Lizana:~$ sudo mv Descargas/sublime_text_3 /opt/
```
4. Lastly we create a symbolic link to use at the command line.
```
joseliza@PC-Lizana:~$ sudo ln -s /opt/sublime_text_3/sublime_text /usr/bin/sublime
```
5. Para crear el lanzador.
```
joseliza@PC-Lizana:~$ sudo ln -s /opt/sublime_text_3/sublime_text.desktop sublime_text.desktop
```
Será necesario editar el archivo */opt/sublime_text_3/sublime_text.desktop* para cambiar la ruta por defecto al archivo ejecutable que viene como *sublime_text* a la ruta correcta que hemos puesto que es *sublime_text_3*. Si tenemos problema con el icono usado, deberíamos comprobar la ruta y poner */opt/sublime_text_3/Icon/48x48/sublime-text.png*

## Foxi (Alternativa a Adobe Acrobat Reader)
<https://www.foxitsoftware.com/products/pdf-reader/>

Versión de 64 bits
Podemos hacer la instalación sin ser root. Si por el contrario queremos que la instalación sea para todos los usuarios debemos hacerla como superusuario. Yo la he hecho sólo para el usuario *joseliza*.
1. Change to the directory containing the downloaded file (used /tmp as the example):
```
joseliza@PC-Lizana:~$ cd /tmp
```
2. Uncompress the executable:
```
joseliza@PC-Lizana:~$ gzip -d 'FoxitReader_version_Setup.run.tar.gz'
```

3. Untar the .tar file
```
joseliza@PC-Lizana:~$ tar xvf 'FoxitReader_version_Setup.run.tar'
```

4. Run the installer:
```
joseliza@PC-Lizana:~$ ./'FoxitReader_version_Setup.run'
```

Follow the steps on the screen to complete the installation
