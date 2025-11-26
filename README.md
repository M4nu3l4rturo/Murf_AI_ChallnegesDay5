# 🤖 MurfAI Voice Agent Starter (Python/React)

Este repositorio contiene el código de inicio para un agente de voz de LiveKit con un frontend en Next.js (React) y un backend de agente en Python, usando servicios de Murf (TTS), Deepgram (STT) y Google (LLM).

## 🌟 Resumen del Proyecto

Este agente está configurado para participar en una sala de LiveKit. Cuando un usuario se conecta a la aplicación web, el agente se une automáticamente, puede escuchar la voz del usuario (Deepgram), procesar la solicitud (Gemini) y responder con voz de alta calidad (Murf TTS).

| Componente | Tecnología | Propósito |
| :--- | :--- | :--- |
| **Frontend** | Next.js (React) | Interfaz de usuario para conectarse a la sala de LiveKit. |
| **Backend** | Python (`uv`) | El agente de voz principal que maneja STT, LLM y TTS. |
| **STT** | Deepgram | Transcripción de voz a texto. |
| **LLM** | Google Gemini | Procesamiento de lenguaje natural y generación de respuestas. |
| **TTS** | Murf AI | Síntesis de texto a voz con voces inmersivas. |

---

## 🛠️ Instalación y Configuración

Necesitas instalar las dependencias de Python y Node.js para que el agente y el frontend funcionen.

### 1. Claves de API (Archivo `.env.local`)

Crea un archivo llamado **`.env.local`** en la **raíz de tu proyecto** y añade todas tus claves de API.

```ini
# LiveKit Cloud (Necesario para Frontend y Backend)
LIVEKIT_URL=wss://murfai-challenge-dn08ikrp.livekit.cloud
LIVEKIT_API_KEY=APIjcGHrHuMp5AL
LIVEKIT_API_SECRET=mkNzWzIwdVjUOKOrkpnzLnlk05FRvKRTqraRASynd1D

# Servicios de Voz y Lenguaje (Necesario solo para Backend/Agente)
DEEPGRAM_API_KEY=YOUR_DEEPGRAM_API_KEY_HERE
MURF_API_KEY=YOUR_MURF_API_KEY_HERE
GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY_HERE
