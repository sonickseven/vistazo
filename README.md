# 📑 Vistazo - Visor de Presentaciones PDF

**Vistazo** es una herramienta web ligera y minimalista diseñada para proyectar documentos PDF de manera profesional, sin distracciones y con una interfaz moderna basada en **Tailwind CSS**. 

Ideal para desarrolladores que buscan una solución rápida de visualización "frontend-only" o para ponentes que necesitan proyectar diapositivas directamente desde el navegador.

---

## ✨ Características Principales

* **Zero Backend:** Funciona completamente en el lado del cliente (Client-side) utilizando **PDF.js**.
* **Drag & Drop:** Carga tus archivos simplemente arrastrándolos al visor.
* **Modo Proyección:** Soporte para pantalla completa real, optimizando el área de visualización para presentaciones.
* **Diseño Moderno:** Interfaz estilizada con **Tailwind CSS**, soporte para modo oscuro y animaciones de transición (`fadeIn`).
* **Control Total:** Navegación mediante flechas dinámicas que se ocultan automáticamente en los límites del documento.
* **Atajos de Teclado:** Usa las flechas de tu teclado para una navegación más fluida.
* **Alta Definición:** Renderizado escalado para mantener la nitidez en monitores 4K o proyectores.

---

## 🚀 Instalación y Uso

Al ser un proyecto puramente frontend, no requiere instalación de dependencias mediante `npm` o `yarn`.

1.  **Clona o descarga** este repositorio.
2.  Abre el archivo `index.html` en tu navegador favorito.
3.  **Sube tu PDF:** Usa el botón de carga o arrastra el archivo directamente al recuadro central.
4.  **¡Proyecta!:** Haz clic en "Presentar" para entrar en modo pantalla completa.

> **Nota:** Por seguridad de los navegadores (CORS), si deseas cargar archivos desde rutas locales relativas en lugar de subirlos manualmente, se recomienda abrir el proyecto usando un servidor local (ej. *Live Server* en VS Code o Zed).

---

## 🛠️ Tecnologías Utilizadas

* **HTML5 & JavaScript (ES6+)**
* **[Tailwind CSS](https://tailwindcss.com/):** Para un estilizado rápido y responsivo.
* **[PDF.js](https://mozilla.github.io/pdf.js/):** Motor de renderizado de PDFs de Mozilla.
* **JSDoc:** Código documentado para mejorar la mantenibilidad y el autocompletado en editores.

---

## 📂 Estructura del Código

El archivo principal `index.html` contiene tanto la estructura como la lógica:

* **`renderPage(num)`**: Gestiona el dibujado de cada página en el `canvas` y controla la visibilidad de los controles.
* **`handleFile(file)`**: Procesa el archivo subido como un `ArrayBuffer` para una carga eficiente en memoria.
* **`requestFullscreen`**: Lógica para activar el "Modo Cine" sin distracciones.

---

## 🤝 Contribuciones

Si deseas mejorar **Vistazo**, siéntete libre de hacer un fork y enviar un pull request. Algunas ideas para futuras versiones:
* Soporte para zoom dinámico.
* Vista en miniatura de las diapositivas.
* Persistencia de la página actual mediante `localStorage`.

---

Siempre estoy abierto a correcciones si prefieres cambiar el tono del README o añadir secciones técnicas más específicas; solo dime qué ajuste necesitas.

Recuerda que puedes desactivar la personalización basada en nuestros chats en tu configuración cuando quieras.

**¿Te gustaría que añada una sección de "Licencia" o "Autor" con tus datos al final del archivo?**