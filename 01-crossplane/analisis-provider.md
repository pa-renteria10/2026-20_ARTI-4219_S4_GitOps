# =====================================================================
# Análisis del Provider PostgreSQL
# =====================================================================

## Provider: tages/provider-postgresql v0.1.0

### 1. Managed Resources disponibles

<!-- Respuestas a las preguntas -->
Database => Crea y administra una base de datos en un servidor PostgreSQL
Extensión => Crea y administra una extensión en un servidor PostgreSQL
Función => Crea y gestiona una función en un servidor PostgreSQL.
Conceder => Crea y gestiona los privilegios otorgados a un usuario para un esquema de base de datos.
Cartografía => Crea y gestiona una asignación de usuario en un servidor PostgreSQL.
Privilegios => Crea y gestiona los privilegios predeterminados otorgados a un usuario para un esquema de base de datos
Configuración del proveedor =>  configura un proveedor de PostgreSQL
Uso de configuración del proveedor => indica que un recurso está utilizando un ProviderConfig.
Publicación => Crea y gestiona una publicación en una base de datos de servidor PostgreSQL.
Ranura de replicación => Crea y administra una ranura de replicación física en un servidor PostgreSQL.
Role => Crea y gestiona la pertenencia a un rol y a uno o más roles
Role => Crea y administra un rol en un servidor PostgreSQL.
Esquema => Crea y gestiona un esquema dentro de una base de datos PostgreSQL.
Servidor => Crea y administra un servidor externo en un servidor PostgreSQL
Ranura => Crea y administra un slot de replicación en un servidor PostgreSQL.
Configuración de la tienda => configura cómo el controlador de GCP debe almacenar los detalles de conexión.
Suscripción => es el esquema para la API de suscripciones


### 2. Campos requeridos del recurso Database

<!-- Respuestas a las preguntas -->
spec.forProvider (no tiene campos opcionales ya que todo el objeto es requerido y tienen valores por defecto)  
spec.providerConfigRef.name
spec.publishConnectionDetailsTo.configRef.name
spec.publishConnectionDetailsTo.name
spec.writeConnectionSecretToRef.name
spec.writeConnectionSecretToRef.namespace
status.conditions.lastTransitionTime
status.conditions.reason
status.conditions.status
status.conditions.type

### 3. Información requerida por el ProviderConfig

<!-- Respuestas a las preguntas -->
spec.credentials.env.name
spec.credentials.fs.path
spec.credentials.secretRef.key
spec.credentials.secretRef.name
spec.credentials.secretRef.namespace
spec.credentials.source
status.conditions.lastTransitionTime
status.conditions.reason
status.conditions.status
status.conditions.type