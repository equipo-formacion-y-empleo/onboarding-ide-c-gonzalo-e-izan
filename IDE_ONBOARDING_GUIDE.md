# Guía de Configuración de Entornos de Desarrollo

> 📋 **Guía Técnica**: Esta documentación establece los procedimientos para configurar un entorno de desarrollo en C# y otros lenguajes. Incluye las configuraciones necesarias para mantener consistencia en el desarrollo de software.

> **Nota importante**: Este documento se enfoca en aspectos técnicos y procedimientos. Para análisis comparativos, reflexiones personales y conclusiones, utiliza el archivo `CONCLUSIONES_EVALUACION.md`.

**Autores**: [Izan] y [Gonzalo]  
**Fecha V0**: [Fecha de entrega inicial]  
**Fecha V1**: [Fecha de entrega final]

---

## Visual Studio Code - Entorno Principal

### Instalación y Verificación

**Método de instalación:** Para comenzar con la instalación debemos buscar en nuestro navegador la página de Visual Studio Code, una vez dentro seleccionamos la opción "Download for Windows"

(/screenshots/VSCode_enlace.png) 
(/screenshots/VSCode_SistemaOperativo.png)
(/screenshots/VSCode_Archivo.png)
**Proceso de instalación:**
- **Descarga:** En cuanto tengamos el archivo de descarga le seleccionamos y abrimos el instalador
- **Opciones del instalador:** Lo primero que tenemos que aceptar es la licencia y le damos a "Next", luego seleccionar la carpeta de destino que puedes dejar la ubicación predeterminada o seleccionar una carpeta diferente donde quieras instalar VS Code. Haz clic en "Next", luego seleccionamos los componentes que queremos agregar en este caso agregamos el path y crear un acceso directo en el escritorio.

Agregar al PATH: Esto permite abrir VS Code desde la línea de comandos.Ahora damos a install y comenzara la instalacion de vs code.

(/screenshots/VSCode_Terminos.png)  
(/screenshots/VSCode_Terminos1.png)  
(/screenshots/VSCode_Terminos2.png)
(/screenshots/VSCode_Terminos4.png)
(/screenshots/VSCode_Terminos5.png)

---

# Uso Básico de VS Code

**Abrir una carpeta de proyecto**:

Haz clic en File > Open Folder (o presiona Ctrl + K, Ctrl + O)
Navega hasta la carpeta de tu proyecto
Selecciona la carpeta y haz clic en "Seleccionar carpeta"

(/screenshots/VSBarralateral.png)

**Crear un nuevo archivo**:

Haz clic derecho en el explorador de archivos (barra lateral izquierda)
Selecciona "New File" (o presiona Ctrl + N)
Escribe el nombre del archivo (ejemplo: Program.cs)
Presiona Enter


**Editar y guardar código**:

Escribe o pega tu código en el editor
Observa el punto blanco en la pestaña del archivo (indica cambios sin guardar)
Guarda el archivo con Ctrl + S o File > Save
El punto blanco desaparece cuando el archivo está guardado



**Navegación por la interfaz**:

**Barra lateral izquierda**: Explorador de archivos, búsqueda, control de versiones, extensiones
**Área del editor**: Zona principal para editar código (soporta múltiples pestañas)
**Paleta de comandos**: Presiona Ctrl + Shift + P para acceder a todos los comandos disponibles
**Terminal integrada**: Presiona Ctrl + ñ para abrir/cerrar la terminal

---

# Personalización del Entorno

Vamos a personalizar VS Code para mejorar tu experiencia de desarrollo.

## Cambiar el tema de color

**Estado inicial (tema predeterminado)**:



**Pasos para cambiar el tema**:

Presiona Ctrl + K, Ctrl + T o ve a File > Preferences > Theme > Color Theme
Aparecerá una lista de temas disponibles
Usa las flechas del teclado para previsualizar cada tema en tiempo real
Selecciona "One Dark Pro" o "Material Theme" (recomendados)
Presiona Enter para aplicar el tema

(/screenshots/temas_Completos.png)

**Resultado final**:



## Configurar fuente con ligaduras (Fira Code)

**Antes de aplicar Fira Code**:



**Pasos de instalación**:

Descarga Fira Code desde https://github.com/tonsky/FiraCode
Instala la fuente en tu sistema (doble clic en el archivo .ttf > Instalar)
En VS Code, abre la configuración: Ctrl + , o File > Preferences > Settings
Busca "font family"
Añade 'Fira Code' al inicio de la lista de fuentes
Busca "font ligatures" y marca la casilla para activarlas



