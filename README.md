# OsintwitX
🔥 Este script te ayudará a obtener información clave sobre cualquier usuario de Twitter en segundos. Aqui las funciones utilizadas apartir una biblioteca de Python ( [Twikit](https://github.com/d60/twikit) ) que permite interactuar con la API interna de Twitter sin necesidad de una clave de API. Esto se logra mediante técnicas de scraping, facilitando el acceso a diversas funcionalidades de Twitter de forma gratuita.

- 🔎 Búsqueda y obtención de información
    * search_tweet(query: str): Buscar tweets con palabras clave o hashtags
    * search_user(query: str): Buscar usuarios por nombre o palabra clave.
    * get_user_by_screen_name(username: str): Obtener información de un usuario por su @usuario.
    * get_user_by_id(user_id: str): Obtener información de un usuario por su ID de Twitter.
    * get_user_tweets(user_id: str): Obtener los tweets de un usuario específico.
    * get_trends(): Obtener temas de tendencia en Twitter.
    * get_place_trends(woeid: int): Obtener tendencias en una ubicación específica.

- 👉 Útil para:

    * Identificar a personas relacionadas con un tema.
    * Buscar tweets recientes sobre eventos importantes.
    * Ver tendencias y posibles campañas de desinformación.

- 👤 Investigación de perfiles
    * get_user_followers(user_id: str): Obtener los seguidores de un usuario.
    * get_user_following(user_id: str): Obtener las cuentas que sigue un usuario.
    * get_lists(user_id: str): Ver las listas en las que un usuario está agregado.

- 👉 Útil para:

    * Analizar la red de contactos de una persona.
    * Identificar cuentas asociadas con grupos o movimientos.
    * Ver en qué listas públicas ha sido agregado un usuario.

- 🕵️ Análisis de comunidades y grupos
    * search_community(query: str): Buscar comunidades en Twitter.
    * get_community(community_id: str): Obtener información de una comunidad.
    * get_community_tweets(community_id: str): Obtener tweets de una comunidad.

- 👉 Útil para:
    * Investigar grupos y comunidades relacionadas con un tema.
    * Analizar qué se dice dentro de una comunidad específica.
    * Identificar usuarios influyentes dentro de un grupo.
  
- 📡 Monitoreo de actividad
    * get_notifications(): Obtener las notificaciones de la cuenta.
    * get_dm_history(): (Si tienes acceso a una cuenta) Ver el historial de mensajes directos.

- 👉 Útil para:
    * Monitorear menciones y respuestas a tweets clave.
    * Identificar patrones de interacción en tiempo real.


##  🔧 Configuracion | Comenzando
### Crear un entorno virtual llamado "OsintwitX"
`python3 -m venv OsintwitX`

### Activar el entorno virtual
- `source OsintwitX/bin/activate  # En Linux/macOS`
- `OsintwitX\Scripts\activate     # En Windows (PowerShell)`

### Instalar las dependencias dentro del entorno virtual
`pip install twikit python-dotenv networkx matplotlib`

### Crea un archivo .env en la misma carpeta donde está el script.
- Añade tus credenciales de Twitter en el archivo .env con este formato:

- ``TWITTER_USERNAME=tu_usuario``
- ``TWITTER_EMAIL=tu_email@example.com``
- ``TWITTER_PASSWORD=tu_contraseña``

- Guarda el archivo.

🔴 IMPORTANTE: Nunca compartas tus credenciales con nadie y evita guardarlas en repositorios públicos.

## 🚀 Ejecucion
### Cada vez que quieras ejecutar el script, activa el entorno virtual con:


- ``source OsintwitX/bin/activate``
- ``python3 OsintwitX.py``

✏️ Ejemplo de uso:

- Para buscar tweets de un tema, selecciona 1 e introduce una palabra clave o hashtag.
- Para ver información de un usuario, selecciona 2 e ingresa su @usuario.
- Para obtener las tendencias actuales, selecciona 5.
📌 Los datos obtenidos se guardan en archivos JSON o CSV automáticamente.





## 🎯 Consejos Adicionales
- Usa una cuenta secundaria de Twitter, ya que el scraping puede generar bloqueos si se usa en exceso.
- Revisa los archivos generados (.json, .csv) para analizar mejor la información.


