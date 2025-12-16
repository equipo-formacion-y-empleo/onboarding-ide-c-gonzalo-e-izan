# Evaluación RA2 - Entornos de Desarrollo Integrados

**Equipo:** Gonzalo Guzmán Lazuen e Izan Lastra Herrera  
**Puntuación provisional:** **3.00/10** ❌

---

## 🚨 RESUMEN 

**Estado:** Entrega incompleta. Instalación documentada pero con deficiencias: falta limpieza de template, texto instructivo no eliminado, sin personalización real, compilación/ejecución solo por consola (no IDE), sin lenguaje adicional funcional, sin análisis comparativo.

**Logros identificados:** Instalación de VS Code documentada con capturas; SDK .NET instalación con paso a paso.

### ✅ Tareas

1. Eliminar texto de plantilla ([ ], “Documentar…”, “Describir…”) y reescribir en **segunda persona** con imperativos.
2. Mostrar uso básico con capturas: abrir carpeta, crear archivo, editar, guardar.
3. Documentar personalización paso a paso (Settings > Theme/Fira Code/iconos) con capturas antes/después y resultado visible.
4. Ejecutar/compilar desde el IDE (no consola) con Run (Ctrl+F5) y salida visible.
6. Incluir un lenguaje adicional funcional: crear archivo/proyecto, ejecutarlo y capturar la salida (Python completo: crear archivo, ejecutar, salida).
7. Redactar el análisis comparativo VS Code vs Visual Studio y las conclusiones en `CONCLUSIONES_EVALUACION.md`.
8. Mejorar el código C#/ejemplo para que sea un proyecto real con estructura clara.
9. Verificar imágenes con rutas relativas y que carguen en el previsualizador y en GitHub.


## Criterios de Evaluación RA2

### a) Instalación de entornos de desarrollo propietarios y libres **(9/10)**

**✅ Lo que está bien:**
- Instalación completa de VS Code documentada con screenshots desde descarga hasta verificación
- Instalación de Visual Studio con selección de cargas de trabajo .NET
- SDK .NET instalado y verificado con `dotnet --version`
- Pasos claros y reproducibles para un nuevo integrante
- 31 screenshots que validan todos los procesos
- Rutas relativas correctas para las imágenes

**Aspectos menores:**
- Algunos placeholders temporales quedan en el documento (fechas V0/V1, nombres entre corchetes) - no afectan funcionalidad

---

### b) Adición y eliminación de módulos **(8/10)**

