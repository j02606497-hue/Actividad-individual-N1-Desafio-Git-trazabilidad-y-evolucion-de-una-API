# DESAFIO 1


---


### Estudiante

Juan Jose Pareja Ruiz


### Universidad

Universidad de Manizales  


### Facultad

Facultad de Ciencias e Ingeniería


### Programa Academico

Programa de Ingeniería de Sistemas Virtual


### Curso

Programacion V 


### Profesor

Carlos Alberto Gutierrez Rodas


---


## Comandos utilizados

## 1. Navegación al directorio del proyecto 

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia> cd ProgramacionV.Api

- Respuesta: Permite ingresar al directorio específico del proyecto. Esto establece la ubicación de trabajo desde la cual se ejecutarán las operaciones posteriores de Git y .NET.

```


## 2. Creación del archivo .gitignore

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> dotnet new gitignore

- Resultado: La plantilla "archivo gitignore de dotnet" se creó correctamente.

- Respuesta: Crea correctamente el archivo .gitignore mediante la plantilla proporcionada por .NET. El resultado confirma que la plantilla fue generada sin errores.

```


## 3. Inicializar el repositorio

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git init -b main

- Resultado: Initialized empty Git repository in C:/Users/juanj/OneDrive/Desktop/ProgramacionV - copia (2) - copia/ProgramacionV.Api/.git/

- Respuesta: Inicializa un nuevo repositorio Git y establece main como rama inicial. El resultado confirma que el repositorio vacío fue creado correctamente dentro del directorio del proyecto.

```


## 4. Verificar

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git status

- Resultado: 

On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        Controllers/
        Data/
        Migrations/
        Models/
        Program.cs
        ProgramacionV.Api.csproj
        ProgramacionV.Api.http
        Properties/
        Repositories/
        WeatherForecast.cs
        appsettings.Development.json
        appsettings.json
        programacionv.db

nothing added to commit but untracked files present (use "git add" to track)

- Respuesta: Confirma que el repositorio está en la rama main, aún no tiene commits y contiene archivos sin seguimiento. Esto permite verificar el estado inicial antes de agregar los archivos al control de versiones.

```


## 5. Commit inicial C1 en main

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git add .

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git commit -m "C1: commit inicial en main"

- Resultado: 

[main (root-commit) 25b67c8] C1: commit inicial en main
 20 files changed, 1408 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 Controllers/EstudiantesController.cs
 create mode 100644 Controllers/ProgramasController.cs
 create mode 100644 Controllers/WeatherForecastController.cs
 create mode 100644 Data/AppDbContext.cs
 create mode 100644 Migrations/20260828214724_InitialCreate.Designer.cs
 create mode 100644 Migrations/20260828214724_InitialCreate.cs
 create mode 100644 Migrations/AppDbContextModelSnapshot.cs
 create mode 100644 Models/Estudiante.cs
 create mode 100644 Models/ProgramaAcademico.cs
 create mode 100644 Program.cs
 create mode 100644 ProgramacionV.Api.csproj
 create mode 100644 ProgramacionV.Api.http
 create mode 100644 Properties/launchSettings.json
 create mode 100644 Repositories/EstudianteRepository.cs
 create mode 100644 Repositories/ProgramaRepository.cs
 create mode 100644 WeatherForecast.cs
 create mode 100644 appsettings.Development.json
 create mode 100644 appsettings.json
 create mode 100644 programacionv.db

- Respuesta: Los comandos git add . y git commit agregan todos los archivos del proyecto y crean el commit inicial C1 en main. El resultado confirma que se registraron 20 archivos y que el commit quedó identificado con el hash corto 25b67c8.

```


## 6. Crear feature/telefono-estudiante desde main

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git checkout -b feature/telefono-estudiante

- Resultado: Switched to a new branch 'feature/telefono-estudiante'

- Respuesta: El comando crea la rama feature/telefono-estudiante a partir de la rama actual main. El resultado confirma que la nueva rama fue creada correctamente y que Git cambió a ella.

```


## 7. Hacer un cambio y crear C2

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> "Cambios relacionados con telefono del estudiante" > feature-telefono-estudiante.txt

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git add .

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git commit -m "C2: cambios en feature/telefono-estudiante"

- Resultado: 

[feature/telefono-estudiante e7a98a2] C2: cambios en feature/telefono-estudiante
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feature-telefono-estudiante.txt

- Respuesta: Se crea feature-telefono-estudiante.txt, se agrega al área de preparación y se registra mediante el commit C2. El resultado confirma que el archivo fue creado y que C2 quedó identificado con el hash corto e7a98a2.

