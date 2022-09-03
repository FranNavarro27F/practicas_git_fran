comandos:

- bit brack nomreDeLaRama  - cra una rama con el Nombre de la rama, donde estes parado o checkauteado -

- git checkout nombre    - este comando es "pararte en tal nombre", aplica a commits y a ramas -

- git merge nombreDeRama  - este comando mergea, unifica, las dos ramas desde donde se esta parado traes los cambios de la otra rama -

- git rebase nombreDeLaRama  - este comando rebasa, unifica, las dos ramas creara un nuevo comit que incluye todo lo trabajado en la rama donde estas y añade tambien todo lo trabajado en la rama a la que vas, (luego se hace el mismo comando en la rama objetivo de este rebase hacia la rama que lo hizo en primer lugar, para que las 2 ramas esten actualizadas) -

- git branck -f lugarAlQueMovemosLaRama   - este comando fuerza el cambio de lugar de la rama a donde se le indique -

- ^ esto nos ayuda a tomar referencias relativas de posicion: - git checkout main^ - ese comando nos posisionaria en un comit anterior al ultimo del main -

- ~ esto nos ayuda a tomar cierta cantidad numerica como referencia relativa,
- git ckeckout main~4 - nos movera 4 comits antes de el ultimo de main -

- git reset main~1 - este comando  revierte los cambios moviendo la referencia de una rama hacia atrás en el tiempo a un commit anterior. En este sentido podés pensarlo como "reescribir la historia". git reset va a mover la rama hacia atrás, como si el commit nunca se hubiera hecho -

- git revert: revierte los cambios en el repositorio remoto, pero no es tan asi... revierte los cambios del ultimo comit al crear un nuevo commit con la info del anterior al cambio y luego hay que pushear ese nuevo comit que va a dejar todo como antes del cambio no deseado. (para usarse: comandos de consola linux  Esc + shift + :      luego tipear "w"(sin las commillas)para guardar, "q" (sin las comillas) para quitear) -

- git cherry-pick ejempoHashComit1 ejempoHashComit2 ...etc   - este comando capia los comits que indiquemos de las ramas que se nos cante, y crea tantos comits como tengamos copiados con esa misma informacion pero en la rama en donde estabamos parados, es decir: que tomamos el trabajo de otras ramas y lo colocamos donde querramos! -

- git rebase -i   - complicadisimo de usar. resultados similares a cherry-pick -

- git log   - este comando muestra o loguea todos los hashes de los comits.

- concepto:
          : *head*: commit en donde estoy parado al ingresar a la rama. (comit en donde esta el foco, etc.)
          : *detachear* (des-adjuntar) HEAD simplemente significa adjuntarla a un commit en lugar de a un branch.
          : *atachear*: apuntar el head a un comit en particular.
          : *hash*: codigo (creado por git, un hash) asociado al nombre del comit.
          : *drag & drop*: arrastrar y soltar.
          : *--* los dos guiones medios significan "pick".
          : *squashear commits*: permite combinar varios comits en uno solo.
          :




lñaksdjfklñasdjgklñasjdglñahjsfgñasdfhfñjsdfñljsadfas asdklñjfñaklsdjfñklasdjfñklasdjflñkasdjfñlkasdjfjasdfñjasdlfjasdldkfjasdkljfñasdflasdjklfasdjñf.