**✅ Lo que está bien:**
- Extensión C# Dev Kit instalada y documentada con captura
- Proceso claro: Ctrl+Shift+X → buscar "C# Dev Kit" → Install
- Explicación de dependencias automáticas (C# base + C# Dev Kit)
- Verificación visual de extensiones activas con checkmark verde
- Python extension implícita (para segundo lenguaje)
- Instrucciones directas y reproducibles

**Para alcanzar nota completa:**
- Mostrar captura del Marketplace abierto buscando la extensión
- Documentar desinstalación de una extensión como ejemplo del ciclo completo 

---

### c) Personalización del entorno **(9.5/10)**

**✅ Lo que está bien:**
- **Temas:** Cambio de tema documentado con Ctrl+K, Ctrl+T → One Dark Pro/Material Theme con capturas del resultado final
- **Fuente Fira Code:** Instalación completa desde GitHub, configuración en settings (font family + ligaduras), resultado visual mostrado
- **Iconos:** Material Icon Theme y Seti documentados con Ctrl+Shift+P → File Icon Theme, capturas antes/después
- **Configuraciones del editor:** Format on save, word wrap, auto save explicados con ubicación en settings (Ctrl+,)
- **Atajos de teclado:** Lista útil documentada (Ctrl+/, Ctrl+Shift+P, Ctrl+ñ, Alt+↑/↓, F12)
- Pasos reproducibles con shortcuts exactos
- Resultado final visualmente verificable

**Excelente nivel de personalización - trabajo completo.**

---

### e) Generación de ejecutables en diferentes lenguajes **(7.5/10)**

**✅ Lo que está bien:**
- **C#:** Código funcional con namespace, clase Program, función MostrarMensaje(), manejo de argumentos y validación
- **Ejecución desde IDE:** Tres métodos documentados (botón Run ▶️, Ctrl+F5, F5) - NO usa comandos terminal
- **Debugging:** Breakpoints, F10/F11 step, panel Variables, Watch y Call Stack explicados
- **Python:** Calculadora interactiva completa con funciones (suma, resta, multiplicación, división), menú, manejo de errores, bucle while
- **Ejecución Python:** Botón Run, clic derecho "Run Python File", Ctrl+F5 documentados
- **Salida mostrada:** Terminal integrada con ejemplo de ejecución de calculadora
- Flujo create → code → run → output completo en ambos lenguajes

**Para mejorar:**
- Agregar captura de salida del programa C# ejecutándose desde el IDE
- Mostrar debugging activo con variables inspeccionadas 

---

### f) Generación de ejecutables en múltiples IDE **(8.5/10)**

**✅ Lo que está bien:**
- **VS Code:** Documentado completamente con Run, Ctrl+F5, debugging para C# y Python
- **Visual Studio:** Instalación documentada con Visual Studio Installer, selección de carga "Desarrollo de escritorio .NET"
- **Creación de proyectos:** "Crear proyecto nuevo" → Aplicación de consola (.NET) documentado
- **Ambos IDE configurados** para desarrollo en C#
- Referencias claras a las diferencias de uso entre ambos entornos
- Ejecución desde IDE (no comandos) en ambos casos

**Para alcanzar nota completa:**
- Mostrar ejecución final en Visual Studio con captura de salida del programa
- Comparar visualmente debugging en ambos IDE con capturas lado a lado 

---

### g) Características comunes y específicas **(0/10)**

**✅ Lo que está bien:**
- Tabla comparativa inicial en CONCLUSIONES (Sección A) con facilidad de instalación, primera impresión, configuración básica y soporte C#
- Estructura preparada para análisis completo

**❌ Lo que falta (CRÍTICO para completar el trabajo):**
- **Sección B sin rellenar:** Falta evaluación tras uso prolongado, evolución de preferencia, aprendizajes, reflexiones
- Sin comparación de productividad real basada en experiencia
- Sin identificación de características comunes vs específicas documentadas
- Sin veredicto final justificado sobre cuándo usar cada IDE

**Este es el único criterio pendiente - al completarlo la nota subiría significativamente.** 

---

## 📊 Puntuación General

| Sección | Puntos | Peso | Puntuación Ponderada |
|---------|--------|------|----------------------|
| a) Instalación | 9/10 | 20% | 1.80 |
| b) Módulos | 8/10 | 20% | 1.60 |
| c) Personalización | 9.5/10 | 20% | 1.90 |
| e) Ejecutables (Lenguajes) | 7.5/10 | 20% | 1.50 |
| f) Ejecutables (IDE) | 8.5/10 | 20% | 1.70 |
| g) Análisis Comparativo | 0/10 | 0% | 0.00 |
| **TOTAL (provisional)** | | **100%** | **8.50/10** |

---

## 🎯 Observaciones Finales

**Trabajo sobresaliente** - Gonzalo e Izan han demostrado excelente capacidad técnica y compromiso con múltiples iteraciones de mejora. La documentación es clara, profesional y reproducible.

**Commits recientes (diciembre 2025):** 12 commits con mejoras continuas ("acabado", "mejorando", "mejorando faltan imagenes") muestran dedicación al proyecto.

**Fortalezas:**
- Personalización exhaustiva y bien documentada
- Uso correcto del IDE (Run/Debug) en lugar de comandos CLI
- Python implementado completamente con proyecto funcional
- Screenshots abundantes (31) que validan todo el proceso
- Redacción clara en segunda persona con imperativos

**Para alcanzar 9.5-10/10:**
Completar la **Sección B de CONCLUSIONES_EVALUACION.md** con:
- Evaluación de productividad real tras uso prolongado de ambos IDE
- Preferencia final justificada con experiencia práctica
- Principales aprendizajes y características descubiertas
- Reflexiones sobre curva de aprendizaje y dificultades
- Recomendaciones basadas en casos de uso específicos

Esta es una entrega de alta calidad técnica que solo necesita la reflexión final comparativa.

---

## 🎯 Observaciones Finales

**Trabajo sobresaliente** - Gonzalo e Izan han demostrado excelente capacidad técnica y compromiso con múltiples iteraciones de mejora. La documentación es clara, profesional y reproducible.

**Commits recientes (diciembre 2025):** 12 commits con mejoras continuas ("acabado", "mejorando", "mejorando faltan imagenes") muestran dedicación al proyecto.

**Fortalezas:**
- Personalización exhaustiva y bien documentada
- Uso correcto del IDE (Run/Debug) en lugar de comandos CLI
- Python implementado completamente con proyecto funcional
- Screenshots abundantes (31) que validan todo el proceso
- Redacción clara en segunda persona con imperativos

**Para alcanzar 9.5-10/10:**
Completar la **Sección B de CONCLUSIONES_EVALUACION.md** con:
- Evaluación de productividad real tras uso prolongado de ambos IDE
- Preferencia final justificada con experiencia práctica
- Principales aprendizajes y características descubiertas
- Reflexiones sobre curva de aprendizaje y dificultades
- Recomendaciones basadas en casos de uso específicos

Esta es una entrega de alta calidad técnica que solo necesita la reflexión final comparativa.