```


## 8. Crear feature/validar-telefono desde feature/telefono-estudiante

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git checkout -b feature/validar-teléfono

- Resultado: Switched to a new branch 'feature/validar-telefono'

- Respuesta: El comando crea una nueva rama a partir de la rama actualmente activa, feature/telefono-estudiante. El resultado confirma que la rama feature/validar-telefono fue creada correctamente y quedó seleccionada.

```


## 9. Hacer un cambio y crear C4

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> "Validacion de formato de telefono" > feature-validar-telefono.txt

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git add .

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git commit -m "C4: cambios en feature/validar-telefono"

- Resultado: 

[feature/validar-telefono 6a59a99] C4: cambios en feature/validar-telefono
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feature-validar-telefono.txt

- Respuesta: Se crea feature-validar-telefono.txt, se agrega al seguimiento y se registra mediante el commit C4. El resultado confirma que el archivo fue creado y que C4 quedó identificado con el hash corto 6a59a99.

```


## 10. Volver a main y crear feature/consulta-estudiantes

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git checkout main

- Resultado: Switched to branch 'main'

- Respuesta: El comando git checkout main cambia correctamente desde la rama actual hacia main, dejando esta como rama activa. El resultado confirma que el cambio se realizó correctamente.

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git checkout -b feature/consulta-estudiantes

- Resultado: Switched to a new branch 'feature/consulta-estudiantes'

- Respuesta: El comando git checkout -b feature/consulta-estudiantes crea una nueva rama a partir de main y cambia automáticamente a ella. El resultado confirma que la rama feature/consulta-estudiantes fue creada y seleccionada correctamente.

```


## 11. Hacer un cambio y crear C3

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> "Consulta de listado de estudiantes" > feature-consulta-estudiantes.txt

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git add .

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git commit -m "C3: cambios en feature/consulta-estudiantes"

- Resultado: 

[feature/consulta-estudiantes bcbc34c] C3: cambios en feature/consulta-estudiantes
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feature-consulta-estudiantes.txt

- Respuesta: Se crea feature-consulta-estudiantes.txt, se agrega al área de preparación y se registra mediante el commit C3. El resultado confirma que el archivo fue creado y que C3 quedó identificado con el hash corto bcbc34c.


```


## 12. Visualizar el historial gráfico completo

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git log --all --graph --oneline --decorate

- Resultado: 

* bcbc34c (HEAD -> feature/consulta-estudiantes) C3: cambios en feature/consulta-estudiantes
| * 6a59a99 (feature/validar-telefono) C4: cambios en feature/validar-telefono
| * e7a98a2 (feature/telefono-estudiante) C2: cambios en feature/telefono-estudiante
|/  
* 25b67c8 (main) C1: commit inicial en main

- Respuesta: El resultado muestra los cambios realizados y cómo se fueron creando las diferentes ramas. Se puede ver que C1 fue el inicio y luego se crearon C2, C4 y C3 en sus respectivas ramas.

```


## 13. Hash + commit + rama

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git log --all --format="%h %s" --decorate

- Resultado: 

bcbc34c C3: cambios en feature/consulta-estudiantes
6a59a99 C4: cambios en feature/validar-telefono
e7a98a2 C2: cambios en feature/telefono-estudiante
25b67c8 C1: commit inicial en main

- Respuesta: El comando muestra los cuatro commits junto con sus hashes cortos y referencias de rama disponibles.

```


## 14. Hash corto de cada commit creado

```bash

Commit	Hash corto
C1	25b67c8
C2	e7a98a2
C4	6a59a99
C3	bcbc34c

- Respuesta: La tabla registra el hash corto correspondiente a cada commit creado durante el desafío. Los valores coinciden con los identificadores observados en el historial gráfico: C1 25b67c8, C2 e7a98a2, C4 6a59a99 y C3 bcbc34c.

```


## 15. Nombre de la rama en la que se realizó cada commit

```bash

Commit	Rama
C1	main
C2	feature/telefono-estudiante
C4	feature/validar-telefono
C3	feature/consulta-estudiantes

- Respuesta: La tabla identifica la rama asociada a cada commit según la secuencia de operaciones realizada. C1 pertenece a main, C2 a feature/telefono-estudiante, C4 a feature/validar-telefono y C3 a feature/consulta-estudiantes.

