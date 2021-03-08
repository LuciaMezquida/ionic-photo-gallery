# ionic-photo-gallery
Photo gallery app for mobile devices, using the ionic documentation tutorial.

## Android Studio

Después de desplegar el comando `ionic build`, `ionic cap add android` y `ionic cap open android` para deployar a producción, se abre automáticamente *Android Studio* con el archivo generado. Lo cerramos e importamos el proyecto desde Import Project (Gradle, Eclipse ADT, etc.). Abrimos la carpeta *Android* y listo.

En mi caso tuve que hacer un ajuste pues me aparecía el siguiente error: 

~~~
Gradle sync failed: com.android.tools.idea.gradle.project.sync.idea.issues.SdkPlatformNotFoundException:

Module: 'app' platform 'android-29' not found
~~~

Hubo que abrir *Settings* --> *System settings* --> *Android SDK*. Y en SDK platforms, seleccionar Android 10.0(Q), API Level 29. Y a continuación: *File* --> *Sync project with gradle files*