**Resultado final (con ligaduras)**:

Las ligaduras convierten secuencias como =>, !=, >= en símbolos más legibles.

(/screenshots/Firacode.png)

## Cambiar iconos de archivos

**Antes (iconos predeterminados)**:



**Pasos**:

Presiona Ctrl + Shift + P
Escribe "file icon theme" y selecciona "Preferences: File Icon Theme"
Elige "Material Icon Theme" o "Seti"
Los iconos se actualizan inmediatamente



**Resultado final**:



## Configuraciones adicionales del editor

Abre la configuración con Ctrl + , y aplica estos ajustes:

**Format On Save**: Busca "format on save" y marca la casilla (el código se formatea automáticamente al guardar)
**Word Wrap**: Busca "word wrap" y selecciona "on" (las líneas largas se ajustan sin scroll horizontal)
**Auto Save**: Busca "auto save" y selecciona "afterDelay" (guarda automáticamente después de 1 segundo)

Mostrar imagen

**Atajos de teclado útiles**:

Ctrl + /: Comentar/descomentar líneas
Ctrl + Shift + P: Abrir paleta de comandos
Ctrl + ñ: Abrir/cerrar terminal integrada
Alt + ↑/↓: Mover líneas hacia arriba/abajo
Ctrl + D: Seleccionar siguiente coincidencia
F12: Ir a definición

---

# SDK .NET

## Proceso de instalación:

Dirígete a https://dotnet.microsoft.com/download
(/screenshots/dotnet1.png)

Descarga el SDK de .NET (versión más reciente recomendada)

(/screenshots/dotnet2.png)

Ejecuta el instalador y sigue el asistente de instalación

(/screenshots/dotnet3.png)
## Verificación:

Abre la terminal (PowerShell o CMD) y ejecuta:

```bash
dotnet --version
```

Deberías ver la versión del SDK instalado (ejemplo: 8.0.100)

(/screenshots/dotnet4.png)

---

# Configuración para C#

## Extensiones esenciales:

Abre el panel de extensiones con Ctrl + Shift + X
Busca "C# Dev Kit" en el Marketplace
Haz clic en "Install" en la extensión oficial de Microsoft


Esta extensión instala automáticamente:

**C#**: Soporte base del lenguaje (IntelliSense, sintaxis)
**C# Dev Kit**: Gestión de proyectos, debugging y navegación de código

(screenshots/dotnet5.png)
**Verificación de extensiones instaladas**:

Confirma que ambas extensiones están activas en el panel de extensiones (aparecerán con un checkmark verde).

---

# Flujo de Trabajo con C#

## Creación de un proyecto desde VS Code

**Usando la interfaz de C# Dev Kit**:

Presiona Ctrl + Shift + P para abrir la paleta de comandos
Escribe ".NET: New Project" y selecciona la opción
Elige "Console App" de la lista de plantillas
Introduce el nombre del proyecto (ejemplo: MiPrimerProyecto)
Selecciona la carpeta donde guardar el proyecto
El proyecto se crea automáticamente con la estructura básica



**Estructura del proyecto creado**:

```
MiPrimerProyecto/
├── Program.cs          # Archivo principal con el código
├── MiPrimerProyecto.csproj  # Archivo de configuración del proyecto
└── obj/                # Archivos temporales de compilación
```

## Código de ejemplo mejorado

Reemplaza el contenido de Program.cs con este código:

```csharp
namespace MiPrimerProyecto
{
    class Program
    {
        static void Main(string[] args)
        {
            // Verificar si se pasaron argumentos
            if (args.Length == 0)
            {
                Console.WriteLine("No se proporcionaron nombres.");
                Console.WriteLine("Uso: dotnet run <nombre1> <nombre2>");
                return;
            }

            // Mostrar mensaje para cada argumento
            foreach (string nombre in args)
            {
                string mensaje = MostrarMensaje(nombre);
                Console.WriteLine(mensaje);
            }

            // Esperar entrada del usuario antes de cerrar
            Console.WriteLine("\nPresiona cualquier tecla para salir...");
            Console.ReadKey();
        }

        static string MostrarMensaje(string nombre)
        {
            return $"¡Hola {nombre}! Bienvenido al sistema.";
        }
    }
}
```

Mostrar imagen

## Compilación y ejecución desde el IDE

