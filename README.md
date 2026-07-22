# Guía de Configuración: Entorno de Compilación LaTeX (Local)

Instrucciones para configurar un entorno de desarrollo local en Windows para la edición y compilación de documentos LaTeX.

---

## 1. Instalación del Compilador (Motor LaTeX)

Para procesar y compilar archivos `.tex` en Windows, se requiere un motor ejecutable. En este caso utilizaremos **MiKTeX**.

* **Descarga:** [Página oficial de MiKTeX](https://miktex.org/download)
* *Nota:* Sigue el asistente de instalación recomendado de forma predeterminada.

---

## 2. Editores de Texto y Entornos recomendados

Puedes elegir cualquiera de las siguientes alternativas según tu preferencia:

### Opción A: TeXworks (Liviano y Sencillo)
Es un editor liviano y con una interfaz básica e intuitiva, ideal para proyectos sencillos o inicios rápidos.

* **Descarga:** [Página oficial de TeXworks](https://tug.org/texworks/)

### Opción B: Visual Studio Code (Recomendado para uso avanzado)
Si ya utilizas Visual Studio Code, puedes configurarlo como tu entorno principal para redactar LaTeX.

#### 1. Extensión requerida
Instala la extensión principal para el soporte de lenguaje:
* **Nombre:** `LaTeX Workshop`
* **Autor:** *James Yu*

#### 2. Dependencia del entorno (Strawberry Perl)
Para gestionar la automatización de referencias y compilaciones avanzadas (como `latexmk`), se requiere el ejecutable de Perl.

Abre **PowerShell** como administrador y ejecuta el siguiente comando:

```powershell
winget install StrawberryPerl.StrawberryPerl
