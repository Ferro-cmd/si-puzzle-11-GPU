# Teoría · Pieza 11: Unidad de Procesamiento Gráfico(GPU)

**Grupo:** Pablo Quiros Dominguez · Esteban Amador Fernández

## Conceptos clave

- **GPU:** Unidad de Procesamiento Gráfico, en español, es un circuito electrónico que sirve para acelerar el procesamiento informático de gráficos e imágenes. 
- **Controlador  de la GPU:** Gestiona el flujo de datos y las instrucciones.  
- **Núcleos de procesamiento:** Realizan los cálculos en paralelo, píxeles, efectos, ia...
- **Shaders:** Son programas que corren e los núcleos de sombreado de la GPU.
- **VRAM:** Capacidad de almacenamiento de datos gráficos.
- **Rendimiento de cálculo:** Cantidad de operaciones de coma flotante(calculos matematicos con numeros reales que contienen partes fraccionarias). 
- **Ancho de banda:** cantidad de datos que se pueden transferir por segundo.
- **Consumo eléctrico:** Potencia electrica que consume la GPU.
- **Unidades especializadas:** hardware diseñado especificamente para acelerar tareas matemáticas y de procesamiento masivo. Ej: IA, Ray Tracing.
- **Interfaz de memoria:** Gestiona el acceso a la memoria y el ancho de banda.
## Tabla resumen

| Tipo | Dato clave | Cuándo se usa |
|---|---|---|
|Grafica Integrada (iGPU)|Forma parte de la CPU o del chip principal y usa la RAM del sistema; consume y cuesta poco pero su potencia es limitada|Se usa en portatiles, en ordenadores de ofimatica y equipos compactos|
|Dedicada GPU|Tarjeta independiente en ranura PCIe, con su propio chip, VRAM, refrigeración y alimentación. Es mucho más potente pero más cara y requiere más energía|Se usa videojuegos, edición de video, renderizado 3D e IA|
|Virtual vGPU|No es un chip, es una forma de repartir una GPU física en varias GPU virtuales para distintas máquinas virtuales|Se usa en servidores y centros de datos|
|Gráfica Externa|Son tarjets dedicadas instaladas en una carcasa externa que se conecta al ordenador mediante una interfaz de alta velocidad|Se usa para aumetnar la potencia de una misma GPU física entre varios usuarios.|Se utiliza para videojuegos y trabajos gráficos exigentes|
|Gráficas profesionales|Estan diseñadas para apicaciones profesionales y estaciones de trabajo|Se usa para arquitectura, ingenieria, simulaciones,y renderizado |

## Datos que hay que saberse
La GPU ejecuta la misma operación sobre muchisimos datos a la vez,(cálculo en paralelo).
Recibe las instrucciones de la CPU por bus PCIe y envia la imagen final al monitor por HDMI o DisplayPort.
Además de gráficos, sirve para entrenar modelos IA, codificar y decodificar vídeo y hacer simulaciones cientficas.
Unidades de medida:
   - a) Frecuencia Mhz o Ghz.
   - b) VRAM en GB.
   - c) Rendimiento de cálculo en GFLOPS o TFLOPS.
   - d) Ancho de banda, en GB/s, 
   - e) Consumo en W.
   - f) Temperatura en ºC
   - g) Rendimiento en videojuegos FPS.

La evolución de las GPU se debe a diversos factores relacionados entre ellos, el aumento de potencia, el aumento de la capacidad de memoria y su velocidad y a la incorporación de nuevas tecnologías.


Averías típicas:
a) Artefactos visuales: Puede deberse al sobrecalentamiento, drivers mal actualizados,problemas en la fuente de alimentación o al realizar overclock(forzar).

b) Pantalla negra: Puede deberse a un fallo real en la tarjeta física o una mala conexión al monitor. También puede ser por drivers corruptos o desactualizados.

