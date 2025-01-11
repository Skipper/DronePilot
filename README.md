# 🚀 Proyecto DronePilot: Construcción y Control desde Cero  

## 📝 Introducción  
**DronePilot** es un proyecto desarrollado completamente desde cero para demostrar conocimientos avanzados en todas las fases de construcción de un dron. Desde el ensamblaje del hardware hasta la programación personalizada del sistema de control, este proyecto utiliza un enfoque innovador y experimental.  

El dron utiliza un chasis **F450**, con un módulo **ESP32** que actúa como cerebro principal, integrando múltiples sensores y demostrando su capacidad de manejar tareas complejas simultáneamente. Esto incluye la creación de una estructura improvisada para un **PID Test Rig**, que permite afinar el controlador en los ejes **roll**, **pitch** y **yaw**.  

---

## 🌟 Características Clave  

### Etapa Actual: Desarrollo y Ensamblaje desde Cero  

#### Hardware Personalizado:  
- **Chasis**: F450 ensamblado manualmente.  
- **Conectores XT60** macho y hembra soldados a cables 14 AWG para alimentación eficiente.  
- **Motores brushless** de 1000 kV con conectores tipo banana (3.5 mm), conectados a cuatro ESC de 30A.  
- **Hélices**: 10x4.5 pulgadas, junto con una placa de distribución PDB-XT60 con BEC Matek (5V y 12V).  
- **Batería**: LiPo 3S de 2200 mAh, 35C.  

#### Software Personalizado:  
- Uso de un módulo **ESP32** en combinación con un sensor **MPU9250**.  
- Implementación de comunicación I2C para programar el acelerómetro, giroscopio y gestión de motores.  
- Código estructurado aplicando el **principio de responsabilidad única** y organización modular en carpetas y archivos.  
- Control de los motores en un rango de valores PWM (1300-2000) según los ejes de rotación (**yaw**, **roll**, **pitch**).  

#### Control Innovador:  
- En lugar de un transmisor y receptor RC, el dron se controla mediante **Micro ROS**, permitiendo operar desde un ordenador portátil.  

#### Estructura Improvisada para PID Test Rig:  
- Se diseñó una estructura improvisada para realizar pruebas y calibraciones en los ejes **roll**, **pitch** y **yaw**, optimizando el controlador PID del cuadricóptero.  

#### Sensores Adicionales y Periféricos:  
- **Zumbador** para alertas y notificaciones.  
- **Sensor de temperatura y humedad DHT11** para recopilar datos ambientales.  
- **Sensor ultrasónico HC-SR04** para medir distancias.  
- **Pantalla OLED 128x64** para mostrar información en tiempo real, como lecturas de los sensores y estado del sistema. 
- El **ESP32** demostró su potencia al gestionar correctamente todos estos sensores simultáneamente, mientras actúa como el cerebro principal del dron.  

---

## ⚙️ Estructura del Proyecto  

### Hardware  
- Ensamblaje detallado del chasis, motores, ESC y sistema de alimentación.  
- Configuración de la electrónica para asegurar eficiencia y seguridad.  
- Implementación de sensores adicionales y periféricos para ampliar la funcionalidad.  

### Software  
- Programación desde cero en el **IDE de Arduino** para el ESP32 y el MPU9250.  
- Enfoque en la estabilidad de vuelo y control básico, priorizando un manejo mediante **Micro ROS**.  
- Integración de los datos de los sensores en el sistema de control, mostrando información clave en la pantalla OLED.  

---

## 💻 Requisitos Técnicos  

### Hardware Implementado  
- **Chasis**: F450.  
- **Motores**: Brushless 1000 kV.  
- **Hélices**: 10x4.5 pulgadas.  
- **ESC**: 30A.  
- **Placa de distribución**: PDB-XT60 con BEC Matek (5V y 12V).  
- **Batería**: LiPo 3S de 2200 mAh, 35C.  
- **Controlador**: Módulo ESP32 con sensor MPU9250.  
- **Sensores Adicionales**:  
  - DHT11 (temperatura y humedad).  
  - HC-SR04 (ultrasónico).  
  - Pantalla OLED 128x64.  
  - Zumbador para alertas.  

### Software  
- **Lenguaje de programación**: C++ (Arduino IDE).  
- **Protocolo de comunicación**: I2C para interacción con sensores.  
- **Control**: Micro ROS para manejo remoto desde un computador portátil.  

---

## 🌟 Planes Futuros  

### Mejoras en el Hardware  
- Integración de sensores avanzados como **GPS** y cámaras HD.  
- Implementación de un sistema de detección de obstáculos más robusto utilizando **LiDAR A1**.  

### Expansión del Software  
- Desarrollo de una aplicación móvil nativa para control remoto y configuración avanzada.  
- Creación de rutas de vuelo predefinidas y modos autónomos.  
- Exploración de tecnologías innovadoras como control por gestos o comandos de voz.  

---

## ▶️ Instrucciones de Ejecución  

1. Ensamble el hardware siguiendo las especificaciones detalladas del proyecto.  
2. Programe el ESP32 utilizando el IDE de Arduino, asegurándose de configurar correctamente los sensores y periféricos.  
3. Configure **Micro ROS** en el ordenador portátil para el control remoto del dron.  
4. Utilice el **PID Test Rig improvisado** para realizar ajustes en los controladores de los ejes **roll**, **pitch** y **yaw**.  
5. Realice pruebas iniciales de vuelo en un entorno seguro, documentando los resultados.  

---

## 🔎 Casos de Uso  

- **Educación**: Introducción práctica al diseño y construcción de drones desde cero, ideal para entusiastas y estudiantes.  
- **Desarrollo Experimental**: Probar configuraciones personalizadas antes de implementar funcionalidades avanzadas.  
- **Futuras Aplicaciones**: Exploración de usos prácticos como videografía aérea, vigilancia automatizada o investigación académica.  
