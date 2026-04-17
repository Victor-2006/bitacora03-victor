# bitacora03-victor

 # Fundamentos de Seguridad y Auditoría
 # Anatomía de Syslog

# El sistema Syslog permite registrar eventos del sistema combinando:

# Facility: origen del mensaje (auth, cron, daemon…)
# Severity: nivel de importancia (debug, info, warning, error, critical…)

# Esto ayuda a clasificar y analizar los eventos del sistema de forma eficiente.

## ¿Por qué es una negligencia grave que el archivo /var/log/auth.log tenga permisos de lectura para usuarios no privilegiados?

 Es grave que /var/log/auth.log sea accesible a usuarios normales porque contiene información sensible como intentos de login, usuarios, IPs o procesos, lo que puede facilitar ataques.

# Diferencias en logs:

## ¿Qué información específica (como PIDs, nombres de usuario o direcciones IP) diferencia un intento fallido de conexión remota SSH de un simple fallo de contraseña de un usuario local frente a la pantalla?


SSH fallido: muestra IP remota y servicio SSH
Fallo local: solo usuario y proceso, sin IP
 Log Management y cumplimiento (RGPD)

La gestión centralizada de logs consiste en enviar registros a un servidor externo seguro.

 # Ventajas:

Evita manipulación si el sistema es comprometido
Mejora auditorías y trazabilidad
Cumple normativas como el RGPD
Permite análisis y monitorización centralizada

 # Referencias (IEEE)

[1] R. Gerhards, “The Syslog Protocol,” IETF, RFC 5424, 2009.

[2] A. Behl and K. Behl, Cybersecurity and Cyberwar: What Everyone Needs to Know, Oxford University Press, 2017.
