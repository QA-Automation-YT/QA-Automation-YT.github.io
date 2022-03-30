# Pruebas Automatizadas 

Guía rápida y sencilla de Ejecución de Pruebas de Chattigo ;)

## Marcas de los tests

### Marcas Generales

- **critical**: Pruebas críticas que NO pueden fallar en producción. 
- **smoke**: Pruebas básicas que deben funcionar si o sí para empezar a probar un determinado flujo
- **back**: Pruebas a nivel de API y WebSockets, son las pruebas mas rápidas que se pueden ejecutar
- **web**: Pruebas a nivel del Frontend de la Aplicación, son pruebas desde el punto de vista del usuario de la plataforma.

### Marcas para pruebas del Agente
[Repositorio](https://github.com/chattigodev/automation-agente)
- **chat**: Pruebas correpondientes a las funcionalidades que interactuan con un chat
- **login**: Pruebas relacionadas con el login en la plataforma
- **states**: Pruebas relacionadas con los estados del agente (online, descanso, etc.)

### Marcas para pruebas de los Canales
[Repositorio](https://github.com/chattigodev/automation-canales)
- **webchat**: Pruebas del webchat
- **whatsapp**: Pruebas de WhatsApp
- **messenger**: Pruebas de Messenger
- **facebook**: Pruebas de Facebook Muro


![Test Runner](https://docs.github.com/assets/cb-22017/images/actions-manually-run-workflow.png)
