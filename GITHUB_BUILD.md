# Compilar FakeCall Studio con GitHub Actions

Este proyecto incluye el flujo `.github/workflows/build-apk.yml`, que compila el APK de depuración automáticamente.

## Pasos desde el celular
1. Descarga y descomprime `FakeCallStudio_v1.1_GitHub.zip`.
2. En GitHub, crea un repositorio nuevo llamado `FakeCallStudio`. Puedes dejarlo privado.
3. Sube el CONTENIDO de la carpeta `FakeCallStudio` al repositorio (incluida la carpeta oculta `.github`). No subas la carpeta contenedora adicional; en la raíz del repositorio deben verse `settings.gradle.kts`, `build.gradle.kts`, `app/` y `.github/`.
4. Abre la pestaña **Actions** del repositorio y habilita Actions si GitHub te lo solicita.
5. El flujo se ejecuta al subir a `main` o `master`. También puedes entrar a **Actions → Compilar APK Android → Run workflow**.
6. Cuando termine en verde, abre la ejecución y baja el artefacto **FakeCallStudio-APK**. Descomprime el ZIP del artefacto para obtener `app-debug.apk`.
7. Abre `app-debug.apk` en Android y acepta instalar desde esa fuente si el sistema lo solicita.

## Notas
- Es un APK de depuración firmado con una clave de depuración generada por Gradle; sirve para instalación y pruebas, no es una versión de publicación en Play Store.
- Si la compilación falla, abre la ejecución de Actions y revisa el paso **Compilar APK**; el error mostrará la causa.
- La aplicación solo simula llamadas y no realiza llamadas telefónicas reales.
