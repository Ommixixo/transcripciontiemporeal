# 🎤 AI Transcriptor - Transcripción de Voz en Tiempo Real

Una aplicación web moderna que utiliza tecnología de reconocimiento de voz para transcribir audio en tiempo real. Desarrollada con un enfoque en IA y diseño responsivo.

![Firebase Hosting](https://img.shields.io/badge/Firebase-Hosting-orange)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)

## 🌟 Características

- ✅ **Transcripción en Tiempo Real**: Convierte tu voz en texto instantáneamente
- ✅ **Comando de Voz**: Di "terminar" para detener la grabación automáticamente
- ✅ **Diseño Moderno**: Interfaz elegante con enfoque en IA
- ✅ **Totalmente Responsivo**: Funciona perfectamente en móviles, tablets y desktop
- ✅ **Descarga de Texto**: Guarda tus transcripciones en formato .txt
- ✅ **Barra de Navegación**: Diseño moderno y funcional
- ✅ **Colores Sólidos**: Diseño limpio y profesional

## 🚀 Demo en Vivo

Visita la aplicación en: [https://transcriptor-c2f6e.web.app](https://transcriptor-c2f6e.web.app)

## 📋 Requisitos

- **Navegador**: Google Chrome, Microsoft Edge, o cualquier navegador basado en Chromium
- **Conexión a Internet**: Requerida para el reconocimiento de voz
- **Permisos de Micrófono**: El navegador solicitará permiso para acceder al micrófono

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura de la aplicación
- **CSS3 / Tailwind CSS**: Estilos y diseño responsivo
- **JavaScript**: Lógica de transcripción y funcionalidad
- **Web Speech API**: Reconocimiento de voz del navegador
- **Firebase Hosting**: Alojamiento y despliegue

## 📦 Instalación Local

Si deseas ejecutar el proyecto localmente:

1. **Clona o descarga el repositorio**
   ```bash
   git clone https://github.com/Ommixixo/transcripciontiemporeal.git
   cd transcripciontiemporeal
   ```

2. **Abre el archivo index.html**
   - Simplemente abre `index.html` en tu navegador
   - O usa un servidor local:
     ```bash
     # Con Python
     python -m http.server 8000
     
     # Con Node.js (http-server)
     npx http-server
     ```

3. **Accede a la aplicación**
   - Abre tu navegador y ve a `http://localhost:8000`

## 🎯 Uso

### Iniciar Transcripción

1. Haz clic en el botón **"Iniciar Grabación"**
2. Permite el acceso al micrófono cuando el navegador lo solicite
3. Comienza a hablar - verás el texto aparecer en tiempo real

### Detener Transcripción

Tienes dos opciones:

- **Manual**: Haz clic en el botón **"Detener Grabación"**
- **Por Voz**: Di la palabra **"terminar"** y la grabación se detendrá automáticamente

### Guardar Transcripción

1. Una vez detenida la grabación, haz clic en **"Guardar (.txt)"**
2. El archivo se descargará automáticamente con el nombre `transcripcion_YYYY-MM-DD.txt`

## 🔧 Configuración

### Idioma

El reconocimiento está configurado para español de España (`es-ES`). Para cambiar el idioma, edita la línea en el código:

```javascript
recognition.lang = 'es-ES'; // Cambia a 'en-US', 'fr-FR', etc.
```

## 📱 Compatibilidad

### Navegadores Soportados

- ✅ Google Chrome (recomendado)
- ✅ Microsoft Edge
- ✅ Opera
- ✅ Otros navegadores basados en Chromium
- ❌ Firefox (soporte limitado)
- ❌ Safari (soporte limitado)

### Dispositivos

- ✅ Desktop (Windows, macOS, Linux)
- ✅ Tablets
- ✅ Móviles (Android, iOS)

## 🚀 Despliegue en Firebase

Este proyecto está configurado para desplegarse en Firebase Hosting. Para más detalles, consulta [README-FIREBASE.md](README-FIREBASE.md)

### Despliegue Rápido

```bash
firebase deploy --only hosting
```

## 📝 Estructura del Proyecto

```
transcripciontiemporeal/
│
├── index.html              # Archivo principal de la aplicación
├── firebase.json           # Configuración de Firebase Hosting
├── .firebaserc             # Configuración del proyecto Firebase
├── .gitignore              # Archivos ignorados por Git
├── README.md               # Este archivo
├── README-FIREBASE.md      # Guía de despliegue en Firebase
└── PROTECCION.md           # Nota sobre protección del código
```

## 🔒 Protección del Código

Este proyecto incluye medidas básicas de protección para dificultar el acceso casual al código. **Importante**: Es técnicamente imposible ocultar completamente el código del lado del cliente. Para más detalles sobre las limitaciones, consulta [PROTECCION.md](PROTECCION.md).

## 🎨 Personalización

### Colores

Los colores principales están definidos en el CSS:

- **Color Principal**: `#667eea` (Indigo)
- **Fondo**: `#667eea`
- **Texto**: Grises y blancos según el contexto

### Fuentes

- **Principal**: Inter (Google Fonts)
- **Títulos**: Space Grotesk (Google Fonts)

## ⚠️ Limitaciones

- Requiere conexión a internet para el reconocimiento de voz
- Funciona mejor en navegadores basados en Chromium
- La precisión depende de la calidad del micrófono y el ruido ambiental
- Algunos navegadores pueden tener limitaciones de privacidad

## 🔒 Privacidad

- **No almacenamos tus grabaciones**: Todo el procesamiento se hace localmente en tu navegador
- **Sin servidor**: El reconocimiento de voz utiliza la API del navegador
- **Sin cookies**: No se utilizan cookies de seguimiento

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 👨‍💻 Autor

Desarrollado con ❤️ para facilitar la transcripción de voz en tiempo real.

## 📞 Soporte

Si tienes problemas o preguntas:

- Abre un [Issue](https://github.com/Ommixixo/transcripciontiemporeal/issues) en GitHub
- Revisa la documentación de [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)

## 🙏 Agradecimientos

- [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API) por la funcionalidad de reconocimiento de voz
- [Tailwind CSS](https://tailwindcss.com/) por el framework de estilos
- [Firebase](https://firebase.google.com/) por el hosting gratuito

---

⭐ Si este proyecto te fue útil, ¡considera darle una estrella en GitHub!