❌ **NO USES** comandos de terminal (dotnet build, dotnet run)  
✅ **Ejecuta desde el IDE** con estos métodos:

### Método 1: Botón Run (Recomendado)

Observa la parte superior derecha del editor
Haz clic en el botón ▶️ Run (triángulo verde)
El programa se compila y ejecuta automáticamente
La salida aparece en el panel DEBUG CONSOLE

Mostrar imagen

### Método 2: Atajo de teclado

Presiona Ctrl + F5 (ejecutar sin depuración)
O presiona F5 (ejecutar con depuración)
La aplicación se ejecuta y muestra la salida

**Salida del programa**:

Mostrar imagen

```
¡Hola Izan! Bienvenido al sistema.
¡Hola Gonzalo! Bienvenido al sistema.

Presiona cualquier tecla para salir...
```

Mostrar imagen

## Debugging (Depuración)

**Configurar puntos de interrupción (breakpoints)**:

Haz clic en el margen izquierdo del editor (junto al número de línea)
Aparecerá un punto rojo que indica el breakpoint
El programa se detendrá en esa línea durante la ejecución

Mostrar imagen

**Ejecutar con depuración**:

Presiona F5 o haz clic en Run > Start Debugging
El programa se detiene en el primer breakpoint
Usa los controles de depuración:

- F10: Paso a paso (siguiente línea)
- F11: Entrar en función
- Shift + F11: Salir de función
- F5: Continuar ejecución

Mostrar imagen

**Inspeccionar variables**:

El panel VARIABLES muestra todas las variables visibles
Pasa el cursor sobre una variable en el código para ver su valor
Usa el panel WATCH para observar expresiones específicas

Mostrar imagen

**Panel Call Stack**:

Muestra la pila de llamadas de funciones
Útil para rastrear cómo llegaste al punto actual de ejecución

---

# Visual Studio - IDE Alternativo

## Instalación

**Proceso de instalación**:

Dirígete a https://visualstudio.microsoft.com/es/
Descarga Visual Studio Community (versión gratuita) o Professional (con licencia)

Mostrar imagen

Ejecuta el instalador descargado
Espera a que se cargue el Visual Studio Installer

**Componentes necesarios**:

En la ventana del instalador, selecciona la carga de trabajo:

✅ **Desarrollo de escritorio de .NET**

Incluye: C#, Windows Forms, WPF, SDK de .NET y compiladores

Mostrar imagen

Haz clic en "Instalar" y espera a que finalice (puede tardar varios minutos)

**Verificación**:

Abre Visual Studio desde el menú Inicio
En la pantalla de bienvenida, haz clic en "Crear un proyecto nuevo"
Busca y selecciona "Aplicación de consola" (.NET)
Si puedes crear el proyecto, la instalación fue exitosa

Mostrar imagen

---

# Desarrollo con C#

## Creación de proyecto

**Pasos para crear un nuevo proyecto**:

Abre Visual Studio
En la pantalla de inicio, haz clic en "Crear un proyecto nuevo"
En el cuadro de búsqueda, escribe "consola"
Selecciona "Aplicación de consola" con C# (.NET)
Haz clic en "Siguiente"

Mostrar imagen

**Configurar el proyecto**:

**Nombre del proyecto**: MiProyectoVisualStudio
**Ubicación**: Elige la carpeta donde guardarlo
**Nombre de la solución**: (se autocompletará)

Haz clic en "Crear"

Mostrar imagen

Visual Studio crea automáticamente el proyecto con un archivo Program.cs básico.

## Código de ejemplo en Visual Studio

Reemplaza el contenido de Program.cs con este código:

```csharp
namespace MiProyectoVisualStudio
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("=== Sistema de Bienvenida ===\n");

            // Solicitar nombres al usuario
            Console.Write("Introduce el primer nombre: ");
            string nombre1 = Console.ReadLine() ?? "Usuario1";

            Console.Write("Introduce el segundo nombre: ");
            string nombre2 = Console.ReadLine() ?? "Usuario2";

            // Mostrar mensajes de bienvenida
            Console.WriteLine();
            MostrarBienvenida(nombre1);
            MostrarBienvenida(nombre2);

            // Mostrar estadísticas
            Console.WriteLine($"\nTotal de usuarios registrados: 2");
            
            Console.WriteLine("\nPresiona cualquier tecla para salir...");
            Console.ReadKey();
        }

        static void MostrarBienvenida(string nombre)
        {
            string mensaje = $"¡Hola {nombre}! Bienvenido al sistema.";
            Console.WriteLine(mensaje);
            Console.WriteLine($"Tu nombre tiene {nombre.Length} caracteres.");
        }
    }
}
```