```


## 16. Explicación por qué feature/validar-telefono se origina desde feature/telefono-estudiante y no desde main

- Respuesta: feature/validar-telefono se creó mientras feature/telefono-estudiante estaba activa, por lo que heredó su historial y el commit C2. Esto permite que la validación se construya sobre los cambios previamente realizados en la funcionalidad de teléfono, en lugar de partir directamente de main.



---



# DESAFIO 2

## Comandos utilizados

## 1. Hash corto del commit donde se agregó el teléfono del estudiante

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git log --all --oneline -- feature-telefono-estudiante.txt

- Resultado: e7a98a2 (feature/telefono-estudiante) C2: cambios en feature/telefono-estudiante

- Respuesta: El hash corto del commit es e7a98a2, identificado en la rama feature/telefono-estudiante, Este commit corresponde a C2: cambios en feature/telefono-estudiante, donde se realizó el cambio relacionado con el teléfono del estudiante.

```


## 2. Quién realizó ese commit

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git show -s --format="Autor: %an <%ae>" e7a98a2

- Resultado: Autor: th3hu5tl30630-hub <th3hu5tl3.0630@gmail.com>

- Respuesta: El commit e7a98a2 fue realizado por th3hu5tl30630-hub, utilizando el correo th3hu5tl3.0630@gmail.com, Estos datos corresponden directamente al autor registrado por Git en ese commit.

```


## 3. Cuál fue el mensaje utilizado

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git show -s --format="Mensaje: %s" e7a98a2

- Resultado: Mensaje: C2: cambios en feature/telefono-estudiante

- Respuesta: El mensaje utilizado para identificar el commit fue “C2: cambios en feature/telefono-estudiante”, Este mensaje permite reconocer que el commit corresponde a los cambios realizados en la rama feature/telefono-estudiante.

```


## 4. En qué fecha fue realizado

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git show -s --format="Fecha: %ad" e7a98a2

- Resultado: Fecha: Sat Aug 29 10:40:05 2026 -0500

- Respuesta: El commit e7a98a2 fue realizado el 29 de agosto de 2026 a las 10:40:05, con zona horaria -0500, La fecha y hora corresponden al registro mostrado directamente por Git para ese commit.

```


## 5. Qué archivos fueron modificados en ese commit

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git show --stat e7a98a2

- Resultado: 

commit e7a98a242a71fe92caf8624094280ec6ba0298fb (feature/telefono-estudiante)
Author: th3hu5tl30630-hub <th3hu5tl3.0630@gmail.com>
Date:   Sat Aug 29 10:40:05 2026 -0500

    C2: cambios en feature/telefono-estudiante

 feature-telefono-estudiante.txt | Bin 0 -> 102 bytes
 1 file changed, 0 insertions(+), 0 deletions(-)

- Respuesta: En el commit e7a98a2 se modificó únicamente el archivo feature-telefono-estudiante.txt, Git registra 1 archivo cambiado, con un tamaño de 102 bytes, sin mostrar inserciones ni eliminaciones porque el archivo está registrado como binario.

```


## 6. Cuál fue el commit donde se implementó la validación del teléfono

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git log --all --oneline -- feature-validar-telefono.txt

- Resultado: 6a59a99 (feature/validar-telefono) C4: cambios en feature/validar-teléfono

- Respuesta: El commit donde se implementó la validación del teléfono es 6a59a99, ubicado en la rama feature/validar-telefono, Su mensaje es “C4: cambios en feature/validar-teléfono”, según el resultado mostrado por Git.

```



---



# DESAFIO 3

## Comandos utilizados

## 1. Confirmar la rama actual

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git Branch

- Resultado: 

* feature/consulta-estudiantes
  feature/telefono-estudiante
  feature/validar-telefono
  main

- Respuesta: La rama actual es feature/consulta-estudiantes, como indica el asterisco (*) en el resultado de git branch. También se muestran las ramas feature/telefono-estudiante, feature/validar-telefono y main.

```


## 2. Realizar la modificación intencional en Program.cs

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> Add-Content -Path Program.cs -Value "`n// Modificacion de prueba - Desafio 3"

- Respuesta: Se agregó al archivo Program.cs la línea // Modificacion de prueba - Desafio 3. Esta modificación se realizó intencionalmente para generar un cambio en el archivo y posteriormente recuperarlo.

```


## 3. Resultado antes de recuperar el archivo

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git status

- Resultado: 

On branch feature/consulta-estudiantes
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Program.cs

no changes added to commit (use "git add" and/or "git commit -a")

- Respuesta: Git detectó que Program.cs fue modificado, pero el cambio todavía no había sido preparado para un commit. El estado muestra que existen cambios sin agregar al área de preparación.

```


## 4. Resultado del comando que muestra las diferencias

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git diff Program.cs

- Resultado: 

