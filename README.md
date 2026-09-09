# Dossier de Revisión IA — Colegio San Ignacio de Loyola

Revisión de las disposiciones institucionales sobre uso responsable y ético de la
Inteligencia Artificial, año escolar 2026-2027. **Borrador para discusión.**

Preparado por Prof. Guillermo Núñez · 9 de septiembre de 2026

---

## Qué contiene

Un solo archivo, `index.html`, autocontenido: 28 hallazgos filtrables por prioridad
y buscables, el lenguaje normativo propuesto para cada uno, la escala IA-0 a IA-4,
la validación de las 16 observaciones y un plan de acción de 25 tareas.

No requiere servidor, base de datos ni proceso de build. Funciona igual servido por
GitHub Pages o abierto directamente desde el disco (doble clic).

## Cómo funciona el plan de acción

El avance se guarda en el `localStorage` del navegador de cada lector, así que es
**por persona y por navegador**. Para compartirlo se usa el botón *Copiar enlace con
este avance*: el estado se codifica dentro del propio enlace (`#plan=...`), de modo
que quien lo abra ve ese avance y queda guardado en su navegador. No hay servidor
de por medio y por tanto no hay estado compartido en vivo: si dos personas marcan
tareas a la vez, cada una tiene su copia hasta que alguien comparta su enlace.

## Publicar en GitHub Pages

### Opción A — desde la web de GitHub, sin terminal

1. En GitHub: **New repository**. Nombre sugerido: `csi-ia-revision`.
   Elige la visibilidad con cuidado (ver la advertencia abajo).
2. En el repo nuevo: **Add file → Upload files** y sube `index.html`.
   **Commit changes**.
3. **Settings → Pages**. En *Build and deployment*, Source: **Deploy from a branch**;
   Branch: **main**, carpeta **/ (root)**. **Save**.
4. Espera uno o dos minutos. El sitio queda en:
   `https://<tu-usuario>.github.io/csi-ia-revision/`

### Opción B — desde la terminal

```bash
cd csi-ia-pages
git init -b main
git add index.html README.md
git commit -m "Dossier de revisión de la política de IA — borrador para discusión"
git remote add origin https://github.com/<tu-usuario>/csi-ia-revision.git
git push -u origin main
```

Luego habilita Pages en **Settings → Pages** como en el paso 3 de la opción A.

### Para actualizar

Reemplaza `index.html` y vuelve a hacer commit y push (o súbelo de nuevo por la web).
Pages redespliega solo. El enlace no cambia.

---

## Advertencia de visibilidad — leer antes de publicar

**Un sitio de GitHub Pages es público en Internet, incluso si el repositorio es
privado.** Restringir el acceso a un sitio de Pages requiere GitHub Enterprise
Cloud; en los planes Free, Pro y Team no existe esa opción. Poner el repo en privado
oculta el código, no la página publicada.

Este documento cita textualmente disposiciones de los manuales internos del Colegio,
menciona un correo institucional (`aimteam@sanignacio.pr`) y está marcado como
borrador para discusión. Antes de publicarlo en un URL público conviene considerar:

- que el Colegio conozca y autorice la publicación, dado que el contenido es
  institucional y el documento aún no ha sido discutido;
- que las citas de los manuales queden como referencias (manual y página) en lugar
  de texto completo, si el documento va a quedar accesible al público;
- retirar el correo institucional del texto;
- si solo se necesita que personas fuera de la organización lo lean, enviarles el
  archivo `index.html` por correo cumple lo mismo sin exponerlo en Internet: se abre
  con doble clic, conserva la interactividad completa y funciona sin conexión.

La etiqueta `<meta name="robots" content="noindex, nofollow">` ya está incluida y
pide a los buscadores no indexar la página. Es una petición que los buscadores
grandes respetan, **no** un control de acceso: cualquiera con el enlace entra.

---

## Fuentes

Documentos institucionales del Colegio San Ignacio de Loyola (compendio de
disposiciones sobre IA de 14 de agosto de 2026, Manual del Estudiante, Manual de la
Facultad y del Personal Administrativo Académico, Manual del Educador Ignaciano,
orientación al personal de la fase de implementación, y Repositorio de Herramientas
de IA), más las guías de citación de APA y MLA, el informe *Copyright and Artificial
Intelligence, Part 2: Copyrightability* de la U.S. Copyright Office, y la
legislación de Puerto Rico referenciada en el propio documento.

Este documento no constituye asesoría legal.
