## <center> ACTIVIDAD 1</center>
### <center>Instalación de WSL</center>
1. Comando **sudo**: es la abreviatura de super usuario, permite realizar tareas
   con permisos de root (máxima autoridad en el computador), todo comando
   que sea antecedido por sudo se ejecutará con privilegios elevados.

    ```bash
    # Crear directorio con privilegios root
    sudo mkdir /opt/taller_wls
    ```
    ![Comando sudo](img\taller_punt_1.png)

2. **Pwd**: permite conocer cuál es la ruta de trabajo actual (carpeta en la 
   que nos encontramos)
    ```bash
    # Conocer ruta 
    pwd
    ```
    ![Comando pwd](img\taller_punto_2.png)

3. **cd** es el comando para navegar entre carpetas desde la terminal, permite
   movernos a diferentes directorios, por ejemplo cd /home, o cd /usr , al
   ejecutarlos veremos cómo la ruta en la consola cambia. Para subir un
   directorio podemos emplear el comando cd ..

   ```bash
   # Comando cd .. para subir un directorio
   cd ..

   # Comando cd paranavegar a otro directorio
   cd /opt/taller_wsl/
   ```
   ![Comando cd & cd ..](img\taller_punto_3.png)

4. **ls** permite listar los archivos y carpetas dentro de un directorio, se 
   le pueden agregar opciones, por ejemplo ls -l permite ver en forma de lista 
   o **ls -la** los publica en forma de lista y muestra archivos ocultos. En Linux los archivos ocultos son aquellos cuyo nombre empieza con un punto. Para listar
   directorios con subdirectorios y contenidos se puede emplear **ls -R**
   (recursivo).

   ```bash
   # Listar directorios en /var
   ls -ltr /var/
   ```
   ![Comando ls](img\taller_punto_4.png)

5. **cat:** este comando permite imprimir en la salida estándar (consola) el
   contenido de los archivos. Es útil para visualizar rápidamente archivos y
   configuraciones.

   ```bash
   # Imprimir salida de archivo hosts
   cat /etc/hosts
   ```
   ![Comando cat](img\taller_punto_5.png)

6. **cp:** permite copiar un archivo en otro, por ejemplo
   cp nombrearchivo1.txt nombrearchivo2.txt nombrearchivo3.txt
   /inicio/nombredeusuario/Documentos.

   ```bash
   # Copiar archivo
   sudo cp archivo.txt archivo_copy.txt
   ```
   ![Comando cp](img\taller_punto_6.png)

7. **mv:** permite mover archivos de un lugar a otro.

   ```bash
   # Mover archivo de /opt/taller_wsl a /home/master
   sudo mv archivo_copy.txt /home/master/archivo_copy.txt
   ```
   ![Comando mv](img\taller_punto_7.png)

8. **mkdir:** crea directorios, por ejemplo mkdir micarpeta crearía una carpeta
   llamada micarpeta.

   ```bash
   # Crear directorio 
   sudo mkdir script
   ```
   ![Comando mkdir](img\taller_punto_8.png)

9. **Touch:** permite crear archivos vacíos, por ejemplo touch holamundo.py, si
   inmediatamente después se usa el comando ls se puede apreciar el
   archivo holamundo.py creado.

   ```bash
   # Crear archivo .py 
   sudo touch script/main.py
   ```
   ![Comando touch](img\taller_punto_9.png)

10. **Top:** permite ver los procesos en ejecución con su consumo de recursos,
    para salir se debe pulsar escape o q.

   ```bash
   # Ver procesos en ejecución 
   top
   ```
   ![Comando top](img\taller_punto_10.png)

11. Crear y ejecutar un hola mundo con **python**.
    
   ```bash
   # Editar archivo main.py 
   sudo vim /opt/taller_wsl/script/main.py

   # Agregar hola mundo guardar y salir
   print("Hola mundo...")

   # Ejecutar main.py
   python3 main.py

   ```
   ![Comando top](img\taller_punto_11.png)