# Pruebas Automatizadas 🤖

Guía rápida y sencilla de Ejecución de Pruebas de Chattigo 😉

## Marcas de los tests 🔖

Las marcas especifican la funcionalidad, el nivel o la criticidad de cada prueba. 

### Marcas Generales 🔖

- **critical**: Pruebas críticas que NO pueden fallar en producción. 
- **smoke**: Pruebas básicas que deben funcionar si o sí para empezar a probar un determinado flujo.
- **back**: Pruebas a nivel de API y WebSockets, son las pruebas mas rápidas que se pueden ejecutar.
- **web**: Pruebas a nivel del Frontend de la Aplicación, son pruebas desde el punto de vista del usuario de la plataforma.

### Marcas para pruebas del Agente 🔖
[Repositorio](https://github.com/chattigodev/automation-agente)
- **login**: Pruebas relacionadas con el login en la plataforma.
- **states**: Pruebas relacionadas con los estados del agente (online, descanso, etc.)
- **chat**: Pruebas correpondientes a las funcionalidades que interactuan con un chat.

### Marcas para pruebas de los Canales 🔖
[Repositorio](https://github.com/chattigodev/automation-canales)
- **webchat**: Pruebas del webchat
- **whatsapp**: Pruebas de WhatsApp
- **messenger**: Pruebas de Messenger
- **facebook**: Pruebas de Facebook Muro

### Marcas para pruebas del Supervisor 🔖
[Repositorio](https://github.com/chattigodev/automation-supervisor)
- **login**: Pruebas relacionadas con el login en la plataforma.
- **kpi**: Pruebas del Dashboard de KPI's (Chats cerrados, chat activos por agente, etc.)
- **monitor**: Pruebas relacionadas al monitoreo del agente (chats asignados, etc.) 

## Ejecución de los tests 🚀

Dentro de cada Repositorio (agente, canales, etc.) ir a la sección **Actions** -> **Workflows** -> **Ejecutor de pruebas** -> **Run Workflow**

Se nos desplegará un pequeño formulario con los siguientes campos:

- **Ambiente**: El ambiente dónde queremos correr las pruebas _leones, tigres, panteras, lobos_. OBLIGATORIO❗
- **Marcas**: Las marcas que deseamos ejecutar. Si no se especifica ninguna se ejecutan el 100% de las pruebas de ese repositorio
- **Enviar ejecución a Jira**: Si deseamos que se guarde la ejecución en JIRA Zephyr. (_true/false_)

Hacer click en **run workflow** y LISTO!✅

Si entramos al workflow se nos muestra en tiempo real la ejecución del mismo. Una vez finalizada la ejecución podemos ir al paso llamado _Link Reporte_📌 y se nos mostrará un link al que podremos acceder para visualizar el Reporte de Allure con el status de las pruebas (_imporante estar conectado a la VPN!_)

También podremos acceder al reporte desde el canal de Discord: _automation_tests_ una vez finalizado el workflow.


![Test Runner](https://docs.github.com/assets/cb-22017/images/actions-manually-run-workflow.png)
