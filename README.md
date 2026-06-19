# 🛡️ Innova Reports

**Plataforma de denuncias anónimas para fortalecer la convivencia escolar en Innova Schools.**

![Status](https://img.shields.io/badge/Status-Active-green) ![Version](https://img.shields.io/badge/Version-1.3-blue) ![License](https://img.shields.io/badge/License-MIT-orange)

---

## 📋 Descripción

**Innova Reports** es una plataforma web diseñada para que los estudiantes de Innova Schools reporten de manera segura y anónima situaciones que afecten la convivencia escolar. El sistema permite a profesores y equipo directivo revisar, gestionar y resolver denuncias de manera organizada.

**Objetivo:** Crear un espacio seguro donde la voz de los estudiantes sea escuchada, sin miedo a represalias.

---

## 🎯 Características Principales

### Para Estudiantes 🎒
- ✅ **Formulario de denuncia en 3 pasos** — Motivo → Lugar → Descripción
- ✅ **4 categorías de denuncia** — Estudiante, Profesor, Convivencia, Otro
- ✅ **Anonimato total** — sin necesidad de datos personales
- ✅ **Número de seguimiento** — para monitorear estado de su denuncia
- ✅ **Panel de Estado** — ver historial de denuncias enviadas
- ✅ **Don Quixote** — mascota con personalidad que guía el proceso
- ✅ **FAQ interactivo** — preguntas frecuentes con respuestas claras

### Para Staff (Profesores/ED) 👨‍🏫
- ✅ **Login seguro** — acceso restringido con credenciales
- ✅ **Dashboard de denuncias** — visualización clara de todas las reportes
- ✅ **Gestión de estado** — cambiar estado (Pendiente → En progreso → Resuelto)
- ✅ **Información completa** — motivo, lugar, fecha, descripción de cada denuncia
- ✅ **Auto-actualización** — se refresca automáticamente cada 5 segundos

### Integraciones 🔗
- ✅ **Google Sheets** — almacenamiento automático en hoja de cálculo
- ✅ **localStorage** — copia local en navegador del estudiante
- ✅ **Interfaz moderna** — diseño inspirado en Innova Family

---

## 🚀 Inicio Rápido

### Requisitos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexión a internet
- Para el almacenamiento en Sheets: una cuenta de Google

### Instalación

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/whistersito/InnovaReports.git
   cd InnovaReports
   ```

2. **Desplegar en GitHub Pages**
   - Sube los archivos HTML, PNG e imágenes a tu repositorio
   - Ve a Settings → Pages → selecciona `main` como rama
   - Tu sitio estará disponible en `https://tuusuario.github.io/InnovaReports`

3. **Conectar Google Sheets** (opcional, para almacenamiento en la nube)
   - Crea un Google Sheet llamado "Innova Reports - Denuncias"
   - Añade encabezados: `Fecha | ID | Motivo | Categoría | Lugar | Descripción | Estado`
   - Abre el editor de Apps Script y despliega la web app
   - Reemplaza la URL en `student.html` línea ~872 con tu URL de Apps Script

---

## 📁 Estructura de Archivos

```
InnovaReports/
├── index.html          # Página principal (selector de rol)
├── student.html        # Panel para estudiantes (formulario + historial)
├── staff.html          # Panel para profesores/ED (login + dashboard)
├── faq.html            # Preguntas frecuentes
├── logo.png            # Logo de Innova Schools (fondo transparente)
├── Donqui.png          # Mascota Don Quixote (fondo transparente)
└── README.md           # Este archivo
```

---

## 🎨 Diseño & UX

### Paleta de Colores
- **Navy Azul** (#1A3A6B) — Primario, confianza
- **Verde Limón** (#6AB42B) — Acento, éxito
- **Naranja** (#F5A623) — Atención, detalles
- **Azul Claro** (#2F80C2) — Secundario
- **Blanco/Gris** — Fondos y textos

### Tipografía
- **Nunito** (900, 800, 700) — Títulos y énfasis
- **Inter** (400, 500) — Cuerpo de texto

### Elemento Especial: Don Quixote 🗡️
- Mascota con personalidad estilo Limbus Company
- 20+ frases motivacionales contextuales
- Guía al usuario en el proceso de denuncia
- Flotante en esquina inferior derecha
- Easter egg: 10 clicks = "Dame un momento que recupero el aliento"

---

## 🔐 Seguridad & Privacidad

### Anonimato Garantizado
- ✅ **Sin campos de identificación** en el formulario
- ✅ **Almacenamiento local** — datos quedan en dispositivo del estudiante
- ✅ **Números de seguimiento anónimos** — formato IR-XXXXXX
- ✅ **Solo staff puede ver datos** tras login seguro

### Credenciales por Defecto (Staff)
```
Usuario: innova
Contraseña: innova2026
```
⚠️ **Cambiar antes de producción**

---

## 📊 Flujo de Denuncia

### Estudiante
```
1. Selecciona categoría (Estudiante/Profesor/Convivencia/Otro)
   ↓
2. Especifica lugar donde ocurrió
   ↓
3. Narra los hechos completos
   ↓
4. ENVIAR → Número de seguimiento
   ↓
5. Panel Estado → historial de denuncias
```

### Staff
```
1. Ir a /staff.html
   ↓
2. Login (innova / innova2026)
   ↓
3. Ver dashboard con todas las denuncias
   ↓
4. Cambiar estado: Pendiente → En progreso → Resuelto
   ↓
5. Auto-refresca cada 5s
```
---

## 📈 Estadísticas del Proyecto

| Métrica | v1.2 | v1.3 |
|---------|------|------|
| **Páginas HTML** | 3 | 4 |
| **Líneas de código CSS** | ~400 | ~1200 |
| **Líneas de código JS** | ~300 | ~900 |
| **Funciones JS** | 2 | 15+ |
| **Animaciones** | 3 | 10+ |
| **Elementos interactivos** | ~10 | ~50+ |

---

## 🚀 Próximas Características (Roadmap)

- [ ] Filtros en dashboard staff (por fecha, categoría, estado)
- [ ] Gráficos de denuncias (dashboards analíticos)
- [ ] Envío de notificaciones por email al staff
- [ ] Campos de notas privadas para staff
- [ ] Más categorías de denuncia configurables
- [ ] Sistema de prioridades (urgencia)
- [ ] Exportar datos a PDF/Excel
- [ ] Acceso a múltiples roles (Admin, Profesor, Psicólogo)
- [ ] Historial de cambios de estado
- [ ] QR para acceder rápido desde celular

---

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Storage**: localStorage, Google Sheets
- **Hosting**: GitHub Pages
- **Backend**: Google Apps Script (para Sheets)
- **Design System**: Colores Innova Schools, Tipografía profesional

---

## 👥 Autores

- **Desarrollo y Diseño**: [Tu nombre aquí]
- **Concepto**: Innova Schools Innovation Program (IP)
- **Inspiración**: Innova Family (diseño UI/UX)

---

## 📝 Licencia

MIT License — Libre para usar, modificar y distribuir

---

## 💬 Contacto & Feedback

Para sugerencias, reportes de bugs o mejoras:
- 📧 Crea un Issue en GitHub
- 💬 Contacta al equipo de Innova Schools

---

## 🎓 Notas para Staff

### Primeros Pasos
1. Accede a `/staff.html`
2. Login: `innova` / `innova2026`
3. ¡Verás todas las denuncias en tiempo real!

### Tips de Uso
- Revisa regularmente el dashboard
- Cambia estado a "En progreso" cuando comiences a investigar
- Cuando resuelvas, marca como "Resuelto"
- Las denuncias se actualizan automáticamente cada 5s
- **Nunca** compartas credenciales de acceso

### Seguridad
- Cambia la contraseña antes de lanzar a producción
- Usa HTTPS cuando sea posible (GitHub Pages lo hace automáticamente)
- Considera agregar 2FA en el futuro

---

## ✨ Agradecimientos

- Innova Schools por inspirar este proyecto
- Don Quixote por ser el mejor companion ⚔️
- Todos los estudiantes que hicieron posible esta plataforma

---

**¡Gracias por usar Innova Reports! Juntos hacemos de Innova un lugar mejor. 🛡️✨**

v1.3 — Junio 2025
