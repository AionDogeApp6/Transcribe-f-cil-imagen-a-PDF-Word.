# Transcribe-f-cil-imagen-a-PDF-Word

**Transcribe Fácil** es una aplicación web responsiva, moderna y ligera diseñada para la extracción, edición y conversión de texto a partir de fuentes visuales (**imágenes, fotos de documentos, libros o capturas de pantalla**). 

Optimizada con una interfaz premium en modo oscuro, la aplicación realiza todo el procesamiento en el lado del cliente (directamente en el navegador), permitiendo moldear la información extraída mediante roles profesionales y dialectos de Venezuela, para luego exportarla a archivos **PDF**, **Word** o compartirla de forma inmediata por **WhatsApp**.

---

## 🎯 Características Principales

*   **Extracción OCR en Navegador:** Captura imágenes o fotografías de documentos e indexa el texto alfanumérico en tiempo real sin necesidad de servidores externos.
*   **Editor Interactivo Premium:** Una interfaz estilizada en modo oscuro que permite corregir, adaptar o maquetar el texto extraído antes de generar el archivo final.
*   **Homologación de Diálogos por Profesiones:** Cuenta con un set de configuraciones de lenguaje técnico adaptables según el perfil seleccionado al inicio del documento:
    *   *Ingeniero, Abogado, Doctor, Científico, Matemático, Docente, Policía, etc.*
*   **Filtros de Identidad y Dialecto Venezolano:** Modifica las aperturas (saludos) y cierres (despedidas) adaptándose a la jerga y cultura de las distintas regiones de Venezuela:
    *   *Guaro, Maracucho, Caraqueño, Oriental.*
   
*   **Exportación Directa:**
    *   **PDF:** Generación de documentos listos para lectura o catálogos limpios.
    *   **Word (.docx):** Exportación estructurada para modificaciones formales.
*   **Conectividad con WhatsApp:** Botón directo para compartir el bloque de texto transcrito o adaptado con un solo toque.

---

## 🛠️ Stack Tecnológico (Basado en CDN)

La arquitectura del proyecto destaca por ser completamente portable, ideal para visualizarse y editarse en entornos móviles (**Acode** / **Termux**) al no requerir dependencias pesadas de backend:

*   **HTML5 / CSS3 (Variables nativas):** Paleta de colores en modo oscuro premium para cuidar la vista durante el desarrollo nocturno.
*   **Tesseract.js (v4.0.1 via unpkg CDN):** Motor de reconocimiento óptico de caracteres (OCR) ejecutado directamente en el cliente.
*   **html2pdf.js (via cdnjs):** Librería encargada de convertir el flujo de texto estructurado del editor en documentos PDF descargables de alta calidad.
*   **JavaScript Nativo (ES6):** Manejo de los diccionarios de roles profesionales, módulos dialectales de apertura/cierre y el formateo de salida para Word y WhatsApp.

---

## ⚙️ Estructura del Archivo Principal

El núcleo del sistema se encuentra concentrado de forma eficiente para garantizar portabilidad:

```text
Transcribe-f-cil-imagen-a-PDF-Word/
├── index.html        # Estructura del sitio, estilos Premium CSS y lógica JavaScript (OCR + Exporters)
└── README.md         # Documentación del repositorio
