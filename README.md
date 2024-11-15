# PRÁCTICA Nro 2
## Nombre: Danae Katherin Largo Bobarin
Seguridad de Software

![](https://proiso.pe/wp-content/uploads/elementor/thumbs/ciberataques-qphf4yy64974cnvvv0emjhbhgj02ah1p06gn45wna8.webp)
1. Lectura y Análisis:
Inyección (SQL, NoSQL, OS, LDAP):
Ocurre cuando los atacantes insertan código malicioso (por ejemplo, SQL) a través de campos de entrada sin la debida validación. Esto puede permitir la ejecución de comandos no autorizados en la base de datos o en el sistema operativo.
Cross-Site Scripting (XSS):
Es una vulnerabilidad en la que el atacante inyecta scripts maliciosos en páginas web que son vistas por otros usuarios. Estos scripts pueden robar información sensible o realizar acciones en nombre del usuario sin su consentimiento.
Cross-Site Request Forgery (CSRF):
Un ataque CSRF hace que el navegador de un usuario autenticado envíe solicitudes no autorizadas a un servidor web, lo que puede comprometer la cuenta del usuario sin que lo sepa.
Broken Authentication:
Ocurre cuando un sistema de autenticación es defectuoso, lo que puede permitir a un atacante obtener acceso a cuentas de usuario sin autorización, generalmente aprovechando contraseñas débiles o errores en el proceso de validación.
Insecure Direct Object References (IDOR):
Se presenta cuando una aplicación permite a un usuario acceder directamente a objetos (como archivos o registros en la base de datos) a través de URLs u otros parámetros, sin verificar si el usuario tiene permiso para acceder a esos objetos.
Security Misconfiguration:
Implica una mala configuración de los sistemas, como la exposición de información sensible o el uso de configuraciones predeterminadas que no se han actualizado, lo que facilita los ataques.
Sensitive Data Exposure:
Ocurre cuando los datos sensibles, como contraseñas o información financiera, no se protegen adecuadamente, ya sea por no cifrarlos o por almacenarlos de manera insegura.

2. Investigación de Casos Reales:
Caso 1: Cross-Site Scripting (XSS)
Aplicación Afectada: Yahoo! (2014)
Vulnerabilidad Explotada: XSS almacenado
Consecuencias: Un atacante podía inyectar código JavaScript malicioso en un foro de Yahoo!, lo que permitía robar las credenciales de los usuarios que visitaran ese foro. Los datos comprometidos incluyeron nombres de usuario y contraseñas.
Medidas Correctivas: Se implementó el filtrado adecuado de entradas en el foro y la codificación de salida para evitar la ejecución de scripts maliciosos.
Caso 2: Broken Authentication
Aplicación Afectada: Instagram (2019)
Vulnerabilidad Explotada: Autenticación rota debido a un fallo en la validación de las sesiones de usuario.
Consecuencias: Un atacante podía tomar el control de las cuentas de los usuarios sin conocer sus contraseñas, aprovechando un error en el proceso de validación de las sesiones.
Medidas Correctivas: Instagram implementó un nuevo sistema de autenticación basado en tokens más seguros y fortaleció el proceso de validación de sesiones.

3. Análisis Crítico:
Falta de educación y concienciación: Muchos desarrolladores no están completamente informados sobre las mejores prácticas de seguridad, lo que lleva a la creación de aplicaciones vulnerables.
Desarrollo rápido sin pruebas de seguridad: Muchas veces, la prioridad es lanzar rápidamente el producto sin realizar pruebas de seguridad adecuadas, lo que deja espacio para la explotación de vulnerabilidades.
Configuraciones predeterminadas: Muchas aplicaciones usan configuraciones predeterminadas que son inseguras o no actualizan sus configuraciones de seguridad con regularidad.
Métodos de prevención para las vulnerabilidades seleccionadas:
Prevención para XSS:
Validación de Entrada: Asegurarse de que los datos proporcionados por el usuario sean correctos y no contengan scripts maliciosos.
Codificación de Salida: Escapar los caracteres especiales en las respuestas para evitar la ejecución de scripts.
Uso de Content Security Policy (CSP): Implementar políticas de seguridad que controlen qué recursos pueden ser cargados y ejecutados en la página.
Prevención para Broken Authentication:
Autenticación Multifactor (MFA): Requerir más de un método para verificar la identidad del usuario (por ejemplo, una contraseña y un código enviado por SMS).
Almacenamiento Seguro de Contraseñas: Utilizar algoritmos de hash seguros (como bcrypt) y nunca almacenar contraseñas en texto claro.
Control de Sesiones: Asegurarse de que las sesiones caduquen después de un período de inactividad y se invaliden al cerrar sesión.

4. Evaluación:
Claridad y profundidad del análisis: Explica bien los conceptos, las vulnerabilidades, y las soluciones, y asegúrate de que tu investigación de casos sea precisa.
Investigación y precisión en los casos documentados: Asegúrate de que los ejemplos de vulnerabilidades sean relevantes y bien documentados.
Resumen para tu tarea:
Análisis de las vulnerabilidades: Define las vulnerabilidades del OWASP Top Ten que seleccionaste.
Casos Reales: Incluye los dos ejemplos con los detalles de la vulnerabilidad, las consecuencias y las medidas correctivas.
Análisis Crítico: Explica por qué estas vulnerabilidades son comunes y qué medidas puedes implementar para prevenirlas.
