# ✅ Solucionario Oficial: Automatización Pro 2026
## Instructor: Agustín Pizarro

Este documento es para uso exclusivo del instructor o como guía de apoyo para alumnos que hayan completado los retos.

---

### 🟢 Módulo 1: Escritorio
**Reto: Backup Automático**
- **Lógica:** Recorre el escritorio, identifica archivos (no carpetas) y usa `shutil.copy` para duplicarlos en una ruta segura.
- **Dificultad:** ⭐ (Baja)

---

### 🟡 Módulo 2: Web y Comunicación
**Reto: Notificador de Telegram (Batería)**
```python
import psutil
import requests

def enviar_alerta(mensaje):
    token = "TU_BOT_TOKEN"
    chat_id = "TU_CHAT_ID"
    url = f"https://api.telegram.org/bot{token}/sendMessage?chat_id={chat_id}&text={mensaje}"
    requests.get(url)

bateria = psutil.sensors_battery()
if bateria.percent < 20 and not bateria.power_plugged:
    enviar_alerta(f"⚠️ ¡Batería baja! Tienes solo el {bateria.percent}%")
```

---

### 🔴 Módulo 3: IA y Nivel Pro
**Reto: Analista de Sentimiento con GPT**
```python
import openai

openai.api_key = "TU_API_KEY"

def analizar(texto):
    prompt = f"Analiza si el siguiente comentario es Positivo, Negativo o Neutral: {texto}"
    response = openai.ChatCompletion.create(
        model="gpt-3.5-turbo",
        messages=[{"role": "user", "content": prompt}]
    )
    return response.choices[0].message.content

comentario = input("Escribe tu opinión del curso: ")
print(f"Resultado de la IA: {analizar(comentario)}")
```

---
*Fin del Solucionario v1.0*
