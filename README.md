> **Sistema profesional de Giveaways & Tracking para Discord.**
> *Desarrollado por xPlugins*

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python)
![Discord.py](https://img.shields.io/badge/Discord.py-2.0%2B-5865F2?style=for-the-badge&logo=discord)
![Status](https://img.shields.io/badge/Status-Stable-green?style=for-the-badge)

**Strafe Studios Bot** es una solución completa para comunidades que buscan crecimiento real. Combina un rastreador de invitaciones inteligente (detecta Fakes y Salidas) con un sistema de sorteos que exige requisitos de invitación y roles específicos para participar.

---

## ✨ Características Principales

### 🎉 Sistema de Sorteos (Giveaways)
- **Requisitos Dinámicos:** Configura cuántas invites necesita un usuario para entrar.
- **[NUEVO] Roles Opcionales:** Ahora puedes restringir sorteos a roles específicos (ej: Sorteo solo para VIPs).
- **Tiempo Real:** El panel se actualiza cada 5 segundos mostrando la cuenta regresiva.
- **Embeds Premium:** Diseño dorado y limpio al anunciar ganadores.

### 📈 Tracker Inteligente (Logs)
- **Base de Datos JSON:** Guarda estadísticas persistentes.
- **Estadísticas Reales:**
  - ✅ **Joins:** Entradas totales.
  - ❌ **Left:** Usuarios que se salieron (se restan de las invites reales).
  - 🤖 **Fake:** Cuentas creadas hace menos de 7 días.
  - 🔄 **Rejoins:** Usuarios que volvieron a entrar.

### 📚 Utilidades
- **Ayuda Híbrida:** Funciona tanto con `/ayuda` (Slash) como con `!ayuda` (Prefix).
- **Modularidad:** Código organizado en Cogs (`eventos`, `sorteos`, `general`).

---

## 📂 Estructura del Proyecto

```text
📦 Tu-Carpeta-Bot/
 ├── 📄 main.py           # Núcleo del bot y configuración
 ├── 📄 tracking.json     # Base de datos automática (se crea sola)
 ├── 📄 README.md         # Documentación
 └── 📂 cogs/
     ├── 📄 eventos.py    # Tracker de Invites, Logs y DB
     ├── 📄 sorteos.py    # Sistema de Sorteos con Botones
     └── 📄 general.py    # Comandos de Ayuda e Información
```
🚀 Instalación y Uso1. RequisitosNecesitas tener Python 3.9+ instalado.Instala las dependencias:Bashpip install discord.py

2. ConfiguraciónEdita el archivo main.py:PythonTOKEN = "TU_TOKEN_AQUI"
ID_CANAL_LOGS = 123456789012345678  # ID del canal para logs de bienvenida

Importante: Activa los "Privileged Gateway Intents" (Presence, Server Members, Message Content) en el Discord Developer Portal.3. EjecuciónBashpython main.py

🎮 Comandos Disponibles👮‍♂️ Administración (Staff)
ComandoArgumentosDescripción/sorteopremio duracion invites [rol]Crea un sorteo. El campo [rol] es opcional; úsalo para sorteos exclusivos.👤 Usuarios (Público)ComandoDescripción/ayuda o !ayudaMuestra el panel de ayuda con los comandos./invites(Próximamente) Muestra tus estadísticas de invitaciones.📄 

Licencia & CréditosEste proyecto está bajo la Licencia MIT.PlaintextMIT License
Copyright (c) 2025 Strafe Studios.

Desarrollado con ❤️ por WillfryDev.