warning: in the working copy of 'Program.cs', LF will be replaced by CRLF the next time Git touches it
diff --git a/Program.cs b/Program.cs
index 72d32f0..ad5e7ab 100644
--- a/Program.cs
+++ b/Program.cs
@@ -44,4 +44,5 @@ app.UseHttpsRedirection();
 
 app.MapControllers();
 
-app.Run();
\ No newline at end of file
+app.Run();
+// Modificacion de prueba - Desafio 3

- Respuesta: git diff Program.cs muestra que se agregó la línea // Modificacion de prueba - Desafio 3 después de app.Run();.

```


## 5. Comando utilizado para recuperar el archivo

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git checkout -- Program.cs

- Respuesta: El comando git checkout -- Program.cs se utilizó para descartar la modificación realizada en Program.cs. De esta manera, el archivo volvió al estado que tenía antes del cambio intencional.

```


## 6. Resultado final

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git status

- Resultado:

On branch feature/consulta-estudiantes
nothing to commit, working tree clean

- Respuesta: El resultado confirma que Program.cs ya no presenta modificaciones pendientes. La frase working tree clean indica que el área de trabajo quedó limpia y no hay cambios por confirmar.

```


## 7. ¿Qué habría ocurrido si el cambio ya hubiese sido incluido en un commit? 

- Respuesta: Si el cambio ya estuviera incluido en un commit, git checkout -- Program.cs no eliminaría ese cambio del historial confirmado. En ese caso, sería necesario utilizar otro comando para deshacer o revertir el commit según lo que se quisiera conservar.



---



# DESAFIO 4

## Comandos utilizados

## 1. Cambiar a la rama main

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git checkout main

- Resultado: Switched to branch 'main'

- Respuesta: Se cambió correctamente a la rama main, tal como confirma el mensaje Switched to branch 'main'. Esto permitió tomar main como punto de partida para crear la nueva rama de prueba.

```


## 2. Crear la rama feature/cambio-prueba desde main

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git checkout -b feature/cambio-prueba

- Resultado: Switched to a new branch 'feature/cambio-prueba'

- Respuesta: Se creó correctamente la rama feature/cambio-prueba y Git cambió automáticamente a ella. La nueva rama se creó tomando como base la rama main.

```


## 3. Realizar una modificación sencilla en Program.cs

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> Add-Content -Path Program.cs -Value "`n// Cambio de prueba - Desafio 4"

- Respuesta: Se agregó una modificación de prueba al archivo Program.cs, incorporando el comentario indicado. Este cambio quedó realizado en el archivo y preparado para posteriormente registrarlo mediante Git.

```


## 4. Agregar el cambio al staging

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git add .    

- Respuesta: El comando git add . se utilizó para agregar los cambios existentes al área de preparación. De esta manera, las modificaciones quedaron listas para formar parte del siguiente commit.                                   

```


## 5. Crear el commit original

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git commit -m "Cambio de prueba para Desafio 4"

- Resultado: 

[feature/cambio-prueba cc6d846] Cambio de prueba para Desafio 4
 1 file changed, 2 insertions(+), 1 deletion(-)

- Respuesta: Se creó correctamente el commit cc6d846 con el mensaje Cambio de prueba para Desafio 4. Git confirma que se modificó Program.cs, registrando los cambios realizados en la rama feature/cambio-prueba.

```


## 6. Registrar el hash del commit original

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git log -1 --oneline

- Resultado: cc6d846 (HEAD -> feature/cambio-prueba) Cambio de prueba para Desafio 4

- Respuesta: El comando muestra que el commit original tiene el hash corto cc6d846. Además, HEAD y la rama feature/cambio-prueba apuntaban en ese momento a dicho commit.

```


## 7. Ver historial antes de deshacer el commit (rama actual)

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git log --oneline

- Resultado: 

cc6d846 (HEAD -> feature/cambio-prueba) Cambio de prueba para Desafio 4
25b67c8 (main) C1: commit inicial en main

- Respuesta: El historial muestra que cc6d846 era el commit más reciente de feature/cambio-prueba. También confirma que su commit anterior era 25b67c8, correspondiente a main.

```


## 8. Ver historial antes de deshacer el commit (todas las ramas, gráfico)

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api>  git log --all --graph --oneline --decorate

- Resultado: 

* cc6d846 (HEAD -> feature/cambio-prueba) Cambio de prueba para Desafio 4
| * bcbc34c (feature/consulta-estudiantes) C3: cambios en feature/consulta-estudiantes
|/  
| * 6a59a99 (feature/validar-telefono) C4: cambios en feature/validar-telefono
| * e7a98a2 (feature/telefono-estudiante) C2: cambios en feature/telefono-estudiante
|/  
* 25b67c8 (main) C1: commit inicial en main

- Respuesta: El gráfico muestra que feature/cambio-prueba tenía el commit cc6d846 después de main. También permite observar que las demás ramas (consulta-estudiantes, validar-telefono y telefono-estudiante) conservaban sus propios commits.

```


