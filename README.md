# Sistema de Captura de Voz Direccional con Filtrado de Ruido

## Descripción
Este proyecto desarrolla un sistema de captura de voz direccional con filtrado de ruido, optimizando la calidad de la señal de voz en entornos ruidosos. Se modela el comportamiento del sonido en los micrófonos y se aplican técnicas de control y filtrado para mejorar la señal procesada.

## Autor
**Renzo Tassara**  
_Email:_ renzotassara98@gmail.com  
_Universidad Nacional de Cuyo - Facultad de Ingeniería_  

## Contenido del Repositorio
- **Informe:** Documento PDF detallando el desarrollo del proyecto.
- **Presentación:** Diapositivas utilizadas para exponer el proyecto.
- **Códigos:** Archivos en Matlab/Simulink utilizados para la simulación y procesamiento de señales.

## Funcionamiento
### 1. Generación de sonido
Se simula la generación de sonido con archivos de audio en formato `.mp3`.

### 2. Modelado del sistema
Se modela la interacción del sonido con los micrófonos mediante tres subsistemas:
- **Subsistema mecánico sonoro:** Conversión de sonido en fuerza sobre la membrana del micrófono.
- **Subsistema mecánico de la membrana:** Modelado como un sistema masa-resorte.
- **Subsistema eléctrico:** Conversión del movimiento de la membrana en señal eléctrica.

### 3. Control y filtrado
- Se implementa un sistema de control que ajusta las ganancias de los micrófonos para mejorar la captación de la señal de interés.
- Se restan las señales de ambos micrófonos y se aplica un filtro FIR para reducir el ruido de alta frecuencia.
- Se comparan los resultados obtenidos con y sin filtrado.

## Requisitos
- Matlab con Simulink.
- Archivos de audio `.mp3` de voz y ruido ambiente.

## Instrucciones de Uso
1. Abrir Matlab y cargar los archivos `.slx` en Simulink.
2. Cambiar las ubicaciones de los archivos `.mp3` en los bloques de sonido correspondientes en Simulink
3. Ejecutar la simulación para visualizar el procesamiento de la señal.
4. Analizar los resultados obtenidos en las gráficas generadas.

## Resultados y Conclusiones
- Se logró una atenuación efectiva del ruido ambiental mediante el ajuste de ganancias y filtrado de señal.
- Se verificó que el filtro FIR mejora la calidad de la señal eliminando frecuencias no deseadas.
- Se sugiere como mejora futura la incorporación de más micrófonos para obtener mayor precisión en la direccionalidad.
