# FakeCall Studio — simulador de llamadas (versión 1.1)

Proyecto Android de demostración. Todas las pantallas y acciones son simuladas: la app no realiza llamadas telefónicas reales, no conecta con la red móvil y no activa el micrófono.

## Funciones incluidas

- **Marcador inicial:** permite escribir un número o marcarlo tocando el teclado en pantalla. Incluye borrar dígitos y botón verde para iniciar una llamada simulada.
- **Animación de llamada saliente:** muestra una pantalla de “Llamando…” con avatar animado y permite cancelar.
- **Llamada activa:** cronómetro en tiempo real, avatar con animación suave y botón para finalizar.
- **Controles interactivos:** silenciar (visual), altavoz (visual), teclado en llamada, espera/reanudar, añadir y más. Los controles se animan al pulsarse. El cronómetro continúa en espera.
- **Contactos de muestra:** Mamá, Papá, Hermano, Saúl y Hermana Liz. Sus números son ficticios y se usan únicamente para probar la app.
- **Configuración:** selección de apariencia Android, Samsung, Pixel o iPhone para las pantallas del simulador.
- **Pantalla final:** muestra la duración simulada y permite regresar al marcador o volver a llamar.
- No solicita permisos de llamadas, contactos ni micrófono.

## Requisitos de compilación

- Android Studio reciente.
- JDK 17 (Android Studio puede proporcionar el JDK).
- Conexión a Internet la primera vez para descargar Gradle y dependencias.
- SDK Android 35.

## Abrir, probar y crear el APK

1. Descarga y descomprime `FakeCallStudio.zip`.
2. Abre Android Studio y elige **Open**.
3. Selecciona la carpeta `FakeCallStudio` (la que contiene `settings.gradle.kts`).
4. Espera a que termine **Gradle Sync** e instala los componentes del SDK si te los solicita.
5. Pulsa **Run ▶** para probar la app.
6. Para crear un APK, usa **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
7. Android Studio mostrará una notificación con **Locate**. El APK de depuración suele quedar en `app/build/outputs/apk/debug/app-debug.apk`.

## Identificador y versión

- Paquete: `com.example.fakecallstudio`
- Versión: `1.1` (versionCode 2)

## Limitaciones intencionales

- Es un simulador visual, no un marcador telefónico real.
- Silenciar y altavoz son estados visuales; no controlan el audio del dispositivo.
- Los tonos del teclado durante la llamada solo se muestran en pantalla.
- Los números y contactos de ejemplo no representan contactos de la agenda del teléfono.
