# ÉTICA 360° – ESPRO

**Aplicación web estática lista para usar y publicar en GitHub Pages.** Es un recurso académico de demostración, no un sistema institucional oficial.

## Uso inmediato

Abra `index.html` con Chrome, Edge o Firefox. No necesita instalar Node.js, ejecutar comandos ni conectarse a un servidor. Los seis escenarios y la evaluación funcionan directamente en el navegador.

## Funciones

- Seis escenarios ficticios completos, con tres decisiones sucesivas por caso.
- Historia ramificada: la segunda y tercera escena varían según las decisiones anteriores.
- Retroalimentación inmediata por decisión.
- Nota formativa sobre 5,0 y panel de cinco competencias.
- Modos práctica y evaluación formativa, repetición de casos.
- Exportación local del resultado a CSV (compatible con Excel).
- Interfaz adaptable a móviles y computadores.
- No solicita ni almacena datos personales; al recargar se pierde el avance.

## Publicar en GitHub Pages sin instalar programas

1. Cree un repositorio **público** en GitHub, por ejemplo `simulador-etica-espro`.
2. En **Add file → Upload files**, suba `index.html` desde este paquete a la raíz del repositorio. Es suficiente para publicar la aplicación.
3. En **Settings → Pages**, seleccione **Deploy from a branch**, rama `main` y carpeta `/(root)`. Guarde.
4. Espere a que GitHub termine la publicación y visite `https://USUARIO.github.io/simulador-etica-espro/`.

**Alternativa automatizada:** si sube la carpeta `.github/workflows/deploy.yml` además de `index.html`, puede elegir **GitHub Actions** como origen de Pages. El flujo incluido publica el sitio estático sin compilación.

## Archivos incluidos

- `index.html`: aplicación funcional autónoma. Es el archivo que debe publicar.
- `src/`: código fuente alternativo en React/Vite para futuras ampliaciones.
- `package.json` y `vite.config.js`: entorno opcional de desarrollo React.
- `.github/workflows/deploy.yml`: despliegue opcional mediante GitHub Actions.
- `INSTRUCCIONES_INSTALACION.txt`: guía breve.

## Desarrollo avanzado (opcional)

Con Node.js 22 instalado, puede ejecutar `npm install`, `npm run dev` y `npm run build` para trabajar en la versión React. **La versión publicada por defecto es el archivo autónomo `index.html`; los cambios en `src/` no se reflejan automáticamente en él.** Si modifica los escenarios, deberá actualizar la versión autónoma o configurar el despliegue para compilar React.

## Evaluación y límites

Cada decisión tiene una puntuación pedagógica de 0 a 4. El promedio se contextualiza en cinco indicadores: legalidad (25 %), integridad (25 %), consecuencias (20 %), autocontrol (15 %) y prevención (15 %). La nota se expresa en escala de 5,0. **Los indicadores comparten evidencia y son orientativos, no mediciones independientes ni una evaluación psicológica.**

No se guardan resultados en un servidor ni se implementa autenticación. La modalidad “Evaluación formativa” no es un examen seguro: no hay bloqueo de intentos ni registro docente. Los casos deben revisarse con normativa y procedimientos institucionales vigentes antes de utilizarlos como evaluación oficial.

No incluya datos operativos, información reservada, fotografías personales ni identificadores de estudiantes en un repositorio público. No utilice escudos oficiales sin autorización.