Mostrar imagen

## Compilación y ejecución desde el IDE

❌ **NO uses** Ctrl + Shift + B solo para compilar  
✅ **Ejecuta directamente desde el IDE**:

### Método 1: Botón de Inicio (Recomendado)

Localiza el botón verde con el triángulo ▶️ en la barra superior
Al lado verá el nombre del proyecto
Haz clic en el botón para ejecutar

Mostrar imagen

### Método 2: Atajos de teclado

Presiona F5 - Ejecutar con depuración
Presiona Ctrl + F5 - Ejecutar sin depuración (recomendado para ver la salida completa)

### Método 3: Menú

Ve a Depurar > Iniciar sin depurar (Ctrl + F5)

**Salida del programa**:

Al ejecutar con Ctrl + F5, se abre una ventana de consola:

Mostrar imagen

```
=== Sistema de Bienvenida ===

Introduce el primer nombre: Izan
Introduce el segundo nombre: Gonzalo

¡Hola Izan! Bienvenido al sistema.
Tu nombre tiene 4 caracteres.
¡Hola Gonzalo! Bienvenido al sistema.
Tu nombre tiene 5 caracteres.

Total de usuarios registrados: 2

Presiona cualquier tecla para salir...
```

Mostrar imagen

## Debugging en Visual Studio

**Configurar breakpoints**:

Haz clic en el margen gris izquierdo (junto a los números de línea)
Aparece un punto rojo sólido
Para quitar el breakpoint, vuelve a hacer clic en el punto rojo

Mostrar imagen

**Iniciar depuración**:

Presiona F5 o haz clic en el botón ▶️ verde
El programa se ejecuta y se detiene en el primer breakpoint
La línea actual se resalta en amarillo

Mostrar imagen

**Controles de depuración**:

F10 - Paso a paso por procedimientos (ejecuta la línea actual)
F11 - Paso a paso por instrucciones (entra en funciones)
Shift + F11 - Paso a paso para salir (sale de la función actual)
F5 - Continuar (ejecuta hasta el siguiente breakpoint)
Shift + F5 - Detener depuración

Mostrar imagen

**Inspeccionar variables**:

**Ventana Automático**: Muestra variables de la línea actual y anteriores
**Ventana Variables locales**: Muestra todas las variables del ámbito actual
**Ventana Inspección**: Añade expresiones personalizadas para observar

Para abrir estas ventanas: Depurar > Ventanas > [nombre de la ventana]

Mostrar imagen

**Uso de la ventana Inmediato**:

Durante la depuración, ve a Depurar > Ventanas > Inmediato
Puedes ejecutar código y evaluar expresiones en tiempo real
Ejemplo: escribe nombre1.ToUpper() y presiona Enter

Mostrar imagen

---

# Configuración de Lenguaje Adicional

**Lenguaje seleccionado**: Python

**Justificación**: Python es un lenguaje versátil, fácil de aprender e ideal para desarrollo rápido, scripting, análisis de datos y prototipado. Su sintaxis clara lo hace perfecto como segundo lenguaje de referencia.

## Instalación del Entorno Python

**Descarga e instalación**:

Visita la página oficial https://www.python.org/downloads/
Haz clic en "Download Python 3.x.x" (última versión estable)

Mostrar imagen

Ejecuta el instalador descargado
**IMPORTANTE**: Marca la casilla "Add Python to PATH"
Haz clic en "Install Now"

Mostrar imagen

**Verificación**:

Abre la terminal (PowerShell o CMD) y ejecuta:

```bash
python --version
```

O en algunos sistemas:

```bash
python3 --version
```

Deberías ver la versión instalada (ejemplo: Python 3.12.0)

Mostrar imagen

---

## Configuración en VS Code para Python

**Instalar la extensión de Python**:

Abre VS Code
Presiona Ctrl + Shift + X para abrir el panel de extensiones
Busca "Python" en el Marketplace
Haz clic en "Install" en la extensión oficial de Microsoft

Mostrar imagen

La extensión incluye:

- IntelliSense y autocompletado
- Linting (análisis de código)
- Debugging integrado
- Soporte para Jupyter Notebooks
- Gestión de entornos virtuales

