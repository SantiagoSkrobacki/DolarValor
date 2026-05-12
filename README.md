DolarValor - Reporte Automatizado con IA
Este proyecto consiste en un flujo de automatización desarrollado en n8n que monitorea el valor del dólar blue en Argentina, gestiona un histórico de datos y genera reportes analíticos utilizando Inteligencia Artificial.

🚀 Funcionamiento del Flujo
El sistema se ejecuta automáticamente todos los días a las 08:00 AM y realiza los siguientes pasos:

Obtención de Datos: Consulta el precio actual del dólar blue a través de una API externa.

Persistencia: Almacena el valor y la fecha en una base de datos de Supabase para mantener un registro histórico.

Recolección de Noticias: Realiza un scraping de las principales noticias económicas de Ámbito Financiero utilizando Firecrawl.

Análisis con IA: Un agente de OpenAI analiza la variación matemática entre el primer y el último registro, e intenta correlacionar el cambio de precio con las noticias del día.

Notificación: Envía un correo electrónico automático con el resumen del análisis mediante Gmail.

🛠️ Stack Tecnológico
n8n: Orquestador del flujo de trabajo.

Supabase: Almacenamiento de datos histórico.

Firecrawl: Extracción de contenido web (scraping) optimizado para IA.

OpenAI (GPT-5-mini): Procesamiento de lenguaje natural y análisis económico.

Gmail: Canal de envío de reportes.

📋 Requisitos
Para replicar este flujo, es necesario contar con las siguientes credenciales configuradas en n8n:

API Key de Supabase.

API Key de OpenAI.

API Key de Firecrawl.

Conexión OAuth2 para Gmail.
