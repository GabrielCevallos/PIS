# ProyectoIntegradorPIS

Integrantes: Gabriel Cevallos, Francisco Jaramillo, Jimmy Ontaneda, Ariana Sarango, Nathaly Camacho.

Ciclo: Segundo "A"
                                                                                                                                                             
DIAGRAMA UML


![Sin título](https://github.com/FrancisJaramilloC/ProyectoIntegradorPIS/assets/166524335/44aa6623-1bb8-4805-b914-c8f8325c233c)

# Estructura PIS

Esta estructura describe cómo se organizan las diferentes clases y módulos dentro del proyecto de control del brazo robótico.

- **Contenido:** Control de un brazo robótico. 

- **RoboticArm:** Clase principal para la gestión del brazo robótico.

### Componentes del Brazo Robótico

1. Base.
2. Forearm (Antebrazo).
3. Gripper (Pinza).

### Motores y sensores

Módulo para la gestión de:

1. StepperMotor (Motor paso a paso).
2. Servomotor.
3. Encoder.
4. Button (Botones).
5. WeightSensor (Sensores de peso).
6. Camera.

### Enumeraciones

1. **State:** Define los estados posibles de los componentes.

### Herencia

1. **Motor:** Clase base para motores.
2. **StepperMotor:** Subclase de Motor para motores paso a paso.
3. **Servomotor:** Subclase de Motor para servomotores.

### Composiciones

1. **RoboticArm:** Compuesto por 'Base', 'Forearm', 'Gripper', 'Esp32Cam' y 'WeightSensor'.
2. **Esp32Cam:** Compuesto por 'Camera'.
3. **Base:** Compuesto por 'StepperMotor'.
4. **Forearm:** Compuesto por 'Servomotor'.
5. **StepperMotor:** Compuesto por 'Encoder'.
6. **Servomotor:** Asociado con 'Button'.
