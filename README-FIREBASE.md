# Guía de Despliegue en Firebase Hosting

## 📋 Requisitos Previos

1. **Cuenta de Google**: Necesitas una cuenta de Google
2. **Node.js**: Instala Node.js desde [nodejs.org](https://nodejs.org/) (versión 14 o superior)

## 🚀 Pasos para Desplegar

### Paso 1: Instalar Firebase CLI

Abre PowerShell o Terminal y ejecuta:

```bash
npm install -g firebase-tools
```

### Paso 2: Iniciar Sesión en Firebase

```bash
firebase login
```

Esto abrirá tu navegador para autenticarte con tu cuenta de Google.

### Paso 3: Crear un Proyecto en Firebase Console

1. Ve a [Firebase Console](https://console.firebase.google.com/)
2. Haz clic en **"Agregar proyecto"** o **"Crear un proyecto"**
3. Ingresa un nombre para tu proyecto (ej: "transcripcion-tiempo-real")
4. Opcionalmente, desactiva Google Analytics si no lo necesitas
5. Haz clic en **"Crear proyecto"**
6. Espera a que se complete la creación

### Paso 4: Inicializar Firebase en tu Proyecto Local

En la terminal, navega a la carpeta de tu proyecto:

```bash
cd C:\Users\somar\Documents\sinecta\transcripciontiemporeal
```

Luego ejecuta:

```bash
firebase init hosting
```

**Durante la inicialización, selecciona:**

1. **"Use an existing project"** → Selecciona el proyecto que acabas de crear
2. **"What do you want to use as your public directory?"** → Presiona Enter (usa `.` que es el directorio actual)
3. **"Configure as a single-page app (rewrite all urls to /index.html)?"** → Responde **Y** (Sí)
4. **"Set up automatic builds and deploys with GitHub?"** → Responde **N** (No, a menos que quieras usar GitHub)
5. **"File public/index.html already exists. Overwrite?"** → Responde **N** (No)

### Paso 5: Desplegar tu Aplicación

```bash
firebase deploy --only hosting
```

### Paso 6: Acceder a tu Aplicación

Una vez completado el despliegue, verás una URL similar a:
```
https://tu-proyecto-id.web.app
```
o
```
https://tu-proyecto-id.firebaseapp.com
```

¡Tu aplicación ya está en línea! 🎉

## 🔄 Actualizar tu Aplicación

Cada vez que hagas cambios y quieras actualizar la versión en línea:

```bash
firebase deploy --only hosting
```

## 📝 Comandos Útiles

- **Ver el estado del proyecto**: `firebase projects:list`
- **Ver información del hosting**: `firebase hosting:sites:list`
- **Previsualizar localmente**: `firebase serve` (luego abre http://localhost:5000)
- **Ver logs**: `firebase hosting:channel:list`

## ⚙️ Configuración Personalizada

Si quieres personalizar tu dominio, ve a:
1. Firebase Console → Tu Proyecto → Hosting
2. Haz clic en "Agregar dominio personalizado"
3. Sigue las instrucciones para verificar tu dominio

## 🆘 Solución de Problemas

### Error: "Command not found"
- Asegúrate de que Node.js esté instalado correctamente
- Reinstala Firebase CLI: `npm install -g firebase-tools`

### Error de permisos
- Ejecuta PowerShell como Administrador
- O usa: `npm install -g firebase-tools --force`

### Error al hacer login
- Cierra sesión: `firebase logout`
- Vuelve a iniciar sesión: `firebase login`

## 📚 Recursos Adicionales

- [Documentación de Firebase Hosting](https://firebase.google.com/docs/hosting)
- [Firebase CLI Reference](https://firebase.google.com/docs/cli)