c) Sobrecalentamiento: La GPU debido al calentamiento excesivo, reduce su rendimiento, llegando a provocar "tirones". Si la temperatura sigue subiendo, la GPU se apaga sola como mecanismo de defensa. Se puede observar la temperatura usando los programas MSI Afterburner o HWMonitor.

d) Salidas de vídeo: Puede deberse a distintos factores, Pueden aparecer pantalla negra, parpadeos , en la imagen , artefacto visuales o distorsión de color o reconocimiento parcial, que consiste en que detecta un monitor pero no muestra imagen o limita la resolución. Este tipo de errores puede deberse a que el HDMI o DisplayPort este en mal estado, que estos puertos esten dañados, sucios o desoldados por el peso de cables sobre la placa base, por último este tipo de errores puede deberse simplemente a que no esté bien encajada la GPU.
## Preguntas tipo test (8)

1. ¿Qué permite una GPU virtual(vGPU)?
   - a) Aumentar la frecuencia de reloj de la GPU.
   - b) Sustituir la CPU por la GPU.
   - c) Compartir los recursos de una GPU física entre varias maquinas virtuales o usuarios. <---correcta
   - d) Conectar varios monitores sin cables.
   - Explicación: La vGPU reparte una GPU física en varias virtuales y se usa sobretodos en centros de datos.

2. ¿Qué característica defina a una GPU integrada?
   - a) Tiene su propia VRAM y refrigeración.
   - b) Forma parte de la CPU o del chip principal y usa la ram del sistema. <--- correcta.
   - c) Se conecta por PCIe.
   - d) Solo funciona en servidores.
   - Explicación: las integradas no tienen memoria propia.

3. ¿En que unidad se mide el ancho de banda de memoria de una GPU?
   - a) Mhz.
   - b) TFLOPS.
   - c) Gb/s
   - d) GB/s <--- correcta
   - Explicación: el ancho de banda indica cuantos datos puede transferir por segundo.

4. ¿Para que sirve la VRAM?
   - a) Para almacenar texturas, modelos y datos gráficos. <--- correcta
   - b) Para almacenar el sistema operativo.
   - c) Para almacenar los drivers de la tarjeta,
   - d) Para enviar instrucciones a los núcleos de procesamiento.
   - Explicación: es la memoria gráfica de la GPU y se mide en GB, se usa para guardar texturas modelos y datos gráficos.

5. ¿A qué se debe la evolución de las GPUs?
   - a) Aumento del rendimiento
   - b) Capacidad de la memoria
   - c) Incorporación de nuevas tecnologías
   - d) Todas son correctas <--- Correcta
   - Explicación: No se debe a un único factor su evolución, sino que es un conjunto de ellas, gracias a mejorar las capacidades que tiene y al desarrollo de nuevas tecnologías permiten que su evolución no se quede "estancada".

6. ¿Qué son los shaders?
   - a) Un modelo de sistema de refrigeración.
   - b) Puerto por donde conecta la GPU con el monitor.
   - c) Programas que se ejecutan en los núcleos de sombreado.<--- correcto
   - d) Un tipo de memoria de la GPU.
   - Explicación: Son programas que corren en los núcleos de sombreado de la GPU.

7. Si aparecen artefactos visuales en varias aplicaciones y siguen tras cambiar de drives,¿cuál es la causa mas probable?
   - a) Un fallo del hardware de la GPU. <--- correcta
   - b) Una fuente de alimentación sobredimensionada.
   - c) Un cable HDMI de mala calidad.
   - d) Un fallo del sistema operativo.
   - Explicación: Si descartamos el problema del software(drivers), y ocurre en varias aplicaciones, lo mas probable es que sea culpa del propio hardware.

8. ¿Sobre que temperatura es peligroso mantener una GPU?
   - a) Sobre los 70ºC
   - b) Sobre los 75ºC
   - c) Sobre los 80ºC
   - d) Sobre los 85ºC
   - Explicación: una alta temperatura constante es probable a fallos en la refrigeración de la GPU, ya sea por mala fijación del disipador o por pasta térmica reseca.
