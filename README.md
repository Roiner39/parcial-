# $\textcolor{purple}{\textbf{PARCIAL - CIBERSEGURIDAD}}$

## $\textcolor{blue}{\textbf{¿Qué es la ciberseguridad?, ¿Cuáles son sus características y cómo se ve reflejada en mi vida personal?}}$

### $\textcolor{purple}{\textbf{Ciberseguridad}}$

La ciberseguridad es el conjunto de medidas y herramientas que se utilizan para proteger los dispositivos, sistemas, redes, programas y datos frente a accesos no autorizados, ataques, daños o robos de información.

Su objetivo es que la información pueda manejarse de manera $\textcolor{green}{\textbf{confidencial, íntegra y disponible}}$, reduciendo los riesgos que pueden aparecer por el uso de la tecnología.

<img width="641" height="358" alt="Ciberseguridad" src="https://github.com/user-attachments/assets/0206867f-8def-49d8-a8d0-4da235311e96" />

### $\textcolor{green}{\textbf{Características}}$

Algunas características importantes de la ciberseguridad son la prevención de incidentes, la protección de los sistemas y la recuperación de información cuando ocurre algún problema.

También es importante tener en cuenta que la ciberseguridad no busca eliminar completamente todos los riesgos, sino reducir la posibilidad de que ocurran y disminuir el daño que puedan causar.

- $\textcolor{green}{\textbf{Preventiva y reactiva:}}$ busca prevenir problemas y también responder cuando ocurre un incidente.
- $\textcolor{green}{\textbf{Multidisciplinaria:}}$ necesita conocimientos de diferentes áreas.
- $\textcolor{green}{\textbf{Dinámica y evolutiva:}}$ debe adaptarse porque las amenazas y tecnologías cambian constantemente.
- $\textcolor{green}{\textbf{Orientada a la gestión del riesgo:}}$ busca identificar los riesgos y reducir sus posibles consecuencias.

### $\textcolor{orange}{\textbf{Reflejo en mi vida personal}}$

La ciberseguridad está presente en varias actividades que realizo diariamente. Por ejemplo, utilizo contraseñas y cuentas en diferentes páginas y servicios, por lo que debo tener cuidado con los lugares donde ingreso mi información.

También me ayuda a reconocer que no debo abrir cualquier enlace o archivo y que debo estar atento ante posibles virus o programas maliciosos. Si mi computador llegara a presentar un problema de este tipo, tendría una mejor idea de cómo actuar.

<img width="790" height="366" alt="Seguridad informática" src="https://github.com/user-attachments/assets/438bbf26-1fd9-47da-962c-a0a694d85ce4" />

---

## $\textcolor{purple}{\textbf{¿Cuál es el objetivo de la tríada de seguridad? y ¿Cuál sería su función en un estándar como el EMV usado en tarjetas de crédito?}}$

### $\textcolor{purple}{\textbf{Objetivo}}$

- $\textcolor{blue}{\textbf{Confidencialidad:}}$ garantizar que la información solamente pueda ser consultada por personas o sistemas autorizados.
- $\textcolor{blue}{\textbf{Integridad:}}$ garantizar que la información no sea alterada, modificada o corrompida sin autorización.
- $\textcolor{blue}{\textbf{Disponibilidad:}}$ garantizar que la información y los sistemas estén disponibles cuando los usuarios autorizados los necesiten.

### $\textcolor{blue}{\textbf{Función del estándar EMV}}$

#### $\textcolor{blue}{\textbf{1. Inserción de la tarjeta y detección del chip}}$

El datáfono o terminal POS detecta el chip EMV de la tarjeta y establece comunicación con él. Esto permite utilizar el chip en lugar de depender únicamente de la banda magnética, que es más vulnerable a la clonación.

#### $\textcolor{blue}{\textbf{2. Autenticación del chip}}$

El chip contiene claves criptográficas únicas y certificados digitales que permiten comprobar que la tarjeta es auténtica y no una copia. Para esto se utilizan mecanismos de autenticación dinámica como DDA/CDA y criptografía asimétrica.

#### $\textcolor{blue}{\textbf{3. Generación de un criptograma único por transacción}}$

El chip genera un código criptográfico dinámico diferente para cada transacción. Esto dificulta que un dato interceptado pueda reutilizarse y ayuda a proteger contra la clonación.

#### $\textcolor{blue}{\textbf{4. Verificación del titular}}$

Se puede verificar al titular mediante un PIN cifrado o una firma, confirmando que la persona que está utilizando la tarjeta es el usuario autorizado.

<img width="817" height="393" alt="Tarjeta EMV" src="https://github.com/user-attachments/assets/bc1b6b51-b813-4214-8cc4-2d5f74d611d8" />

