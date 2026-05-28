# Calibracion-monitor-de-signos
## Monitor de signos vitales Mindray uMEC 100
El uMEC 100 es un monitor multiparámetro utilizado para el seguimiento clínico de variables fisiológicas. De acuerdo con la hoja técnica de la serie uMEC 100/120/150, este equipo puede mostrar hasta 8 canales de forma de onda en el modelo uMEC 100 y permite el monitoreo de parámetros como ECG, frecuencia cardíaca, SpO₂, frecuencia de pulso, respiración, temperatura y presión arterial no invasiva, dependiendo de la configuración del equipo.

En esta práctica, el parámetro principal de trabajo es la pulsioximetría, ya que se utiliza el sensor de SpO₂ conectado al simulador OxSim OX-1.

## Simulador Pronk OxSim OX-1
El Pronk OxSim OX-1 es un simulador óptico de pulsioximetría diseñado para probar sistemas completos de SpO₂, incluyendo el monitor, el cable de extensión y el sensor. El fabricante indica que el equipo funciona con dos botones, utiliza una batería AA y detecta automáticamente el tipo de sensor, evitando seleccionar manualmente el fabricante del oxímetro bajo prueba.

El OxSim OX-1 permite simular diferentes combinaciones de SpO₂, frecuencia cardíaca o frecuencia de pulso y perfusión, lo que lo hace útil para evaluar si el monitor responde correctamente ante condiciones normales o alteradas.

### ¿Cómo colocar el uMEC 100 en modo “monitor”?
Para colocar el uMEC 100 en modo monitor se debe tener en cuenta que, en los monitores Mindray, el modo monitor está asociado a una configuración de visualización y filtrado adecuada para el monitoreo continuo del paciente. En el manual de operación de la serie uMEC se indica que, para modificar la configuración de ECG, se debe seleccionar la ventana del parámetro ECG o el área de la forma de onda para acceder al menú ECG Setup. Dentro de este menú, el filtro Monitor se recomienda para condiciones normales de medición.

Para la práctica de pulsioximetría, el procedimiento puede organizarse así:

## Procedimiento paso a paso
### Paso 1. Encender el monitor

Se conecta el monitor uMEC 100 a la alimentación eléctrica y se presiona el botón de encendido. Se espera hasta que el sistema cargue completamente y muestre la pantalla principal.

### Paso 2. Verificar que el equipo esté en pantalla de monitoreo

Una vez encendido, se verifica que el monitor esté en la pantalla principal de monitoreo, donde se visualizan los parámetros fisiológicos disponibles. En esta práctica deben observarse principalmente los espacios correspondientes a SpO₂, frecuencia de pulso o frecuencia cardíaca y la onda fotopletismográfica.

### Paso 3. Conectar el sensor de SpO₂

Se conecta el sensor de SpO₂ al puerto correspondiente del monitor uMEC 100. Luego, la pinza del sensor se coloca sobre el dedo artificial del simulador Pronk OxSim OX-1.

### Paso 4. Verificar la detección de señal

El monitor debe reconocer la señal proveniente del simulador y mostrar valores de saturación periférica de oxígeno, frecuencia de pulso y la onda fotopletismográfica.

### Paso 5. Seleccionar modo monitor en caso de usar ECG

Si también se utiliza ECG, se debe ingresar al área de ECG, abrir el menú ECG Setup, seleccionar la opción Filter y elegir Monitor. Esta configuración se utiliza para condiciones normales de medición y permite una señal adecuada para monitoreo continuo.

### Paso 6. Confirmar lectura estable

Antes de registrar los datos, se debe esperar a que los valores de SpO₂ y frecuencia de pulso se estabilicen. Esto evita tomar datos durante el periodo de transición inicial.
## Parámetros o variables fisiológicas que pueden simularse con el Pronk OxSim OX-1
El Pronk OxSim OX-1 permite simular principalmente variables asociadas a la pulsioximetría. De acuerdo con la información técnica del fabricante, el equipo posee modos de simulación con diferentes valores de saturación, frecuencia cardíaca y perfusión. Por ejemplo, puede simular 85 % de SpO₂ con 80 bpm, 95 % de SpO₂ con 40 bpm, 98 % de SpO₂ con 140 bpm y 99 % de SpO₂ con baja perfusión.

### Saturación periférica de oxígeno, SpO₂
La SpO₂ representa el porcentaje de hemoglobina oxigenada en sangre estimado mediante pulsioximetría. Clínicamente, es una variable fundamental para evaluar el estado de oxigenación del paciente.

