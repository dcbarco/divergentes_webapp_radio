# 🎵 Radio Divergentes WebApp

Una aplicación web moderna para streaming de radio con integración de IA generativa que proporciona datos curiosos y conexiones inesperadas sobre las canciones.

![Radio Divergentes](https://img.shields.io/badge/Radio-Divergentes-orange?style=for-the-badge)
![Node.js](https://img.shields.io/badge/Node.js-18+-green?style=for-the-badge)
![Express](https://img.shields.io/badge/Express-4.18+-blue?style=for-the-badge)
![Gemini AI](https://img.shields.io/badge/Gemini-AI-red?style=for-the-badge)

## 🌟 Características

- **🎵 Streaming en Vivo**: Reproducción directa desde Zeno.fm
- **🤖 IA Generativa**: Información contextual generada por Gemini AI sobre las canciones
- **📱 Diseño Responsivo**: Optimizado para desktop y móvil
- **🎨 Interfaz Moderna**: UI elegante con TailwindCSS
- **📚 Biblioteca de Podcasts**: Colección de episodios científicos
- **🌙 Fondos Dinámicos**: Imágenes generadas por IA que cambian diariamente

## 🚀 Despliegue

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/divergentes_webapp_radio)

## 📋 Prerrequisitos

- Node.js 18.0.0 o superior
- Una API key de Google Gemini AI

## 🔧 Instalación

### 1. Clona el repositorio
```bash
git clone https://github.com/yourusername/divergentes_webapp_radio.git
cd divergentes_webapp_radio
```

### 2. Instala las dependencias
```bash
npm install
```

### 3. Configura las variables de entorno
```bash
cp .env.example .env
```

Edita el archivo `.env` y configura tu API key de Gemini:
```env
GEMINI_API_KEY=your_gemini_api_key_here
PORT=3000
```

### 4. Obtén tu API Key de Gemini
1. Ve a [Google AI Studio](https://aistudio.google.com/app)
2. Crea una nueva API key
3. Copia la key y pégala en tu archivo `.env`

### 5. Ejecuta la aplicación
```bash
# Modo desarrollo
npm run dev

# Modo producción
npm start
```

## 📖 Uso

### Reproducción de Radio
1. Abre tu navegador en `http://localhost:3000`
2. Haz clic en el botón de play central
3. La radio comenzará a reproducir automáticamente

### Información con IA
Cuando aparezcan metadatos de canción:
1. Haz clic en el ícono 👁️ (Datos Divergentes)
2. Gemini AI generará información contextual sobre la canción
3. Se mostrará en un modal con datos curiosos y conexiones inesperadas

### Podcasts
1. Desplázate hacia abajo y haz clic en "Podcasts"
2. Explora la colección de episodios científicos
3. Haz clic en cualquier podcast para ver detalles
4. Selecciona el idioma y reproduce

## 🏗️ Arquitectura

```
📦 divergentes_webapp_radio
├── 📄 server.js                 # Servidor Express principal
├── 📁 api/
│   └── 📄 get-song-info.js      # API endpoint para Gemini AI
├── 📁 public/
│   ├── 📄 index.html            # Interfaz de usuario principal
│   ├── 📄 style.css             # Estilos CSS adicionales
│   └── 📁 backgrounds/          # Imágenes de fondo dinámicas
├── 📄 package.json              # Configuración del proyecto
├── 📄 .env.example              # Plantilla de variables de entorno
└── 📄 README.md                 # Este archivo
```

## 🔑 API Endpoints

### POST /api/get-song-info
Genera información contextual sobre una canción usando Gemini AI.

**Request Body:**
```json
{
  "prompt": "Descripción de la canción y artista"
}
```

**Response:**
```json
{
  "response": "Información generada por IA sobre la canción"
}
```

## 🎨 Personalización

### Cambiar el Stream de Radio
Edita la constante `STREAM_URL` en `public/index.html`:
```javascript
const STREAM_URL = 'https://tu-stream-url.com';
```

### Modificar Prompts de IA
Personaliza los prompts en `api/get-song-info.js` para cambiar el estilo de las respuestas de IA.

### Agregar Nuevos Podcasts
Edita el array `podcastData` en `public/index.html` para agregar nuevos episodios.

## 🚀 Despliegue en Vercel

### Opción 1: Deploy Automático
1. Conecta tu repositorio de GitHub con Vercel
2. Vercel detectará automáticamente la configuración
3. Configura las variables de entorno en el dashboard de Vercel

### Opción 2: Deploy Manual
```bash
# Instala Vercel CLI
npm i -g vercel

# Despliega
vercel

# Para producción
npm run vercel-deploy
```

### Variables de Entorno en Vercel
En el dashboard de Vercel, agrega:
- `GEMINI_API_KEY`: Tu API key de Gemini
- `PORT`: 3000 (opcional, Vercel lo maneja automáticamente)

## 🐛 Solución de Problemas

### Error de API Key
- Verifica que tu `.env` esté correctamente configurado
- Asegúrate de que la API key de Gemini sea válida
- Reinicia el servidor después de cambiar variables de entorno

### Problemas de Reproducción
- Verifica la conexión a internet
- Revisa que el stream de Zeno.fm esté activo
- Limpia la caché del navegador

### Error 404 en Vercel
- Asegúrate de que `server.js` esté en la raíz del proyecto
- Verifica que Vercel esté configurado para usar Node.js

## 🤝 Contribuir

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está bajo la Licencia ISC. Ver el archivo `LICENSE` para más detalles.

## 🙏 Agradecimientos

- **Centro de Ciencia Francisco José de Caldas** - Por la creación de Divergentes Radio
- **Google Gemini AI** - Por la tecnología de IA generativa
- **Zeno.fm** - Por el servicio de streaming
- **TailwindCSS** - Por el framework de estilos

## 📞 Contacto

**Centro de Ciencia Francisco José de Caldas**
- Website: [www.ciencia.ucaldas.edu.co](https://www.ciencia.ucaldas.edu.co)
- Email: ciencia@ucaldas.edu.co

---

<div align="center">
  <p><strong>🎵 ¡Sintoniza la ciencia, siente la música! 🎵</strong></p>
  <p>Desarrollado con ❤️ por la comunidad científica</p>
</div>