# Guía de Configuración de Entornos de Desarrollo

> 📋 **Guía Técnica**: Esta documentación establece los procedimientos para configurar un entorno de desarrollo en C# y otros lenguajes. Incluye las configuraciones necesarias para mantener consistencia en el desarrollo de software.

> **Nota importante**: Este documento se enfoca en aspectos técnicos y procedimientos. Para análisis comparativos, reflexiones personales y conclusiones, utiliza el archivo `CONCLUSIONES_EVALUACION.md`.

**Autores**: [Izan] y [Gonzalo]
**Fecha V0**: [Fecha de entrega inicial]
**Fecha V1**: [Fecha de entrega final]

---

## Visual Studio Code - Entorno Principal

### Instalación y Verificación

**Método de instalación:** Para comenzar con la instalacion debemos buscar en nuestro navegador la pagina de visual studio code, una vez dentro seleccionamos la opcion "Download for Windows"
(screenshots/VSCode_enlace.png)
(screenshots/VSC_SO.png)
**Proceso de instalación:**
- **Descarga:** En cuanto tengamos el archivo de descarga le seleccionamos y abrimos el instalador
- **Opciones del instalador:** Lo primero que tenemos que aceptar es la licencia y le damos a "Next", luego seleccionar la carpeta de destino que puedes dejar la ubicación predeterminada o seleccionar una carpeta diferente donde quieras instalar VS Code. Haz clic en "Next", luego seleccionamos los componentes que queremos agregar en este caso agregamos el path y crear un acceso directo en el escritorio.
Agregar al PATH: Esto permite abrir VS Code desde la línea de comandos.Ahora damos a install y comenzara la instalacion de vs code.
(screenshots/VSC1.png)
(screenshots/VSC2.png)
(screenshots/VSC3.png)
(screenshots/VSC4.png)
(screenshots/VSC5.png)

- **Verificación:** [Cómo verificar que funciona]
Para verificar si vs code funciona lo abrimos desde el acceso directo y comprobamos que se puede acceder y modificar diferentes cosas.

### Uso Básico de VS Code

**Navegación y funcionalidades básicas:**
- Navegación por la interfaz: Tenemos la barra lateral en la que encontramos iconos para acceder a la busqueda o extensiones.Tambien tenemos la area de editor que es la zona que se utiliza para editar el codigo.
- Edición de código: Aqui abrimos un archivo para poder modificar dentro de el su codigo.
- Uso de la paleta de comandos: Para abrir la paleta presionamos Ctrl+Shift+P y una vez dentro ejecutamos comandos.
- Gestión de archivos y carpetas: Para poder gestionar archivos arriba a la izquierda tenemos "File" que si lo abrimos nos salen diferentes opciones ya sean para abrir una carpeta o archivo o para crear uno nuevo.

### Personalización del Entorno

**Configuraciones aplicadas:** 

**Temas e iconos:**
Ejemplos:
- Material Theme, One Dark Pro
- File Icon Theme para mejor identificación de archivos

**Configuración de fuentes:**
Ejemplos:
- Fira Code, JetBrains Mono (con ligaduras)

**Atajos de teclado útiles:**
Ejemplos:
- Ctrl+/ para comentar/descomentar
- Ctrl+Shift+P para paleta de comandos
- Ctrl+` para terminal integrada
- Alt+↑/↓ para mover líneas

**Configuración del editor:**
Ejemplos:
- Formateo automático al guardar
- Detección automática de indentación
- Word wrap para líneas largas

**Terminal integrada:**
Ejemplos:
- PowerShell como terminal predeterminado
- Configuración de perfil personalizado

> **Personaliza según tus necesidades**: Estas son sugerencias basadas en prácticas comunes. Experimenta y documenta las configuraciones que encuentres más útiles para tu flujo de trabajo.> 💼 **Manual de Incorporación**: Esta guía establece los estándares del equipo para configurar entornos de desarrollo en C#. Cualquier nuevo desarrollador debe poder seguir estas instrucciones para configurar su entorno de trabajo de manera consistente con el resto del equipo.

### SDK .NET

**Proceso de instalación:**
1. **Descarga e instalación:** Para empezar con el proceso de instalación, primero habrá que dirigirse a la página https://dotnet.microsoft.com/download
(screenshots/dotnet1.png)
Descargamos el SDK de .NET
(screenshots/dotnet2.png)
Ejecutamos el instalador y procedemos con el asitente 
(screenshots/dotnet3.png)
1. **Verificación:** Para comprobar que se ha instalado correctamente debemos abrir la terminal y ejecutar el comando dotnet --version.
Con este comando debería de aparecer la versión de SDK que se haya instalado.
(screenshots/dotnet4.png)
### Configuración para C#

**Extensiones esenciales:**
- **Soporte oficial para C#**: Extensión que proporciona IntelliSense, debugging y compilación

(screenshots/dotnet5.png)
**Configuraciones específicas para C#:** 
C# Microsoft: Extensión base que cuenta con soporte para el lenguaje.
C# Dev Kit Microsoft: Permitirá gestionar proyectos, Intellinsense, debugging, así como la propia navegación del código.
(screenshots/dotnet6.png)
**Debugging básico:**
- Configuración de puntos de interrupción (breakpoints): Hacer click en el margen izquierdo del editor
- Ejecutar y depurar: Pulsar la tecla f5 o el icono de run and debug
- Inspección: Para inspeccionar las variables visibles en el panel lateral, lo cual sirve para ver los valores en el momento.

> **Enfoque práctico**: Las funcionalidades básicas que usaremos en el día a día serán principalmente SDK .NET +VS Code, con el fin de poder compilar, depurar y ejecutar sin tener qie recurrir a la versión complpeta de VS Code.

### Flujo de Trabajo con C#

**Creación de proyectos:**
[Documentar el proceso para crear proyectos C#]

**Estructura de proyecto:**
```csharp
sharp
string ShowMessage(string name)
{
    return $"Hola {Izan}Bienvenido";
}
Console.WriteLine(ShowMessage(args.Length > 0 ? args[0] : "Nombre1"));
Console.WriteLine(ShowMessage(args.Length > 1 ? args[1] : "Nombre2"));
```

**Compilación y ejecución:**
Para poder llegar a compilar y ejecutar nuestro código haremos lo siguiente: 

-Compilar:
Abrir la terminal de VS Code (Ctrl + `).
Abrir la carpeta en la que se encuentre nuestro proyecto
Una vez hecho esto, ejecutamos el siguiente comando:
 ```
     dotnet build
     ```