En el OxSim OX-1 se pueden simular valores como:

| Modo | SpO₂ simulada | Interpretación |
|---|---:|---|
| Modo 1 | 85 % | Saturación baja o hipoxia simulada |
| Modo 2 | 95 % | Saturación normal |
| Modo 3 | 98 % | Saturación normal-alta |
| Modo 4 | 98 % | Saturación normal con frecuencia elevada |
| Modo 5 | 99 % | Saturación alta con baja perfusión |

### Frecuencia cardíaca o frecuencia de pulso
La frecuencia cardíaca o frecuencia de pulso corresponde al número de latidos o pulsaciones por minuto, expresado en bpm. En el contexto de esta práctica, el monitor recibe la señal desde el sensor de SpO₂, por lo que realmente se está evaluando la frecuencia de pulso derivada de la onda fotopletismográfica.

El OxSim OX-1 permite simular valores como:

| Valor simulado | Interpretación clínica            |
| -------------: | --------------------------------- |
|         40 bpm | Bradicardia                       |
|         80 bpm | Frecuencia dentro de rango normal |
|        140 bpm | Taquicardia                       |

Estos valores coinciden con los modos de simulación reportados para el OX-1: 40 bpm, 80 bpm y 140 bpm.
### Índice de perfusión o condición de baja perfusión
La perfusión hace referencia a la cantidad de flujo sanguíneo pulsátil que llega al sitio donde se ubica el sensor. En pulsioximetría, una perfusión baja puede generar una señal débil, con menor amplitud y mayor susceptibilidad al ruido.

El OxSim OX-1 permite simular un modo de baja perfusión con SpO₂ de 99 %, frecuencia de 80 bpm e índice de perfusión aproximado de 0.2, mientras que otros modos tienen un índice de perfusión aproximado de 2.0.

Esta prueba es importante porque permite observar si el monitor mantiene lecturas estables cuando la señal pulsátil es débil.

### Forma de onda fotopletismográfica
Aunque el OxSim no simula directamente una enfermedad como tal, genera una señal óptica pulsátil que el monitor interpreta como una onda fotopletismográfica. Esta onda representa los cambios de volumen sanguíneo arterial asociados a cada latido.

Cuando la frecuencia cardíaca aumenta, los picos de la onda aparecen más cercanos entre sí. Cuando la frecuencia disminuye, los picos se separan. En baja perfusión, la amplitud de la onda puede disminuir o verse menos estable.

## Tolerancias o errores máximos permitidos, EMP
Para definir los errores máximos permitidos se tomaron como referencia las especificaciones del monitor uMEC y las normas aplicables a equipos de pulsioximetría. La serie uMEC declara cumplimiento con la norma ISO 80601-2-61 para SpO₂. Esta norma aplica a la seguridad básica y desempeño esencial de equipos de pulsioximetría, incluyendo monitor, sensor y extensiones del sensor.

En esta práctica, los EMP más importantes son los de SpO₂ y frecuencia de pulso, porque son las variables simuladas con el OxSim OX-1.

### EMP para SpO₂
De acuerdo con el manual de operación de la serie uMEC, la medición de SpO₂ tiene un rango de 0 a 100 %, resolución de 1 % y exactitud de:

| Rango de SpO₂ | Tipo de paciente    | EMP / exactitud |
| ------------- | ------------------- | --------------: |
| 70 % a 100 %  | Adulto / pediátrico |            ±2 % |
| 70 % a 100 %  | Neonato             |            ±3 % |
| 0 % a 69 %    | No especificado     | No especificado |

El manual también indica que la exactitud de SpO₂ fue verificada comparando las mediciones del pulsioxímetro con muestras de sangre arterial medidas con cooxímetro.

Para esta práctica, como se trabaja con valores entre 85 % y 99 %, se puede tomar como referencia:

EMP SpO₂ = ±2 % para adulto/pediátrico.

### EMP para frecuencia de pulso desde SpO₂.
Cuando la frecuencia se obtiene a partir del módulo de SpO₂, el manual de la serie uMEC reporta un rango de medición de 20 a 300 bpm, resolución de 1 bpm y exactitud de ±3 bpm.

Por tanto, para la práctica:

EMP frecuencia de pulso = ±3 bpm

Esto aplica directamente a las pruebas realizadas con el OxSim OX-1, ya que el monitor recibe la señal a través del sensor de SpO₂.

