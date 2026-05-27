# 📖 Contenido Maestro: Especialización en Automatización
## By Agustín Pizarro - v1.0 2026

Este documento detalla cada lección con ejemplos prácticos y visuales.

---

## 🟢 MÓDULO 1: PRINCIPIANTE

### Tema 1.1: El Ecosistema Python
Python es el lenguaje rey de la automatización. Su sintaxis limpia permite que nos enfoquemos en la LÓGICA y no en el CÓDIGO.
- **Imagen:** ![Python Logo](https://www.python.org/static/community_logos/python-logo-master-v3-TM.png)

### Tema 1.4: Manipulación de Archivos Pro
Aprenderás a usar la librería `shutil`.
**Ejemplo de código:**
```python
import os, shutil
# Ordena descargas por extensión
for f in os.listdir("Downloads"):
    if f.endswith(".pdf"):
        shutil.move(f, "Documentos/PDFs")
```

---

## 🟡 MÓDULO 2: INTERMEDIO

### Tema 2.1: El Humano Invisible (Selenium)
Configuración de WebDrivers. Cómo evitar que las webs detecten que eres un bot (User-Agents).
- **Imagen:** ![Selenium](https://upload.wikimedia.org/wikipedia/commons/d/d5/Selenium_Logo.png)

### Tema 2.2: Notificaciones en tiempo real
Conexión con Bots de Telegram para recibir alertas de servidores o de precios en tu celular.

---

## 🔴 MÓDULO 3: AVANZADO

### Tema 3.1: Agentes de IA
Uso de la API de OpenAI para toma de decisiones.
**Ejemplo:**
- Input: Email de cliente enojado.
- Bot: Detecta enojo, genera una disculpa y envía cupón de descuento automáticamente.

### Tema 3.4: Despliegue 24/7
Uso de Linux en la nube (VPS) para ejecutar bots que nunca duermen.

---
*Fin del contenido detallado.*
