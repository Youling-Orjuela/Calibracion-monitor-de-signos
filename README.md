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
