### 1. Concepto y Tipos de Dispositivos Móviles

Un **dispositivo móvil** es un equipo electrónico de cómputo pequeño, con capacidad de procesamiento, conexión inalámbrica, batería autónoma y diseñado para ser transportado y operado fácilmente con una mano o ambas hands.

* **Smartphones:** Dispositivos optimizados para la comunicación por voz/datos cellular, ultraportables (pantallas de 5.5" a 6.8") y con alta densidad de sensores.
* **Tablets:** Equipos orientados al consumo de contenido, productividad y multimedia, con pantallas más grandes (8" a 14") y mayor capacidad de batería.
* **Wearables (Smartwatches / Pulseras):** Enfocados en monitoreo biométrico y notificaciones en tiempo real, con procesadores de ultra bajo consumo.
* **Laptops/Convertibles:** Dispositivos móviles de alta capacidad de cómputo con arquitectura x86/ARM de escritorio.

---

### 2. Cuadro Comparativo: Smartphone vs. Tablet

| Característica | Smartphone | Tablet |
| --- | --- | --- |
| **Tamaño de Pantalla** | 5.5" – 6.8" | 8.0" – 14.6" |
| **Batería** | 3,000 – 5,000 mAh | 7,000 – 11,000 mAh |
| **Conectividad Principal** | Redes Celulares (4G/5G) + Wi-Fi | Principalmente Wi-Fi (Celular opcional) |
| **Casos de Uso** | Comunicación inmediata, fotos rápidas, movilidad extrema | Productividad, lectura, dibujo digital, consumo multimedia |
| **Sensores** | Alta densidad (GPS, giroscopio, NFC, acelerómetro, etc.) | Estándar (Alerómetro, luz ambiental, GPS opcional) |

---

### 3. Arquitectura Hardware y Componentes Internos

#### A. Placa Lógica (Mainboard / Motherboard)

Es la tarjeta de circuito impreso (PCB) multicapa donde se interconectan todos los componentes electrónicos mediante buses de alta velocidad. Optimizada para minimizar el espacio físico y el consumo energético.

#### B. Procesador (SoC - System on Chip)

A diferencia de las PCs, en móviles el procesador está integrado en un solo chip de silicio que contiene:

* **CPU (Central Processing Unit):** Núcleos de alto rendimiento y núcleos de eficiencia (Arquitectura ARM BIG.little / DynamIQ).
* **GPU (Graphics Processing Unit):** Procesamiento gráfico 2D/3D y renderizado de interfaz.
* **NPU/TPU (Neural Processing Unit):** Aceleración de tareas de Inteligencia Artificial y aprendizaje automático.
* **Módem:** Gestión de bandas de radiofrecuencia (5G/4G LTE).
* **ISP (Image Signal Processor):** Procesamiento de señales de las cámaras en tiempo real.

#### C. Memoria y Almacenamiento

* **RAM (LPDDR4X / LPDDR5X):** Memoria de acceso aleatorio de bajo consumo para multitarea y ejecución de apps.
* **Almacenamiento Interno (UFS 3.1 / UFS 4.0 / eMMC):** Memoria flash no volátil donde se aloja el sistema operativo (Android/iOS) y las aplicaciones.

#### D. Pantalla

Unidad de salida y entrada (Digitalizador táctil integrado).

* **Tecnologías:** OLED / AMOLED (píxeles autoemitidos, negros puros) y LCD/IPS (requieren retroiluminación).
* **Controlador Táctil:** Captura los toques mediante variaciones capacitivas.

#### E. Batería

* **Química:** Ion de Litio (Li-ion) o Polímero de Litio (Li-Po).
* **Circuito PMIC (Power Management IC):** Regula las cargas, voltajes y previene sobrecalentamientos.

#### F. Módulos de Comunicación

* **Transceptor de Radiofrecuencia (RF):** Controla antenas para 4G/5G, Wi-Fi, Bluetooth y GPS.
* **NFC (Near Field Communication):** Pagos móviles y emparejamiento cercano.

#### G. Sensores y Cámaras

* **Sensores:** Acelerómetro, Giroscopio, Magnetómetro (Brújula), Sensor de Proximidad, Sensor de Luz Ambiental, Lector de Huellas (óptico/ultrasónico).
* **Sistema de Cámaras:** Sensores CMOS, lentes gran angular/telefoto y motores OIS (estabilización óptica).

---

### 4. Esquema de Arquitectura Básica (Para elaborar en clase)

```
+-----------------------------------------------------------------------+
|                            PANTALLA TÁCTIL                            |
+-----------------------------------+-----------------------------------+
                                    |
                                    v
+-----------------------------------------------------------------------+
|                             PLACA LÓGICA                              |
|  +-----------------------------------------------------------------+  |
|  |                           SoC (CHIP)                            |  |
|  |  +-------------------+  +------------------+  +--------------+  |  |
|  |  |     CPU (ARM)     |  |       GPU        |  |   NPU (IA)   |  |  |
|  |  +-------------------+  +------------------+  +--------------+  |  |
|  |  | Módem (5G/Wi-Fi)  |  | ISP (Foto/Video) |  |     PMIC     |  |  |
|  |  +-------------------+  +------------------+  +--------------+  |  |
|  +-----------------------------------------------------------------+  |
|                                   |                                   |
|   +-------------------+   +---------------+   +-------------------+   |
|   | Memoria RAM LPDDR |   | Almacenamiento|   | Sensores (Giro,   |   |
|   |                   |   | Flash (UFS)   |   | Acelerómetro...)  |   |
|   +-------------------+   +---------------+   +-------------------+   |
+-----------------------------------+-----------------------------------+
                                    |
            +-----------------------+-----------------------+
            |                                               |
            v                                               v
+-----------------------+                       +-----------------------+
|  SISTEMA DE BATERÍA   |                       | MÓDULOS DE CÁMARA Y  |
|      (Li-Po / PMIC)   |                       |   CONECTIVIDAD (RF)   |
+-----------------------+                       +-----------------------+

```
