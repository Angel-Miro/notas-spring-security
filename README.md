# notas-spring-security

### Puntos clave de Spring Security
## Autenticación -> responde a la pregunta ¿Quién soy?
## Autorización  -> responde a la pregunta ¿Sobre que tengo permiso?
## Protección de Recursos -> responde a la pregunta ¿Qué está protegido y qué no lo está, qué es público o privado?
## Integración con diferentes mecanismos de autenticación  -> responde a la pregunta ¿Cómo hago la autenticación y/o autorzación?


# Aplicaciones Stateful (basada en sesiones) vs Stateless (basada en tokens de autenticación)
## Stateful
### Implica tener un estado en el servidor para cada usiaro que interactua con la app
### Eficaz para mantener información del usuario en el servidor y administar su sesión
### Requiere el almacenamiento y la gestión de sesiones en el servidor, lo que puede generar pproblemas de escalabilidad y rendimiento en aplicaciones con muchos usuarios concurrentes

## Stateless
### Se basa en la idea de que cada solicitud que realiza el cliente contiene toda la informacion necesaria para que el servidor la procese
### Altamente escalable y eficiente, ya que el servidor no necesita almacenar información del usuario
### Cada solicitud se procesa de manera independiente 
### Como toda la información necesaria se incluye en cada solicitud , los tokens o JWT debe de ser protegidos adecuadamente para evitar accesos no autorizados
