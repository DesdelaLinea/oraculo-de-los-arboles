# 🌿 Oráculo de los Árboles

**Un oráculo interactivo de los 64 árboles sagrados de Colombia — disponible en 9 idiomas.**

> *"La historia de cada árbol refleja la historia de quien consulta."*

---

## ✨ Descripción

El Oráculo de los Árboles es una experiencia digital de introspección basada en la sabiduría de 64 especies arbóreas sagradas de Colombia. Cada árbol porta un mensaje, un arquetipo, una invitación al autoconocimiento.

La aplicación funciona completamente en el navegador, sin conexión a internet, sin servidores, sin datos enviados a ningún lado. Es un archivo HTML único que puedes guardar, compartir y usar para siempre.

---

## 🌐 Demo

👉 **[Abrir el Oráculo](https://desdelalinea.github.io/oraculo-de-los-arboles)**

---

## 🃏 Características

- **64 cartas** con imágenes reales de cada árbol sagrado colombiano
- **9 idiomas** — Español, English, Português, Français, Deutsch, 中文, 日本語, Русский, हिन्दी
- **Lecturas de 3 o 5 cartas** con posiciones interpretativas únicas
- **Animaciones** de mezcla, volteo y revelación de cartas
- **Audio generativo** — binaural 432Hz/440Hz (ondas Theta 8Hz), paisaje sonoro de bosque, notas de hang pan en escala D Dórico
- **Fondo animado** — cielo nocturno, luna, 130 estrellas, silueta de bosque, niebla y 38 luciérnagas
- **URLs compartibles** — cada lectura tiene su propio enlace (`?ids=7,23,41&lang=en`)
- **Detección automática de idioma** del navegador
- **Offline-ready** — un solo archivo HTML de ~5.4 MB, sin dependencias externas en tiempo de ejecución

---

*Cada carta incluye el mensaje oracular completo en los 9 idiomas disponibles.*

---

## 🌍 Idiomas disponibles

| Código | Idioma | Selector |
|--------|--------|----------|
| `es` | Español | predeterminado |
| `en` | English | `?lang=en` |
| `pt` | Português | `?lang=pt` |
| `fr` | Français | `?lang=fr` |
| `de` | Deutsch | `?lang=de` |
| `zh` | 中文 | `?lang=zh` |
| `ja` | 日本語 | `?lang=ja` |
| `ru` | Русский | `?lang=ru` |
| `hi` | हिन्दी | `?lang=hi` |

El idioma se puede cambiar desde el menú desplegable en la esquina superior derecha, o directamente por URL. La selección se guarda en la URL automáticamente.

---

## 🚀 Uso

### Opción 1 — Desde GitHub Pages
Visita el enlace de la demo y úsalo directamente en el navegador.

### Opción 2 — Descarga local
1. Descarga el archivo `oraculo_arboles_v4_multilingual.html`
2. Ábrelo en cualquier navegador moderno
3. No requiere internet, instalación, ni servidor

### Opción 3 — Clonar el repositorio
```bash
git clone https://github.com/desdelalinea/oraculo-de-los-arboles.git
cd oraculo-de-los-arboles
# Abre el archivo HTML en tu navegador
open oraculo_arboles_v4_multilingual.html
```

---

## 🔧 Técnico

El oráculo es una aplicación de **una sola página HTML** sin dependencias externas en tiempo de ejecución.

| Tecnología | Uso |
|-----------|-----|
| HTML5 Canvas | Fondo animado (cielo, bosque, luciérnagas) |
| Web Audio API | Generación de audio procedural (binaural, hang pan, crickets) |
| CSS3 Animations | Flip de cartas, transiciones entre pantallas |
| Vanilla JavaScript | Motor del juego, i18n, generación de URLs |
| Base64 embedded | 64 imágenes JPEG (~3.7 MB) incrustadas en el HTML |

**No usa** frameworks, bundlers, ni llamadas a APIs externas. Funciona en cualquier navegador moderno desde 2018.

### Arquitectura i18n

```
UI_STRINGS        → 9 idiomas × 31 claves de interfaz
CARD_MESSAGES     → 64 cartas × 9 idiomas × mensaje completo
detectLang()      → Lee ?lang= o navigator.language
setLang(código)   → Actualiza UI + URL sin recargar
cardMsg(id)       → Devuelve el mensaje en el idioma activo
```

---

## 📱 Compatibilidad

| Plataforma | Soporte |
|-----------|---------|
| Chrome / Edge | ✅ Completo |
| Firefox | ✅ Completo |
| Safari (iOS & macOS) | ✅ Completo |
| Android Chrome | ✅ Completo |
| Internet Explorer | ❌ No soportado |

---

## 🌱 Origen

Este oráculo está inspirado en la tradición de los oráculos de árboles sagrados de Colombia — una forma ancestral de conectar la naturaleza con el autoconocimiento. Cada árbol es un espejo, cada mensaje una invitación.

El proyecto nació como una herramienta digital de introspección que honra la biodiversidad del bosque colombiano y la sabiduría que cada especie encarna.

---

## 📄 Licencia

Este proyecto es de uso libre para fines personales, educativos y espirituales.

Si compartes o adaptas el oráculo, por favor mantén la atribución a EL oraculo de los árboles. 🌳

---

@musaparadisia & @n33n0
