## 4.2. Information Architecture

### 4.2.1. Organization Systems

1. ***Visual Organization***

Para facilitar la asimilación visual de la información, TerraTech aplicará los siguientes modelos de organización visual en distintas secciones de la plataforma:

- Se aplicará principalmente en el Dashboard de Monitoreo (US09) y la Landing Page. En el panel de control del agricultor, la información más crítica (como alertas rojas de "Riego Inmediato" o los indicadores actuales de N-P-K y Humedad) tendrá el mayor peso visual, ubicándose en la parte superior con tipografía de mayor tamaño y colores de acento. La información secundaria (como configuraciones de cuenta) tendrá un peso visual menor. En la Landing Page, la jerarquía guía el ojo desde la propuesta de valor principal (Hero Section) hacia los detalles (Características).

- Se empleará en los flujos operativos que requieren precisión para evitar la frustración del usuario. Esto incluye el proceso de Registro de Nuevo Usuario (US05), el flujo para Registrar un Nuevo Sensor IoT en la finca (US16) y el formulario de Solicitud de Demo (US03). La interfaz presentará pantallas o formularios divididos en pasos lógicos (ej. Paso 1: Datos personales -> Paso 2: Datos de la finca -> Paso 3: Conexión de sensores).

- Se utilizará para la visualización de datos cruzados y espaciales. Su principal aplicación será en el Mapa de Calor de Fertilidad (US12), donde el agricultor visualiza el estado del suelo cruzando variables espaciales (coordenadas X,Y del campo) con variables de salud (colores). También se aplicará en el Dashboard de la Cooperativa (US19), donde el administrador visualizará una tabla matricial cruzando filas (Socios/Lotes) con columnas (Rendimiento, Humedad, Alertas activas).
### 4.2.2. Labeling Systems

La aplicación utiliza un sistema de etiquetas y botones que ofrecen al usuario, dependiendo de si es un Agricultor individual o un Administrador de cooperativa, una manera de registrar, monitorear y gestionar sus campos de forma intuitiva.

- ***Para el visitante / usuario nuevo:*** Se utilizan botones de llamado a la acción directos en el Landing Page como "Solicitar Demo", junto con etiquetas claras para los formularios de registro (Nombre, Tamaño de terreno, etc).

- ***Para el Agricultor (Usuario principal):*** Se emplea terminología técnica pero accesible. Las métricas se etiquetan con sus unidades de medida claras: "Humedad (%)", "Nutrientes (N-P-K ppm)", y "Temperatura (°C)". Se utilizan botones de acción como "Agregar Sensor", "Ver historial" y selectores de rangos de fechas. Las alertas utilizan un lenguaje directo y accionable (ej. "Humedad excesiva en zona Sur").

- ***Para los Administradores de Cooperativa:*** Se tendrá una sección de "Reportes" y un "Dashboard Agregado". Las etiquetas cambian hacia un enfoque gerencial, mostrando columnas como "Promedio de rendimiento", "Hectáreas totales", y botones administrativos como "Exportar PDF", permitiendo comparar el rendimiento de múltiples lotes o socios.

### 4.2.3. SEO Tags and Meta Tags

Los SEO tags son etiquetas HTML que ayudan a los motores de búsqueda a entender y posicionar en los resultados. Los meta tags son etiquetas que proporcionan información sobre la página, como su descripción, palabras clave y autor, lo cual ayuda al ser buscado en el navegador. A continuación se presentan los SEO tags y meta tags que se utilizarán en la plataforma TerraTech:

***Title Tag:*** Este tag define el título de la página y es uno de los factores más importantes para el SEO. Debe ser único y contener palabras clave relevantes.

```html
<title>TerraTech - Monitoreo Inteligente y Agricultura de Precisión IoT</title>
```

***Meta Description:*** Este tag proporciona una breve descripción del contenido de la página. Permite a los usuarios entender de qué trata la página antes de hacer clic en el enlace. Debe ser conciso y atractivo.

```html
<meta name="description" content="TerraTech es una plataforma de agricultura inteligente que optimiza el riego y la fertilización mediante sensores IoT en tiempo real, mapas de fertilidad y análisis predictivo para agricultores.">
```

***Language tag:*** Este tag indica el idioma principal del contenido de la página. Es importante para la accesibilidad y el SEO.

```html
<meta http-equiv="Content-Language" content="es-PE">
```

***Robots tag:*** Este tag indica a los motores de búsqueda cómo deben indexar la página. Puede ser utilizado para evitar que ciertas páginas sean indexadas (por ejemplo, el dashboard interno).

```html
 <meta name="robots" content="index, follow">
```

***Author tag:*** Este tag indica el autor del contenido de la página. Es útil para dar crédito a los creadores de contenido.

```html
<meta name="author" content="NovaTech Agro Team">
```

***Meta Viewport:*** Este tag es esencial para que la página sea responsiva en dispositivos móviles (vital para agricultores en el campo). Mejora la experiencia del usuario y es un factor importante para el SEO técnico.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

***Canonical Tag:*** Este tag especifica la URL canónica de la página para evitar problemas de contenido duplicado en motores de búsqueda. Ayuda a consolidar el posicionamiento de una sola versión de la página.***

```html
<link rel="canonical" href="https://www.terratech-agro.com/">
```

### 4.2.4. Searching Systems

Para encontrar ciertas funcionalidades de nuestra aplicación, usamos varios botones y empleamos varios indicadores visuales para que el usuario sepa dónde encontrar lo que necesita. A continuación se muestran los ejemplos de los tipos de búsqueda que usaremos:

- ***Búsqueda de zonas y sensores:*** Para facilitar el monitoreo en fincas grandes, usamos una serie de filtros y un selector desplegable para que el agricultor pueda hallar exactamente la zona de cultivo o el sensor individual (ID) del cual desea ver los datos en tiempo real.

- ***Búsqueda en histórico de datos:*** Usamos filtros por rango de fechas y tipo de métrica (Humedad, Nitrógeno, Fósforo, Potasio o Temperatura) para que el agricultor pueda graficar las tendencias de los últimos días y detectar patrones en su suelo.

- ***Búsqueda de socios y reportes:*** Para los administradores de la cooperativa, se les da una forma de buscar rápidamente el rendimiento por socio o por lote específico, permitiéndoles acceder ágilmente al dashboard consolidado y a la exportación de reportes en PDF.

### 4.2.5. Navigation Systems

- ***Registro e Inicio de Sesión:*** Para poder entrar, el usuario ingresará sus credenciales y el sistema registrará qué tipo de usuario es: Agricultor, que busca monitorear sus sembríos y recibir recomendaciones de riego/fertilización, o Administrador de Cooperativa, que requiere visualizar métricas globales y reportes de todos los socios.

- ***Dashboard de Monitoreo:*** Permite a los usuarios visualizar los indicadores clave del suelo en tiempo real, ver el pronóstico del clima integrado y acceder rápidamente a las notificaciones y recomendaciones predictivas del sistema.

- ***Mapas y Análisis:*** Permite a los agricultores navegar de forma interactiva (zoom y desplazamiento) sobre el mapa de calor de fertilidad de su terreno y visualizar imágenes satelitales recientes para identificar áreas críticas.

- ***Gestión de Dispositivos:*** Una sección dedicada donde el agricultor puede registrar nuevos sensores físicos a su cuenta y configurar los umbrales personalizados de alerta para cada métrica.

- ***Mi perfil:***  Permite a los usuarios configurar sus preferencias personales, actualizar la información técnica de su finca o cooperativa, y cambiar su contraseña.