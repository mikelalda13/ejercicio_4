# Ejercicios prácticos de Git


## 1. Configuración

**Ejercicio:** Configura tu nombre de usuario y correo electrónico en Git usando los comandos apropiados. Luego, verifica tu configuración.

## 2. Ambiente de desarrollo

**Ejercicio:** Crea un nuevo directorio llamado "mi_proyecto_git". Inicializa un repositorio Git en este directorio y crea un archivo README.md con una breve descripción del proyecto.

## 3. Estados de los archivos

**Ejercicio:** En el repositorio que creaste, realiza las siguientes acciones:

1. Crea un nuevo archivo llamado "archivo1.txt"
2. Modifica el archivo README.md
3. Usa `git status` para ver el estado de los archivos
4. Agrega "archivo1.txt" al staging area
5. Usa `git status` nuevamente y explica la diferencia en el estado de los archivos

## 4. Comandos básicos para la gestión de un repositorio

**Ejercicio:** Continúa con el repositorio anterior:

1. Realiza tu primer commit incluyendo ambos archivos
2. Modifica "archivo1.txt"
3. Usa `git diff` para ver los cambios
4. Realiza un segundo commit solo con los cambios en "archivo1.txt"
5. Usa `git log` para ver el historial de commits

## 5. Correcciones básicas

**Ejercicio:** Imagina que acabas de hacer un commit pero olvidaste incluir un archivo importante. Realiza los siguientes pasos:

1. Crea un nuevo archivo llamado "archivo_olvidado.txt"
2. Usa el comando apropiado para incluir este archivo en el commit anterior sin crear un nuevo commit
3. Verifica que el cambio se haya aplicado correctamente

## 6. Comandos básicos para ramas

**Ejercicio:** En tu repositorio:

1. Crea una nueva rama llamada "feature-x"
2. Cambia a esta nueva rama
3. Realiza algunos cambios y commits en esta rama
4. Vuelve a la rama principal (main o master)
5. Lista todas las ramas y identifica en qué rama estás actualmente

## 7. Fusión de ramas

**Ejercicio:** Practica dos tipos de fusiones:

1. Realiza una fusión fast-forward de "feature-x" en la rama principal
2. Crea otra rama llamada "feature-y", haz algunos cambios, y luego realiza una fusión recursiva con la rama principal

## 8. Comandos básicos para merges

**Ejercicio:** Documenta los pasos exactos (comandos) que usaste para realizar las fusiones en el ejercicio anterior.

## 9. Navegando entre commits

**Ejercicio:** Usa `git log` para ver el historial de commits. Luego:

1. Navega a un commit específico usando su hash
2. Vuelve al commit más reciente de la rama actual

## 10. Conflictos al realizar un merge

**Ejercicio:** Crea intencionalmente un conflicto de merge:

1. Crea una nueva rama y modifica un archivo
2. Vuelve a la rama principal y modifica el mismo archivo de manera diferente
3. Intenta fusionar la nueva rama en la principal
4. Resuelve el conflicto manualmente
5. Completa el merge

## 11. Repositorios remotos

**Ejercicio:**

1. Crea un repositorio en GitHub (o cualquier otra plataforma Git)
2. Conecta tu repositorio local con el remoto
3. Realiza un push de tus cambios locales al repositorio remoto

## 12. Acceso a repositorios remotos

**Ejercicio:** Clona un repositorio público de GitHub. Luego, lista los remotos asociados a este repositorio clonado.

## 13. Operaciones de lectura y escritura (fetch, pull y push)

**Ejercicio:** Con el repositorio que creaste en GitHub:

1. Realiza un cambio directamente en GitHub
2. Usa `git fetch` para actualizar tu repositorio local
3. Usa `git diff` para ver las diferencias entre tu rama local y la remota
4. Usa `git pull` para incorporar los cambios
5. Realiza un cambio local y usa `git push` para subirlo al remoto

## 14. Obtener información detallada de un repositorio remoto

**Ejercicio:** Usa `git remote show origin` para obtener información detallada sobre tu repositorio remoto. Anota tres piezas de información que encuentres útiles.

## 15. Configurar upstreams

**Ejercicio:** Crea una nueva rama local, súbela al repositorio remoto, y configura el upstream para esta rama.

## 16. Tagging

**Ejercicio:**

1. Crea un tag ligero llamado "v1.0" en tu último commit
2. Crea un tag anotado llamado "v1.1" con un mensaje descriptivo
3. Lista todos tus tags
4. Muestra la información detallada del tag anotado

## 17. Tags y ramas con el mismo nombre

**Ejercicio:** Crea un tag y una rama con el mismo nombre. Luego, explica cómo Git diferencia entre ellos y cómo puedes referirte específicamente a cada uno.

## 18. Publicar y eliminar tags

**Ejercicio:**

1. Publica tus tags en el repositorio remoto
2. Elimina el tag "v1.0" tanto localmente como en el remoto

## 19. GitHub Flow

**Ejercicio:** Simula el uso de GitHub Flow:

1. Crea una rama para una nueva característica
2. Realiza algunos commits en esta rama
3. Abre un Pull Request (puedes hacerlo en GitHub)
4. Simula una revisión de código haciendo algunos comentarios
5. Mergea el Pull Request

## 20. Stashing

**Ejercicio:**

1. Haz algunos cambios en tu working directory
2. Usa `git stash` para guardar estos cambios temporalmente
3. Cambia a otra rama y vuelve
4. Aplica los cambios stashed
5. Crea un nuevo stash con un mensaje descriptivo

## 21. Ignorar archivos (.gitignore)

**Ejercicio:**

1. Crea un archivo `.gitignore` en tu repositorio
2. Agrega reglas para ignorar:
   - Todos los archivos .log
   - El directorio `node_modules`
   - Todos los archivos .tmp excepto important.tmp
3. Verifica que las reglas funcionan correctamente

## 22. Reescribiendo la historia

**Ejercicio:** Usa `git rebase -i` para:

1. Combinar los últimos tres commits en uno solo
2. Cambiar el mensaje de un commit anterior
3. Eliminar un commit específico

## 23. Cherry pick

**Ejercicio:**

1. Crea dos ramas diferentes con algunos commits únicos en cada una
2. Usa `git cherry-pick` para aplicar un commit específico de una rama a la otra

## 24. Reset

**Ejercicio:** Practica los tres tipos de reset:

1. Soft reset: Mueve HEAD pero mantén los cambios en el staging area
2. Mixed reset: Mueve HEAD y actualiza el staging area, pero mantén los cambios en el working directory
3. Hard reset: Mueve HEAD, actualiza el staging area y el working directory

## 25. Revert

**Ejercicio:**

1. Identifica un commit anterior que quieras revertir
2. Usa `git revert` para crear un nuevo commit que deshaga los cambios de ese commit específico

## 26. Rebase

**Ejercicio:**

1. Crea una rama feature que diverja de la rama principal
2. Haz algunos commits en la rama principal
3. Usa `git rebase` para actualizar tu rama feature con los cambios de la rama principal

## 27. Examinando el staging area, working tree y repositorio

**Ejercicio:** Realiza las siguientes acciones y usa los comandos apropiados para examinar el estado después de cada paso:

1. Modifica un archivo
2. Agrega el archivo al staging area
3. Realiza un commit
4. Modifica el mismo archivo nuevamente

Usa `git status`, `git diff`, y `git diff --staged` para examinar los cambios en cada etapa.

Estos ejercicios te ayudarán a practicar y comprender mejor los conceptos de Git. Recuerda consultar la documentación oficial de Git si necesitas más información sobre algún comando o concepto específico.