### EMP para frecuencia cardíaca por ECG
Si el monitor mide frecuencia cardíaca usando ECG, la hoja técnica de la serie uMEC 100/120/150 reporta una exactitud de:

±1 bpm o ±1 %, el valor que sea mayor

También reporta un rango de HR de 10 a 300 bpm en adulto y de 10 a 350 bpm en paciente pediátrico/neonatal.

Sin embargo, en esta práctica no se está usando ECG, sino el sensor de SpO₂ conectado al simulador. Por eso, para los cálculos del laboratorio es más adecuado usar el EMP de frecuencia de pulso desde SpO₂: ±3 bpm.

### EMP para perfusión
El índice de perfusión no se evalúa como una variable fisiológica principal con un error máximo permitido específico en esta práctica. Su función es representar la calidad o intensidad de la señal pulsátil. La hoja técnica del uMEC indica que el equipo cuenta con índice de perfusión y tono de pulso en el módulo de SpO₂.

Para la baja perfusión, más que calcular un error porcentual, se recomienda evaluar:

-si la lectura de SpO₂ se mantiene estable;
-si la frecuencia de pulso se mantiene estable;
-si la onda fotopletismográfica disminuye su amplitud;
-si se genera una falsa alarma;
-si el monitor tarda más en estabilizar la medición.

La FDA recomienda que, para obtener valores confiables de SpO₂ y frecuencia de pulso, se consideren condiciones de señal inadecuada, como baja intensidad de señal o lecturas inestables.

## Tabla resumen de variables simuladas y EMP
| Variable simulada           | Equipo que la simula                    | Equipo que la mide         | Rango o modos usados en práctica | EMP recomendado                                  |
| --------------------------- | --------------------------------------- | -------------------------- | -------------------------------- | ------------------------------------------------ |
| SpO₂                        | OxSim OX-1                              | uMEC 100                   | 85 %, 95 %, 98 %, 99 %           | ±2 % en adulto/pediátrico                        |
| Frecuencia de pulso         | OxSim OX-1                              | uMEC 100 por SpO₂          | 40, 80 y 140 bpm                 | ±3 bpm                                           |
| Frecuencia cardíaca por ECG | No se usa directamente en esta práctica | uMEC 100 por ECG           | 10 a 300 bpm en adulto           | ±1 bpm o ±1 %, el mayor                          |
| Perfusión                   | OxSim OX-1                              | uMEC 100 / calidad de onda | PI aprox. 2.0 y 0.2              | No se especifica EMP; se evalúa calidad de señal |
| Onda fotopletismográfica    | OxSim OX-1                              | Pantalla del uMEC 100      | Onda normal y baja perfusión     | Evaluación visual/cualitativa                    |

Con base en la revisión bibliográfica, se identificó que el monitor Mindray uMEC 100 permite el monitoreo de variables fisiológicas como SpO₂, frecuencia de pulso y frecuencia cardíaca, mientras que el simulador Pronk OxSim OX-1 permite recrear condiciones específicas de pulsioximetría mediante valores controlados de saturación, frecuencia y perfusión. Para la práctica, los principales criterios de comparación son el error de SpO₂, con una tolerancia aproximada de ±2 % en adulto/pediátrico, y el error de frecuencia de pulso, con una tolerancia de ±3 bpm. La baja perfusión se evalúa principalmente a partir de la estabilidad de la lectura y la calidad de la onda fotopletismográfica.

## Referencias.

[1] Universidad Militar Nueva Granada. Guía de preparación práctica de laboratorio: Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas. Instrumentación Biomédica y Biosensores, 2025.

[2] Mindray. uMEC 100/120/150 Patient Monitor Data Sheet. Shenzhen Mindray Bio-Medical Electronics Co., Ltd.

[3] Mindray. uMEC Series Patient Monitor Operator’s Manual. Shenzhen Mindray Bio-Medical Electronics Co., Ltd.

[4] Pronk Technologies. OX-1 OxSim Optical SpO₂ Pulse Oximeter Simulator.

[5] International Organization for Standardization. ISO 80601-2-61:2017, Medical electrical equipment — Particular requirements for basic safety and essential performance of pulse oximeter equipment.

[6] U.S. Food and Drug Administration. Pulse Oximeters for Medical Purposes: Non-Clinical and Clinical Performance Testing, Labeling, and Premarket Submission Recommendations. 2025.
