### Que es ansible

Ansible es una herramienta de automatizacion que permite gestionar equipos de forma eficiente y sencilla. Es considerado agentless porque no requiere que los sistemas a gestionar tengan un software adicional instalado.


### Diferencia entre un comando ad-hoc y un playbook

La diferenica principal radica en su proposito y complejidad, ademas de la forma en la que son ejecutados. Los comandos ad-ohc son ejecuciones rapidas de una unica tarea, mientras que los playbooks son un conjunto de instrucciones que permiten automatizar tareas complejas y pueden ser reutilizables.


### Que es la idempotencia

Una operacion se considera idempotente si el resutlado de ejecutarla una sola vez es exactamente el mismo que ejecutarla repetidas veces. En ansible es importante porque asegura que las tareas definidas no causen cambios inncesarios en caso de haber sido aplicados de forma previa ya que la ejecucion de la misma tarea multiples veces no generara nuevos efectos.

### Como funcionan los handlers y cuando usarlos

Los handlers son instrucciones que ocurren cuando otras instrucciones las llaman. No son ejecutadas a menos que sean notificadas de la ejecucion. Los handlers pueden ser usados para reiniicar algun servicio, o el servidor luego de cambios que asi lo requieran.

### Como verificar errores de sintaxis en un playbook

Para verificar errores en un playbook de ansible basta con ejecutar instalar la herramienta `ansible-lint` que nos ayudara a analizar los playbooks, roles y colecciones de Ansible evitando errores comunes como errores de sintaxis, identado, facilitando la escritura y la deteccion de errores.