-Ejecutar
Una vez hayamos compilado, ejecutaremos este comando para poder ejecutar el código: 
```
     dotnet run
     ```

**Debugging:**
Configuración de launch.json: Ajuste y personalización de las opciones de depuración según el proyecto
Breakpoints: Definición y manejo de puntos de interrupción para detener la ejecución del código
Watch: Incorporación de expresiones para observar sus valores durante la depuración
Call Stack: Revisión y navegación por la pila de llamadas para rastrear la ejecución
Control de ejecución: Comandos para avanzar o retroceder en el flujo (F5, F10, F11, Shift+F11)
Inspección de variables: Consulta de valores en tiempo real desde el panel de variables o al pasar el cursor
Console: Evaluación de expresiones y visualización de resultados en la consola de depuración

---

## Visual Studio - IDE Alternativo

### Instalación

**Proceso de instalación:**
- **Descarga:** Nos dirigiremos a la página https://visualstudio.microsoft.com/es/ 
Se podrá escoger entre la versión Professional o Community, dependiendo de si se quiere usar de forma gratuita o con licencia.
(screenshots/vs1.png)
- **Componentes necesarios:** En el proceso de instalación seleccionaremos la carga de trabajo:
Desarrollo de aplicaciones de escritorio con .NET, utilizando C#, Windows Forms, WPF, el SDK de .NET y sus compiladores.
(screenshots/vs2.png)    
- **Verificación:** 
Abrimos Visual Studio.
Creamos un proyecto C# (por ejemplo, “Aplicación de consola .NET”).
Si el programa compila y muestra “Hello World”, la instalación se completó correctamente.
(screenshots/vs3.png)
### Desarrollo con C#

**Creación de proyecto:**
Abrimos Visual Studio
 Seleccionamos Crear un nuevo proyecto
 Elegimos Amplificación de consola (.NET Core)" como tipo de proyecto
 Configurar el nombre y la ubicación del proyecto
 Hacemos click en "Crear"
(screenshots/vs4.png)
(screenshots/vs5.png)
**Flujo de trabajo básico:**
Escribir código: Utilizamos el editor para escribir nuestro código en C#.
Compilar:Presionamos `Ctrl + Shift + B` o seleccionamos “Compilar” en el menú.
Ejecutar:Presionamos `F5` para ejecutar con depuración o `Ctrl + F5` para hacerlo sin depuración.
Depuración Usamos puntos de interrupción, inspecciones de variables y otras herramientas de depuración integradas.



## Configuración de Lenguaje Adicional

**Lenguaje seleccionado:** Python
**Justificación:** Python es un lenguaje versátil y fácil de aprender, ideal para desarrollo rápido y prototipado.

### Instalación del Entorno

**Runtime/SDK:**
- **Descarga e instalación:** Visitar la página oficial https://www.python.org/downloads/

(screenshots/py1.png)
- **Verificación:**
  - Abrir terminal y ejecutar: `python --version` o `python3 --version`
  - Debe mostrar la versión instalada
### Configuración en VS Code

**Extensiones por lenguaje:**

*Para Java:*
- **Paquete completo de Java**: Incluye compilación, debugging y gestión de proyectos

*Para Python:*
- **Soporte oficial de Python**: Extensión completa con intérprete y debugging

*Para otros lenguajes:*
- Busca la extensión oficial del lenguaje que proporcione soporte completo

**Configuraciones específicas aplicadas:**
[Documentar los ajustes que se realizaron, como configuración del intérprete, formateo automático, linting, etc.]

### Proyecto de Ejemplo

**Código desarrollado:**
```[lenguaje]
// Código de ejemplo aquí
// Comentarios explicativos
```

**Proceso de ejecución:**
[Describir cómo ejecutar el código]

---

## Configuraciones Recomendadas

**Configuraciones generales:**
[Documentar configuraciones que se consideran útiles para cualquier desarrollador]

**Herramientas adicionales:**
[Extensions, herramientas CLI, o utilidades que se consideran beneficiosas]

**Solución de problemas comunes:**
[Problemas frecuentes durante la configuración y sus soluciones]

**Recursos útiles:**
- Enlace [Enlace]: [Descripción]
- Documentación [Documentación]: [Descripción]
