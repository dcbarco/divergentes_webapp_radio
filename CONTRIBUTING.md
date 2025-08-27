# 🤝 Guía de Contribución - Radio Divergentes

¡Gracias por tu interés en contribuir a Radio Divergentes! Este proyecto es una iniciativa del Centro de Ciencia Francisco José de Caldas para democratizar el acceso a la ciencia y la cultura.

## 📋 Cómo Contribuir

### 1. Preparación del Entorno

```bash
# Clona el repositorio
git clone https://github.com/yourusername/divergentes_webapp_radio.git
cd divergentes_webapp_radio

# Configura Node.js (opcional, usa nvm)
nvm use

# Instala dependencias
npm run setup

# Configura variables de entorno
cp .env.example .env
# Edita .env con tu API key de Gemini
```

### 2. Desarrollo Local

```bash
# Ejecuta en modo desarrollo
npm run dev

# O con recarga automática (si tienes nodemon)
npm run dev:watch
```

### 3. Estructura del Proyecto

```
📦 divergentes_webapp_radio
├── 📄 server.js                 # 🖥️  Servidor Express
├── 📁 api/
│   └── 📄 get-song-info.js      # 🤖 API Gemini AI
├── 📁 public/
│   ├── 📄 index.html            # 🎨 Interfaz principal
│   └── 📄 style.css             # 🎨 Estilos adicionales
├── 📄 vercel.json               # 🚀 Configuración Vercel
└── 📄 package.json              # 📦 Dependencias y scripts
```

## 🎯 Áreas de Contribución

### 🎵 Mejoras de Audio
- Nuevos formatos de streaming
- Mejor gestión de metadatos
- Controles de reproducción avanzados

### 🤖 Inteligencia Artificial
- Nuevos modelos de IA
- Prompts más creativos
- Integración con otras APIs de IA

### 🎨 Interfaz de Usuario
- Nuevos temas visuales
- Mejor experiencia móvil
- Animaciones y transiciones

### 📚 Contenido
- Nuevos podcasts científicos
- Categorización de contenido
- Sistema de búsqueda

### 🚀 Infraestructura
- Optimización de rendimiento
- Nuevas plataformas de despliegue
- Monitoreo y logging

## 🔧 Estándares de Código

### JavaScript/Node.js
- Usa ES6+ features
- Comentarios descriptivos en español
- Manejo de errores robusto
- Funciones pequeñas y modulares

### HTML/CSS
- Semántica correcta
- Responsive design
- Accesibilidad (WCAG 2.1)
- Performance optimizada

### Git
```bash
# Flujo de trabajo recomendado
git checkout -b feature/nueva-funcionalidad
# ... desarrollo ...
git add .
git commit -m "✨ Agrega nueva funcionalidad X"
git push origin feature/nueva-funcionalidad
# Abre Pull Request
```

## 🐛 Reportar Bugs

1. **Verifica** que el bug no haya sido reportado
2. **Usa la plantilla** de issue de GitHub
3. **Proporciona**:
   - Descripción clara del problema
   - Pasos para reproducir
   - Información del entorno (OS, navegador, versión)
   - Screenshots si aplica

## 💡 Proponer Nuevas Funcionalidades

1. **Discute primero** en Issues con etiqueta `enhancement`
2. **Describe** el problema que soluciona
3. **Considera** alternativas existentes
4. **Especifica** el comportamiento esperado

## 📝 Licencia

Al contribuir, aceptas que tus contribuciones serán licenciadas bajo la **Licencia ISC**.

## 🎯 Valores del Proyecto

- **🌍 Acceso Universal**: Ciencia para todos
- **🤝 Colaboración**: Comunidad científica abierta
- **🎨 Creatividad**: Enfoque artístico e innovador
- **📚 Educación**: Divulgación científica de calidad
- **🌱 Sostenibilidad**: Código mantenible y escalable

## 📞 Contacto

- **Centro de Ciencia**: ciencia@ucaldas.edu.co
- **Issues**: [GitHub Issues](https://github.com/yourusername/divergentes_webapp_radio/issues)
- **Discusiones**: [GitHub Discussions](https://github.com/yourusername/divergentes_webapp_radio/discussions)

---

<div align="center">
  <p><strong>🚀 ¡Tu contribución hace la diferencia!</strong></p>
  <p>Gracias por ayudar a construir el futuro de la comunicación científica 🎵</p>
</div>