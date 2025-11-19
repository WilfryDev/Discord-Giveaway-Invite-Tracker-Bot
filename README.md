# 🤖 Discord Giveaway & Invite Tracker Bot

> **Un sistema avanzado de sorteos y rastreo de invitaciones para comunidades de Discord.**

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python)
![Discord.py](https://img.shields.io/badge/Discord.py-2.0%2B-5865F2?style=for-the-badge&logo=discord)
![Status](https://img.shields.io/badge/Status-Stable-green?style=for-the-badge)

Este bot combina un potente **Tracker de Invitaciones** con un sistema de **Sorteos (Giveaways)** que exige requisitos de invitación para participar. Todo funcionando en tiempo real y estructurado modularmente con Cogs.

---

## ✨ Características Principales

### 🎉 Sistema de Sorteos Avanzado
- **Requisitos de Entrada:** Los usuarios solo pueden participar si cumplen con un número X de invitaciones.
- **Tiempo Real:** El Embed del sorteo actualiza el contador de tiempo cada 5 segundos (sin saturar la API).
- **Botones Interactivos:** Sistema de un clic para participar.
- **Anti-Fraude:** Verifica las invites reales al momento de hacer clic.

### 📈 Tracker de Invitaciones (Logs)
- **Bienvenidas Inteligentes:** Detecta quién invitó al nuevo usuario.
- **Contador Personal:** Muestra cuántas invites tiene el invitador en el mensaje de bienvenida.
- **Caché de Invites:** Sistema optimizado para comparar cambios en las invitaciones.

### ⚙️ Estructura Profesional
- Código limpio y modular usando **Cogs**.
- Configuración centralizada en `main.py`.

---

## 📂 Estructura del Proyecto

El proyecto está organizado para ser escalable:

```text
📦 Tu-Proyecto/
 ├── 📄 main.py           # Archivo principal (Configuración y Arranque)
 ├── 📄 README.md         # Documentación
 └── 📂 cogs/
     ├── 📄 eventos.py    # Lógica del Tracker de Invites y Logs
     └── 📄 sorteos.py    # Lógica de los Sorteos y Comandos
```

🚀 Instalación y Uso1. Requisitos PreviosAsegúrate de tener Python instalado. Luego instala la librería ``discord.py:Bashpip install discord.py``

2. ConfiguraciónAbre el archivo ``main.py`` y edita las siguientes líneas con tus ``datos:Python#`` En ``main.py``

``TOKEN = "TU_TOKEN_DE_DISCORD_AQUI"``
``ID_CANAL_LOGS = 123456789012345678``  # ID del canal para las bienvenidas

Nota: Asegúrate de activar los "Privileged Gateway Intents" (Presence, Server Members, Message Content) en el Discord Developer Portal.

3. Iniciar el Bot Ejecuta el archivo principal desde tu terminal:Bash usando ``python main.py``

🎮 Comandos DisponiblesComando 

 - DescripciónPermiso/sorteo [premio] [tiempo] [invites] Crea un sorteo con cuenta regresiva y requisitos.

👮‍♂️ Admin/invitesMuestra cuántas invitaciones tienes actualmente.👤 Usuario📷 

PrevisualizaciónSorteo en Tiempo Real:El bot crea un panel donde se ve el premio, el host y el tiempo restante actualizándose. Si el usuario no tiene las invites necesarias, el bot le avisará efímeramente.Log de Bienvenida:"📥 ¡Nuevo Miembro! Bienvenido @Usuario. Invitado por @Inviter (Sus Invites: 5)."

---

## 👨‍💻 CréditosDesarrollado con ❤️ y ☕ por WillfryDev. Si usas este código, por favor mantén los créditos en el footer de los embeds.

