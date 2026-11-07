# Teoría · Pieza 11: Unidad de Procesamiento Gráfico(GPU)

**Grupo:** Pablo Quiros Dominguez · Esteban Amador Fernández

> Máximo 1 folio por las dos caras. Es lo que estudiará toda la clase para el test: claro, exacto y sin relleno.

## Conceptos clave

- **GPU:** Unidad de Procesamiento Gráfico, en español, es un circuito electrónico que sirve para acelerar el procesamiento informático de gráficos e imágenes. 
- **Controlador  de la GPU:** Gestiona el flujo de datos y las instrucciones.  
- **Núcleos de procesamiento:** Realizan los cálculos en paralelo, píxeles, efectos, ia...
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
|Gráfica Externa|Son tarjets dedicadas instaladas en una carcasa externa que se conecta al ordenador mediante una interfaz de alta velocidad|Se usa para aumetnar la potencia de una misma GPU física entre varios usuarios.|Se utiliza para videojusegos y trabajos gráficos exigentes|
|Gráficas profesionales|Estan diseñadas para apicaciones profesionales y estaciones de trabajo|

## Datos que hay que saberse
- La GPU ejecuta la misma operación sobre muchisimos datos a la vez,(cálculo en paralelo).
- Recibe las instrucciones de la CPU por bus PCIe y envia la imagen final al monitor por HDMI o DisplayPort.
- Además de gráficos, sirve para entrenar modelos IA, codificar y decodificar vídeo y hacer simulaciones cientficas.
- Unidades de medida:
a) Frecuencia Mhz o Ghz.
b) VRAM en GB.
c) Rendimiento de cálculo en GFLOPS o TFLOPS.
d) Ancho de banda, en GB/s, 
e) Consumo en W.
f) Temperatura en ºC
g) Rendimiento en videojuegos FPS.

- Averías típicas:
a) Artefactos visuales: Puede deberse al sobrecalentamiento, drivers mal actualizados,problemas en la fuente de alimentación o al realizar overclock(forzar).

b) Pantalla negra: Puede deberse a un fallo real en la tarjeta física o una mala conexión al monitor. También puede ser por drivers corruptos o desactualizados.

c) Sobrecalentamiento: La GPU debido al calentamiento excesivo, reduce su rendimiento, llegando a provocar "tirones". Si la temperatura sigue subiendo, la GPU se apaga sola como mecanismo de defensa. Se puede observar la temperatura usando los programas MSI Afterburner o HWMonitor.

d) Salidas de vídeo: Puede deberse a distintos factores, Pueden aparecer pantalla negra, parpadeos , en la imagen , artefacto visuales o distorsión de color o reconocimiento parcial, que consiste en que detecta un monitor pero no muestra imagen o limita la resolución. Este tipo de errores puede deberse a que el HDMI o DisplayPort este en mal estado, que estos puertos esten dañados, sucios o desoldados por el peso de cables sobre la placa base, por último este tipo de errores puede deberse simplemente a que no esté bien encajada la GPU.
## Preguntas tipo test (8)

1. Pregunta
   - a) …
   - b) …  ← correcta
   - c) …
   - d) …
   - Explicación: …
