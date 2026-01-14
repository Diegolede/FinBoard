<div align="center">
  <img src="src/logo.png" alt="FinBoard Logo" width="180" />
  <h1>FinBoard</h1>
  <p>
    <strong>Tu espacio de trabajo visual definitivo.</strong>
  </p>

  <!-- Badges -->
  <p>
    <img src="https://img.shields.io/badge/Versión-1.0.1-blue?style=for-the-badge" alt="Version" />
    <img src="https://img.shields.io/badge/Hecho%20con-Arch%20Linux-1793d1?style=for-the-badge&logo=archlinux&logoColor=white" alt="Arch Linux" />
    <img src="https://img.shields.io/badge/Editor-VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white" alt="VS Code" />
    <img src="https://img.shields.io/badge/IA-Gemini-8E75B2?style=for-the-badge&logo=googlebard&logoColor=white" alt="Gemini" />
  </p>
  <p>
    <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
    <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
    <img src="https://img.shields.io/badge/Electron-47848F?style=for-the-badge&logo=electron&logoColor=white" alt="Electron" />
    <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
    <img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQLite" />
  </p>
</div>

---

## Descripción 

**FinBoard** es una aplicación de pizarra digital de alto rendimiento diseñada para la productividad y la creatividad. Proporciona un lienzo infinito donde los usuarios pueden organizar ideas, gestionar proyectos y visualizar conceptos. Su arquitectura garantiza rapidez y fluidez, integrando herramientas esenciales en una interfaz moderna y minimalista completamente en español.

<br>
<div align="center">
  <img src="src/captura.gif" alt="Captura de pantalla de FinBoard" width="1000" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);">
  <p><em>Vista general del espacio de trabajo</em></p>
</div>
<br>

## ✨ Funcionalidades

### Herramientas de Creación
*   **Texto Inteligente**: Sistema click-to-create con drag-to-resize para definir el tamaño del texto de forma visual e intuitiva.
*   **Notas Adhesivas**: Creación y edición rápida de notas con soporte para formato de texto, ideales para brainstorming y organización.
*   **Herramientas de Dibujo**: Sistema de trazado a mano alzada con suavizado automático para esquematización clara y profesional.
*   **Gestión de Recursos Visuales**: Importación, redimensionamiento y rotación precisa de imágenes y **GIFs animados** que mantienen su animación en el canvas.

### Organización y Gestión
*   **Lienzo Infinito**: Espacio de trabajo ilimitado que permite expandir diagramas y mapas mentales sin restricciones espaciales.
*   **Agrupación y Jerarquía**: Herramientas avanzadas de selección múltiple, agrupación de elementos y control de orden (Z-Order) para una gestión estructurada del contenido.
*   **Transformaciones Completas**: Drag & drop, resize, rotate con controles precisos y visuales.

### Sistema y Persistencia
*   **Persistencia Local**: Guardado automático de todos los cambios en tiempo real con SQLite, asegurando la integridad de los datos.
*   **Sistema de Historial**: Funcionalidad completa de deshacer y rehacer para un flujo de trabajo flexible y seguro.
*   **Interfaz en Español**: UI completamente traducida con terminología consistente y natural.
*   **Confirmación de Salida**: Modal de confirmación al salir de la aplicación para evitar pérdidas accidentales.

---

## ⌨️ Atajos de Teclado y Controles

Optimiza tu flujo de trabajo con estos controles rápidos:

| Acción | Atajo / Control |
| :--- | :--- |
| **Herramientas** | |
| Seleccionar (Cursor) | <kbd>S</kbd> |
| Texto | <kbd>T</kbd> |
| Dibujar | <kbd>D</kbd> |
| Imagen | <kbd>I</kbd> |
| Nota Adhesiva | <kbd>N</kbd> |
| **Edición** | |
| Deshacer | <kbd>Ctrl</kbd> + <kbd>Z</kbd> |
| Rehacer | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Z</kbd> |
| Eliminar Elemento | <kbd>Supr</kbd> / <kbd>Backspace</kbd> |
| Confirmar Texto | <kbd>Enter</kbd> (al editar) |
| Cancelar / Salir | <kbd>Esc</kbd> |
| **Aplicación** | |
| Salir de la App | <kbd>Ctrl</kbd> + <kbd>Q</kbd> |
| **Navegación** | |
| Zoom | Rueda del Ratón |
| Panoramizar (Moverse) | Click Central + Arrastrar |

---

## 📦 Requisitos y Dependencias

FinBoard se distribuye como un archivo **AppImage** autocontenido. En la mayoría de los entornos de escritorio modernos (GNOME, KDE, XFCE), la aplicación funcionará de inmediato.

La única dependencia del sistema que comúnmente requiere instalación manual en distribuciones recientes (como Ubuntu 22.04+ o Fedora 38+) es la biblioteca **FUSE (Filesystem in Userspace)** en su versión 2, necesaria para montar el archivo AppImage.

### Guía de Instalación de Dependencias

<details>
<summary><strong>Arch Linux / Manjaro</strong></summary>

```bash
sudo pacman -S fuse2
```
</details>

<details>
<summary><strong>Fedora / CentOS / RHEL</strong></summary>

```bash
sudo dnf install fuse
```
</details>

<details>
<summary><strong>Ubuntu 24.04 / Debian 13 (Trixie) y superiores</strong></summary>

En versiones muy recientes, el paquete ha sido renombrado para gestionar la transición de 64 bits:
```bash
sudo apt update
sudo apt install libfuse2t64
```
</details>

<details>
<summary><strong>Ubuntu 20.04 - 23.10 / Debian 11 - 12</strong></summary>

Para versiones estándar recientes:
```bash
sudo apt update
sudo apt install libfuse2
```
</details>

*Nota: El resto de las bibliotecas gráficas (GTK, ALSA, X11) suelen estar preinstaladas en cualquier distribución orientada al escritorio.*

---

## 🚀 Descarga e Instalación

Para utilizar FinBoard en su sistema:

1.  Diríjase a la sección **[Releases](../../releases)** del repositorio.
2.  Descargue la última versión del archivo `.AppImage` (ej. `FinBoard-1.0.1.AppImage`).
3.  Otorgue permisos de ejecución al archivo mediante la terminal:

    ```bash
    chmod +x FinBoard-*.AppImage
    ```

4.  Ejecute la aplicación:

    ```bash
    ./FinBoard-*.AppImage
    ```

---

<div align="center">
  <p>Desarrollado por <strong>Diego Ledesma</strong></p>
  <p><em>Versión 1.0.1 - Enero 2026</em></p>
</div>
