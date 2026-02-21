+++
date = '2026-02-20T22:46:17-08:00'
draft = false
title = 'Practica 0: Manejo de repositorios'
+++

## Subsecciones
* **Primera sesión:** Sintaxis y uso de Markdown.
* **Segunda sesión:** Uso de Git y GitHub (control de versiones).
* **Tercera sesión:** Generación de páginas estáticas con Hugo y GitHub Actions.
* **Enlaces del proyecto:** Portafolio y página desplegada.

---

## Descripción de la práctica
El objetivo de esta práctica es establecer las bases para el manejo de repositorios, control de versiones y documentación. A lo largo de tres sesiones, aprendimos a formatear texto utilizando Markdown, gestionar nuestros archivos locales y subirlos a la nube mediante Git y GitHub, y finalmente, automatizar la creación y publicación de un sitio web estático utilizando Hugo y GitHub Actions. Este reporte es la primera entrada oficial de nuestro portafolio.

---

## Desarrollo de la práctica

### Primera sesión: Sintaxis y uso de Markdown
**¿Qué es Markdown y cómo se utiliza?**
Markdown es un lenguaje de marcado ligero que nos permite aplicar formato a un texto de manera sencilla utilizando caracteres de texto plano. Se utiliza ampliamente en documentación, archivos `README` y generadores de sitios estáticos porque es fácil de leer tanto para humanos como para computadoras.

**Sintaxis básica:**
* **Títulos:** Se utilizan numerales (`#`). Un `#` es el título principal, `##` para subtítulos, etc.
* **Negritas y cursivas:** Para **negritas** se usan dos asteriscos `**texto**`, y para *cursivas* un solo asterisco `*texto*`.
* **Listas:** Se pueden usar guiones `-` o asteriscos `*` para listas desordenadas, y números `1.` para listas ordenadas.
* **Bloques de código:** Se encierran entre tres comillas invertidas (\`\`\`).
* **Enlaces e imágenes:** `[Texto del enlace](url)` y `![Texto alternativo](url_de_la_imagen)`.
#### Para ver mas contenido de la sintaxis 
[Click aqui]({{< ref "practica0/ayuda.md" >}})

### Segunda sesión: Uso de Git y GitHub
**¿Qué son Git y GitHub?**
* **Git:** Es un sistema de control de versiones local que rastrea los cambios en nuestros archivos a lo largo del tiempo, permitiéndonos volver a versiones anteriores si es necesario.
* **GitHub:** Es una plataforma en la nube que aloja repositorios de Git, facilitando el trabajo colaborativo, el respaldo de la información y la publicación de proyectos.

**Comandos esenciales para subir información:**
Para crear un repositorio local y subirlo a GitHub, seguimos este flujo básico:
1. `git init`: Inicializa un nuevo repositorio de Git en la carpeta actual.
2. `git add .`: Prepara todos los archivos modificados para ser guardados.
3. `git commit -m "Mensaje"`: Guarda los cambios localmente con un mensaje descriptivo.
4. `git branch -M main`: Asegura que la rama principal se llame "main".
5. `git remote add origin <URL>`: Conecta nuestro repositorio local con el repositorio en la nube de GitHub.
6. `git push -u origin main`: Sube nuestros archivos locales a GitHub.

### Tercera sesión: Hugo y GitHub Actions
**¿Qué es Hugo y GitHub Actions?**
* **Hugo:** Es un generador de sitios estáticos (SSG) muy rápido, escrito en Go. Toma nuestros archivos de Markdown y los convierte en páginas HTML listas para la web.
* **GitHub Actions:** Es una herramienta de automatización integrada en GitHub que permite crear flujos de trabajo (workflows) para construir, probar y desplegar código (CI/CD).

**Creación y publicación del sitio:**
1. **Crear el sitio en Hugo:** Usamos comandos como `hugo new site mi-portafolio` para generar la estructura base y añadimos un tema.
2. **Subir a GitHub:** Guardamos todo el proyecto en nuestro repositorio usando los comandos de Git vistos en la sesión dos.
3. **Configurar GitHub Actions:** Creamos un archivo `.yml` en la ruta `.github/workflows/`. Este archivo le indica a los servidores de GitHub que instalen Hugo, construyan la página a partir de nuestros archivos Markdown y envíen el resultado a la rama de **GitHub Pages** para que el sitio quede publicado y accesible en internet.

---

## Enlaces del proyecto
* **Repositorio en GitHub:** https://github.com/Maurongas/PORTAFOLIO-PARADIGMAS
* **Portafolio en GitHub Pages:** https://maurongas.github.io/PORTAFOLIO-PARADIGMAS/

---

## Conclusiones
Esta práctica nos permitió comprender el ciclo completo de desarrollo y despliegue moderno. Desde la redacción de documentación limpia con Markdown, pasando por el respaldo y control de cambios con Git, hasta la automatización del despliegue en la web con Hugo y GitHub Actions. Estas herramientas son fundamentales para mantener proyectos organizados, profesionales y accesibles.