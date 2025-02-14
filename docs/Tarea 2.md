# Tarea 2 

> Realizado por ORTIZ GONZALEZ Fernando

[TOC]

## Trabajo Local

1. Inicializa un nuevo repositorio Git en una carpeta llamada `"labdist"` y agrega los archivos proporcionados en el aula virtual. Renombra la rama master a `main` , si es necesario. Realiza el primer commit. Muestra el log del repositorio.

  ```bash
  git init
  git branch -M main
  git log
  git status
  git add .
  git commit -m "se agrega fichefo .gitignore"
  nano .gitignore
  git status
  git add .
  git commit -m "En .gitignore se agrega: README.md, LICENCE.txt, passwords.txt"
  git log --oneline
  
  
  ```

Se utiliza el Visual Studio Code como editor para los archivos .txt .css .html y la creación de ficheros para la tarea como `.gitignore` .

![image-20250214165543773](./Tarea%202.assets/image-20250214165543773.png)

![image-20250214171247995](./Tarea%202.assets/image-20250214171247995.png)

![image-20250214173713419](./Tarea%202.assets/image-20250214173713419.png)

![image-20250214174213758](./Tarea%202.assets/image-20250214174213758.png)

![image-20250214174327248](./Tarea%202.assets/image-20250214174327248.png)

2. ------

   Incluye un fichero `.gitignore` para que los ficheros `README.md`, `LICENCE.txt`  y `passwords.txt` sean ignorados por el control de versiones. Realiza el commit y muestra los logs del repositorio en una línea

   

![image-20250214174820675](./Tarea%202.assets/image-20250214174820675.png)

![image-20250214183021082](./Tarea%202.assets/image-20250214183021082.png)

3. ------

   En el repositorio, crea los archivos README.md , LICENCE.txt y passwords.txt con algún contenido. Muestra el estado del repositorio. Muestra el listado de archivos ignorados.

![image-20250214183753263](./Tarea%202.assets/image-20250214183753263.png)

4. ------

   Crea una rama `feature-estilos` . Cámbiate a ella.

   * Modifica el archivo `estilos.css` :

      * propiedad color del `body` y de `h2` : `#2a2a2a`
      * propiedad `background-color` de `header`y `footer`: `#2a75ff`

   * Comprueba el estado del repositorio. Añade los cambios, realiza un commit con el
     mensaje "actualizados estilos a azules"

     ```bash
     git branch feature-estilos
     git log --graph --oneline
     git checkout feature-estilos
     ls
     cd css/
     ls
     nano estilos.css
     git status
     git add .
     git commit -m "actualizados estilos a azules"
     git log --oneline
     
     
     ```

     ![image-20250214184819030](./Tarea%202.assets/image-20250214184819030.png)

     ![image-20250214185033916](./Tarea%202.assets/image-20250214185033916.png)

     ![image-20250214185204033](./Tarea%202.assets/image-20250214185204033.png)

     ![image-20250214185552740](./Tarea%202.assets/image-20250214185552740.png)

     ![image-20250214185827596](./Tarea%202.assets/image-20250214185827596.png)

     ![image-20250214190145565](./Tarea%202.assets/image-20250214190145565.png)

     ------

   5. Vuelve a la rama main . En el archivo index.html añade un comentario donde se indique tu nombre como autor de la página. Comprueba el estado del repositorio. Añade los cambios, realiza un commit con el mensaje ' añadido autor en index'. Muestra los logs del repositorio en una línea, gráficamente y con 'decoración'.

      ```bash
      git checkout main
      cd ..
      ls
      nano index.html
      git status
      git add index.html
      git commit -m "añadidio autor en index.html"
      git log --graph --oneline --decorate --all
      ```

      ![image-20250214190741027](./Tarea%202.assets/image-20250214190741027.png)

      ![image-20250214192157081](./Tarea%202.assets/image-20250214192157081.png)

6. ------

   Fusiona la rama `feature-estilos` en la rama `main` . Muestra los logs del repositorio en una línea, gráficamente y con 'decoración'.

   ```bash
   git merge feature-estilos
   git log --graph --oneline --decorate --all
   ```

![image-20250214192837869](./Tarea%202.assets/image-20250214192837869.png)

------



## Trabajo Remoto

1. Continúa con el repositorio labdist . Añade el repositorio a Sourcetree

![image-20250214201118991](./Tarea%202.assets/image-20250214201118991.png)

2. En tu cuenta de GitHub, crea un repositorio remoto y sube al remoto los ficheros de tu repositorio local. Debes subir todas las ramas. Muestra, además, la captura de pantalla donde se vean en GitHub, algo similar a esto:

   

   ![image-20250214204525227](./Tarea%202.assets/image-20250214204525227.png)

![image-20250214204909503](./Tarea%202.assets/image-20250214204909503.png)

![image-20250214205008108](./Tarea%202.assets/image-20250214205008108.png)

4. En el repositorio local, crea una rama ``feature-index`` . Añade el siguiente código dentro de la <section class="about"> . Añade los cambios y crea un ``commit``con el mensaje "Añadido párrafo equipo en index.html". Sube los cambios al remoto. (Recuerda que debes usar SourceTree en todo este apartado )

![image-20250214205235053](./Tarea%202.assets/image-20250214205235053.png)

![image-20250214213548347](./Tarea%202.assets/image-20250214213548347.png)

![image-20250214213709472](./Tarea%202.assets/image-20250214213709472.png)

![image-20250214213829498](./Tarea%202.assets/image-20250214213829498.png)

5. En el repositorio local, fusiona la rama ``feature-index`` en la rama ``main`` .

   ![image-20250214214424821](./Tarea%202.assets/image-20250214214424821.png)

6. Edita el fichero ``contacto.html`` . Borra unas líneas. Muestra los ficheros con cambios pendientes y las diferencias. Añade los cambios y haz un ``commit``.

![image-20250214214905335](./Tarea%202.assets/image-20250214214905335.png)

7. Te das cuenta del error. Deshaz TOTALMENTE el ``commit`` anterior. Captura el estado actual del repositorio. (Asegúrate de que el fichero ``contacto.html`` ha recuperado todas las líneas borradas y no hay cambios pendientes en el repositorio.)

   ![image-20250214215155532](./Tarea%202.assets/image-20250214215155532.png)

8. Crea una rama ``feature-mapa`` y cámbiate a ella. Incluye este código en el archivo ``contacto.html`` . Añade los cambios. Realiza un ``commit``.