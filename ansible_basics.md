### ¿Qué es Ansible y por qué es "sin agente"?

Ansible es una herramienta de automatización que permite gestionar diferentes equipos de forma eficiente y sencilla. Es considerado agentless porque no requiere que los sistemas a gestionar tengan instalado un software adicional, basta con configurar la herramienta en un servidor para este fin.


### Explica la diferencia entre un comando ad-hoc y un playbook

La diferencia principal radica en su propósito y complejidad, además de la forma en la que son ejecutados. Los comandos ad-hoc son ejecuciones rápidas de una única tarea, mientras que los playbooks son un conjunto de instrucciones que permiten automatizar tareas complejas y pueden ser reutilizables.


### ¿Qué es la idempotencia y por qué es importante en Ansible?

Una operación se considera idempotente si el resultado de ejecutarla una sola vez es exactamente el mismo que ejecutarla repetidas veces. En Ansible es importante porque asegura que las tareas definidas no causen cambios innecesarios en caso de haber sido aplicados de forma previa ya que la ejecución de la misma tarea múltiples veces no generara nuevos efectos.

### ¿Cómo funcionan los handlers y cuando deberías usarlos?

Los handlers son instrucciones que ocurren cuando otras instrucciones las llaman. No son ejecutadas a menos que sean notificadas de la ejecución. Los handlers pueden ser usados para reiniciar algún servicio, o el servidor luego de cambios que así lo requieran.

### ¿Cómo verificar errores de sintaxis en un playbook de Ansible?

Para verificar errores en un playbook de Ansible basta con ejecutar instalar la herramienta `ansible-lint` que nos ayudara a analizar los playbooks, roles y colecciones de Ansible evitando errores comunes como errores de sintaxis e identado, facilitando la escritura y la detección de errores.
