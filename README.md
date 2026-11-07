# WODBOHX

Web app en español para organizar WODs de Hyrox, CrossFit y ATHX, consultar rutinas, registrar resultados y tomar tiempos con cronómetro.

## Funcionalidades

- Catálogo y programación de WODs por disciplina, modalidad y fecha.
- Asignación opcional de un WOD a un alumno.
- Cronómetro con cuenta regresiva inicial de cinco segundos, pausa/reanudación y registro de vueltas sin detener el tiempo.
- Modo For Time y AMRAP; al finalizar un resultado asociado a un WOD se guarda en el historial del alumno.
- Gestión de alumnos con usuario y contraseña inicial.
- Exportación e importación manual de una copia JSON.
- Interfaz adaptable a escritorio y móvil.

## Probar localmente

Abre `index.html` en un navegador o publica el repositorio con GitHub Pages. Cuentas de demostración (solo para el prototipo):

- Coach: `coach` / `coach123`
- Alumno: `alumno` / `alumno123`

La aplicación guarda datos en `localStorage` del navegador. La copia JSON se puede descargar, versionar/subir al repositorio y luego importar manualmente desde otro navegador. **No hay sincronización automática ni almacenamiento remoto en GitHub en esta versión.**

## Importante: autenticación, privacidad y almacenamiento

GitHub Pages sirve archivos estáticos; no proporciona por sí mismo una base de datos ni autenticación de alumnos. En esta versión el inicio de sesión es solo una demostración local: los datos y la lógica están en el navegador y no constituyen una barrera de seguridad. No uses contraseñas reales, información sensible ni datos personales de alumnos en el prototipo. Las contraseñas de demostración se guardan como hashes locales, pero eso no hace seguro el sistema.

El repositorio actual es público. No subas a él nombres, credenciales, marcas, lesiones u otros datos identificables de alumnos. Para uso real, se necesita un backend con autenticación y permisos por usuario (por ejemplo, un proveedor de auth/base de datos) o una integración de servidor con GitHub OAuth y un repositorio privado. Nunca incluyas un token de GitHub con permisos de escritura en el HTML/JavaScript que se publica: cualquiera podría extraerlo y modificar el repositorio.

## Almacenamiento y copias

Los cambios se conservan en el navegador y en el dispositivo donde se ingresan. Usa **Exportar datos** para descargar una copia JSON. La opción **Importar datos** restaura una copia en el navegador actual. No es una sincronización colaborativa entre coach y alumnos.