### $\textcolor{orange}{\textbf{Pasos ante un posible archivo malicioso}}$

- $\textcolor{red}{\textbf{Aislar el equipo:}}$ desconectarlo de la red para evitar que una posible amenaza se propague a otros equipos.
- $\textcolor{red}{\textbf{No apagarlo abruptamente:}}$ conservar, si es posible, la evidencia que se encuentra en la memoria RAM y en los procesos activos.
- $\textcolor{red}{\textbf{Revisar procesos y conexiones activas:}}$ utilizar `tasklist` o el Administrador de tareas para identificar procesos desconocidos o sospechosos.
- $\textcolor{red}{\textbf{Analizar el archivo X:}}$ calcular su hash, por ejemplo MD5 o SHA256, y compararlo en plataformas como VirusTotal.
- $\textcolor{red}{\textbf{Revisar cómo se ejecutó:}}$ comprobar si el usuario tuvo que ejecutarlo manualmente o si se ejecutó por sí solo.
- $\textcolor{red}{\textbf{Analizar el comportamiento:}}$ comprobar si el archivo se replicó o infectó otros archivos.
- $\textcolor{red}{\textbf{Comprobar la propagación:}}$ verificar si se propagó a otros equipos de la red.
- $\textcolor{red}{\textbf{Revisar acciones sospechosas:}}$ comprobar si abrió puertos, creó accesos remotos, robó credenciales o descargó otros archivos.

<img width="705" height="396" alt="Análisis de amenazas" src="https://github.com/user-attachments/assets/854068dd-b968-4e7f-9c89-a9a753fb6d7f" />

---

## $\textcolor{red}{\textbf{El PC de una compañía está funcionando de manera errónea después de descargar un archivo X.}}$

Lo primero que debería hacer la empresa es desconectar el equipo de Internet y de la red, con el objetivo de evitar que una posible amenaza se propague a otros dispositivos.

Después se pueden revisar cuidadosamente los procesos y tareas del sistema, utilizando herramientas como el Administrador de tareas, `Wireshark` o `netstat` para observar conexiones y comportamientos sospechosos.

También es importante analizar el archivo descargado y observar su comportamiento para determinar si se trata de un virus, gusano o troyano.

---

## $\textcolor{blue}{\textbf{Diferencia entre hacker de sombrero negro, sombrero blanco, sombrero gris y cracker}}$

| Tipo | Característica |
|---|---|
| $\textcolor{green}{\textbf{Sombrero blanco}}$ | Trabaja de manera autorizada para encontrar vulnerabilidades y ayudar a mejorar la seguridad de los sistemas. |
| $\textcolor{orange}{\textbf{Sombrero gris}}$ | Puede investigar o entrar en sistemas sin autorización, normalmente por curiosidad o interés. |
| $\textcolor{red}{\textbf{Sombrero negro}}$ | Busca aprovechar vulnerabilidades de forma maliciosa para obtener beneficios o causar daños. |
| $\textcolor{purple}{\textbf{Cracker}}$ | Se caracteriza por romper o vulnerar sistemas, programas o mecanismos de seguridad. |

La principal diferencia está en la $\textcolor{blue}{\textbf{intención y autorización}}$ con la que actúa cada uno.

---

## $\textcolor{purple}{\textbf{Leyes y marcos internacionales orientados a la ciberseguridad y el Habeas Data}}$

| Norma / Marco | Región / Alcance | Descripción |
|---|---|---|
| $\textcolor{blue}{\textbf{GDPR}}$ | Unión Europea | Reglamento de protección de datos personales que establece derechos y obligaciones relacionados con el tratamiento de información personal. |
| $\textcolor{blue}{\textbf{CCPA}}$ | Estados Unidos - California | Otorga a los consumidores derechos relacionados con sus datos personales. |
| $\textcolor{blue}{\textbf{Convenio de Budapest}}$ | Internacional | Tratado orientado a combatir el delito informático mediante cooperación entre países. |
| $\textcolor{blue}{\textbf{HIPAA}}$ | Estados Unidos | Protege la confidencialidad de la información médica y de salud. |
| $\textcolor{blue}{\textbf{ISO/IEC 27001}}$ | Internacional | Estándar para implementar un Sistema de Gestión de Seguridad de la Información. |
| $\textcolor{blue}{\textbf{PCI DSS}}$ | Internacional | Estándar de seguridad relacionado con entidades que procesan, almacenan o transmiten datos de tarjetas de pago. |
Get-FileHash "C:\ruta\archivo.exe" -Algorithm SHA256
Start-MpScan -ScanType FullScan

## $\textcolor{purple}{\textbf{Flujo de trabajo para compartir información mediante GitHub}}$