**Configurar el intérprete**:

Abre un archivo .py o presiona Ctrl + Shift + P
Escribe "Python: Select Interpreter"
Selecciona la versión de Python instalada en tu sistema

Mostrar imagen

**Configuraciones recomendadas para Python**:

Abre la configuración (Ctrl + ,) y busca estas opciones:

**Python > Linting: Enabled** - Activar análisis de código
**Python > Linting: Pylint Enabled** - Activar Pylint para detección de errores
**Python > Formatting: Provider** - Seleccionar "black" o "autopep8"
**Editor: Format On Save** - Formatear automáticamente al guardar

Mostrar imagen

---

## Proyecto de Ejemplo en Python

**Crear un proyecto Python**:

Crea una nueva carpeta para tu proyecto (ejemplo: ProyectoPython)
Abre la carpeta en VS Code: File > Open Folder
Crea un nuevo archivo: haz clic derecho en el explorador > New File
Nómbralo calculadora.py

**Código de ejemplo**:

```python
# calculadora.py
"""
Sistema de calculadora básica con menú interactivo
Autor: Tu Nombre
Fecha: 2024
"""

def suma(a, b):
    """Suma dos números"""
    return a + b

def resta(a, b):
    """Resta dos números"""
    return a - b

def multiplicacion(a, b):
    """Multiplica dos números"""
    return a * b

def division(a, b):
    """Divide dos números"""
    if b == 0:
        return "Error: División por cero"
    return a / b

def mostrar_menu():
    """Muestra el menú de opciones"""
    print("\n=== CALCULADORA ===")
    print("1. Suma")
    print("2. Resta")
    print("3. Multiplicación")
    print("4. División")
    print("5. Salir")
    print("==================")

def main():
    """Función principal"""
    while True:
        mostrar_menu()
        
        try:
            opcion = int(input("\nElige una opción (1-5): "))
            
            if opcion == 5:
                print("¡Hasta luego!")
                break
            
            if opcion < 1 or opcion > 5:
                print("Opción no válida. Intenta de nuevo.")
                continue
            
            # Solicitar números
            num1 = float(input("Introduce el primer número: "))
            num2 = float(input("Introduce el segundo número: "))
            
            # Realizar operación
            if opcion == 1:
                resultado = suma(num1, num2)
                print(f"\n{num1} + {num2} = {resultado}")
            elif opcion == 2:
                resultado = resta(num1, num2)
                print(f"\n{num1} - {num2} = {resultado}")
            elif opcion == 3:
                resultado = multiplicacion(num1, num2)
                print(f"\n{num1} × {num2} = {resultado}")
            elif opcion == 4:
                resultado = division(num1, num2)
                print(f"\n{num1} ÷ {num2} = {resultado}")
                
        except ValueError:
            print("\nError: Debes introducir un número válido")
        except Exception as e:
            print(f"\nError inesperado: {e}")

if __name__ == "__main__":
    main()
```

Mostrar imagen

## Ejecutar el programa desde VS Code

### Método 1: Botón Run (Recomendado)

Observa la esquina superior derecha del editor
Haz clic en el botón ▶️ (triángulo verde)
El programa se ejecuta en la terminal integrada

Mostrar imagen

### Método 2: Clic derecho

Haz clic derecho en cualquier parte del código
Selecciona "Run Python File in Terminal"

### Método 3: Atajo de teclado

Presiona Ctrl + F5 para ejecutar sin depuración

**Salida del programa**:

La terminal integrada muestra el programa en ejecución:

Mostrar imagen

```
=== CALCULADORA ===
1. Suma
2. Resta
3. Multiplicación
4. División
5. Salir
==================

Elige una opción (1-5): 1
Introduce el primer número: 15
Introduce el segundo número: 7

15.0 + 7.0 = 22.0

=== CALCULADORA ===
...
```

Mostrar imagen

## Debugging en Python

**Configurar breakpoints**:

Haz clic en el margen izquierdo junto a la línea donde quieres pausar
Aparece un punto rojo

Mostrar imagen

**Iniciar depuración**:

Presiona F5
Selecciona "Python File" si es la primera vez
El programa se detiene en el breakpoint

Mostrar imagen

**Inspeccionar variables**:

El panel VARIABLES muestra el valor de todas las variables
Puedes expandir listas, diccionarios y objetos
Usa WATCH para observar expresiones específicas

(/screenshots/vscode_python_variables.png)