## 9. Deshacer el commit conservando los cambios en los archivos

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git reset --soft HEAD~1

- Respuesta: Se ejecutó git reset --soft HEAD~1 para quitar el último commit de la historia sin eliminar los cambios realizados. Con esta opción, los cambios permanecen preparados para poder corregirlos y volver a confirmarlos.

```


## 10. Verificar el estado del repositorio después de la operación

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git status

- Resultado: 

On branch feature/cambio-prueba
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   Program.cs

- Respuesta: Git confirma que la rama actual es feature/cambio-prueba y que Program.cs tiene cambios preparados para ser confirmados. Esto demuestra que el commit anterior fue retirado, pero sus modificaciones se conservaron en staging.

```


## 11. Corregir/completar el cambio en Program.cs

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> Add-Content -Path Program.cs -Value "`n// Cambio corregido - Desafio 4"

- Respuesta: Se agregó una nueva modificación a Program.cs mediante el comentario Cambio corregido - Desafio 4. Esto permitió completar o corregir el contenido antes de crear nuevamente el commit.

```


## 12. Agregar el cambio corregido al staging

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git add .

- Resultado: warning: in the working copy of 'Program.cs', LF will be replaced by CRLF the next time Git touches it

- Respuesta: El comando git add . volvió a preparar los cambios de Program.cs para el nuevo commit. La advertencia sobre LF y CRLF corresponde al formato de saltos de línea que Git manejará en el archivo.

```


## 13. Crear el nuevo commit con la corrección

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git commit -m "Cambio corregido para Desafio 4"

- Resultado: 

[feature/cambio-prueba bf359ae] Cambio corregido para Desafio 4
 1 file changed, 4 insertions(+), 1 deletion(-)

- Respuesta: Se creó correctamente el nuevo commit bf359ae con el mensaje Cambio corregido para Desafio 4. Git confirma que los cambios corregidos de Program.cs quedaron registrados en la rama.

```


## 14. Ver historial final (todas las ramas, gráfico)

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git log --all --graph --oneline --decorate

- Resultado: 

* bf359ae (HEAD -> feature/cambio-prueba) Cambio corregido para Desafio 4
| * bcbc34c (feature/consulta-estudiantes) C3: cambios en feature/consulta-estudiantes
|/  
| * 6a59a99 (feature/validar-telefono) C4: cambios en feature/validar-telefono
| * e7a98a2 (feature/telefono-estudiante) C2: cambios en feature/telefono-estudiante
|/  
* 25b67c8 (main) C1: commit inicial en main

- Respuesta: El historial final muestra que bf359ae es ahora el commit más reciente de feature/cambio-prueba. El commit anterior cc6d846 ya no aparece en la historia de esta rama después del reset --soft.

```


## 15. Registrar el nuevo hash

```bash

- Comando: PS C:\Users\juanj\OneDrive\Desktop\ProgramacionV - copia (2) - copia\ProgramacionV.Api> git log -1 --oneline

- Resultado: bf359ae (HEAD -> feature/cambio-prueba) Cambio corregido para Desafio 4

- Respuesta: El nuevo commit quedó identificado con el hash corto bf359ae. El resultado también confirma que HEAD y feature/cambio-prueba apuntan actualmente a este commit.

```


## Explicación de qué ocurrió con el commit

- Respuesta: El commit original cc6d846 fue deshecho mediante git reset --soft HEAD~1, por lo que dejó de aparecer en el historial de la rama. Posteriormente, los cambios corregidos se registraron nuevamente en el commit bf359ae.



## Explicación de qué ocurrió con los archivos modificados

- Respuesta: Los cambios realizados en Program.cs no se eliminaron al deshacer el commit, sino que permanecieron disponibles para ser corregidos. Después, el archivo fue actualizado, agregado nuevamente al staging y registrado en el nuevo commit bf359ae.



# Pregunta de análisis 

## Explique qué diferencia existiría si el commit que se desea deshacer ya hubiera sido publicado y compartido en GitHub 

- Respuesta: Si el commit ya estuviera publicado en GitHub, modificar la historia con git reset podría generar diferencias entre la copia local y la compartida. En ese caso, normalmente sería más seguro usar git revert, porque deshace los cambios mediante un nuevo commit sin eliminar el historial existente.


