
> **Nota:** La aplicación es un único archivo HTML que contiene todo el código (CSS y JS integrados). No requiere dependencias externas.

---

## 🚀 INSTALACIÓN Y DESPLIEGUE

### Opción 1: Uso local (en tu ordenador)

1. **Descarga el archivo** `herramienta-analisis-ia.html`
2. **Ábrelo con cualquier navegador** (Chrome, Firefox, Edge, etc.)
3. **¡Listo!** No necesita servidor web

### Opción 2: Despliegue en GitHub Pages

1. **Crea un repositorio** en GitHub
2. **Sube el archivo** `herramienta-analisis-ia.html`
3. **Ve a Settings > Pages**
4. **Selecciona la rama** `main` y la carpeta `/root`
5. **Guarda** y obtendrás una URL como: `https://tu-usuario.github.io/tu-repositorio/herramienta-analisis-ia.html`

### Opción 3: Despliegue en Vercel

1. **Conecta tu repositorio** de GitHub a Vercel
2. **Importa el proyecto** (detecta automáticamente HTML estático)
3. **Despliega** en un clic
4. Obtendrás una URL como: `https://tu-proyecto.vercel.app`

### Requisitos mínimos
- Navegador moderno con JavaScript habilitado
- Conexión a Internet para acceder a las IAs
- localStorage disponible (todos los navegadores lo soportan)

---

## ❓ PREGUNTAS FRECUENTES

### ¿Necesito una cuenta en las IAs?
Sí, necesitarás cuentas gratuitas o de pago en las plataformas que quieras usar:
- DeepSeek: Gratuito
- Gemini: Gratuito con cuenta Google
- ChatGPT: Gratuito (versión limitada) o de pago
- Claude: Requiere cuenta

### ¿Dónde encuentro el ISIN de un producto?
- En tu bróker o banco
- Buscando en Google "ISIN de [nombre empresa]"
- En plataformas como Yahoo Finance o Investing.com

### ¿Se guardan las respuestas para siempre?
Las respuestas se guardan en el **localStorage de tu navegador**. Si borras datos de navegación o cambias de dispositivo, se perderán. Puedes hacer backup manual copiando las respuestas a un archivo.

### ¿Puedo usar la aplicación sin Internet?
Puedes generar prompts sin conexión, pero necesitas Internet para:
- Abrir las IAs
- Obtener las respuestas de las IAs

### ¿Los prompts funcionan en cualquier IA?
Sí, están diseñados para funcionar en cualquier IA conversacional. Algunas pueden dar respuestas más detalladas que otras.

### ¿Puedo compartir mis respuestas guardadas?
Las respuestas están en tu navegador y no son compartibles directamente. Puedes:
- Exportarlas manualmente copiando el texto
- Usar la función de edición para guardarlas en un archivo

### ¿La aplicación es gratuita?
**Completamente gratuita**. Solo necesitas las cuentas en las IAs (la mayoría tienen versiones gratuitas).

---

## 🔧 PERSONALIZACIÓN

### Añadir nuevos tipos de análisis
Puedes extender la funcionalidad añadiendo más casos en la función `generarPrompt(numero)`:

```javascript
case 13: // Nuevo análisis
    prompt += `## 🔬 ANÁLISIS PERSONALIZADO
    ... contenido del prompt ...
    `;
    break;
