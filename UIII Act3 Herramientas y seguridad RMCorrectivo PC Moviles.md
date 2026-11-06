### 1. Herramientas de Precisión y Equipos de Medición

Para el desensamble y diagnóstico de dispositivos móviles se utilizan herramientas diseñadas para evitar daños mecánicos en componentes SMD e integrados delicados:

* **Destornilladores de Precisión:** Puntas magnéticas de alta durabilidad en calibres específicos (Torx T2/T3/T4/T5, Pentalobe P2 0.8mm para iPhone, Tri-Point Y0.6, Phillips PH000).
* **Herramientas de Apertura:** Ventosas de succión, púas de plástico (picks) y espátulas plásticas (*spudgers*). Se evita el uso de herramientas metálicas directas sobre bordes de pantallas.
* **Pinzas de Precisión (ESD-safe):** Pinzas de punta fina recta y curva con recubrimiento antiestático para manipular conectores FPC y microcomponentes.
* **Estación de Calor / Plancha de Separación:** Ajustadas a temperaturas controladas (80 °C – 100 °C) para ablandar adhesivos estructurales sin degradar la pantalla u OLED.
* **Equipos de Medición:**
* *Multímetro Digital:* Medición de continuidad, voltaje de batería ($3.7\text{ V} - 4.4\text{ V}$) y caída de tensión en diodos.
* *Fuente de Alimentación Regulada (DC Power Supply):* Inyección de voltaje ($3.8\text{ V} - 4.2\text{ V}$) para verificar consumos de corriente y detectar cortocircuitos.



---

### 2. Protección Contra Descargas Electrostáticas (ESD)

La electricidad estática del cuerpo humano (que puede superar los $2,000\text{ V}$) destruye circuitos integrados sin dejar huella visible.

| Elemento ESD | Función y Aplicación Práctica |
| --- | --- |
| **Pulsera Antiestática** | Descarga la electricidad estática del técnico a tierra. Debe conectarse a un punto común de tierra con resistencia de $1\text{ M}\Omega$. |
| **Tapete ESD (ESD Mat)** | Superficie de trabajo disipativa que evita acumulación de cargas y protege los chasis de rayaduras. |
| **Guantes o Dediles Antiestáticos** | Evitan la transferencia de estática y la acumulación de grasa corporal en los conectores. |

---

### 3. Seguridad en la Manipulación de Baterías de Litio (Li-ion / Li-Po)

Las baterías de ion de litio almacenan alta densidad de energía química. Su perforación o cortocircuito provoca **embalamiento térmico** (*thermal runaway*).

#### Riesgos Asociados:

* **Riesgo Térmico:** Incendios espontáneos y temperaturas superiores a $600\text{ }^\circ\text{C}$.
* **Riesgo Químico / Químico-Tóxico:** Emisión de gases tóxicos (fluoruro de hidrógeno) si la celda se perfora.
* **Riesgo Mecánico:** Deformación o ignición por presión directa con palancas metálicas.

> **Regla de Oro:** NUNCA utilizar herramientas metálicas, punzantes o afiladas cerca de la batería. Se debe retirar la batería aplicando alcohol isopropílico para disolver el adhesivo o jalando las tiras adhesivas de extracción (*pull tabs*). En caso de ignición, utilizar arena seca o un extintor Clase D/polvo seco (nunca agua).

---

### 4. Secuencia de Desensamble Seguro (Práctica Guiada)

1. **1. Preparación del Área y EPP:** Desconexión de energía exterior y seguridad laboral.
Colocar tapete ESD, conectar la pulsera antiestática a tierra y colocarse gafas de protección visual. Apagar el dispositivo por completo y retirar la bandeja SIM/MicroSD.


2. **2. Aplicación de Calor Estructurado:** Uso controlado de temperatura.
Calentar el borde posterior de la tapa/pantalla con estación de aire caliente a 80 °C durante 3 a 5 minutos. Usar ventosa y púas plásticas para cortar el adhesivo sin profundizar más de 3 mm.


3. **3. Desconexión Inmediata de la Batería:** Paso crítico obligatorio antes de manipular cualquier otro componente.
Una vez retirada la tapa/pantalla, retirar el blindaje metálico del conector de la batería y desconectarla usando **únicamente** un *spudger* de plástico.


4. **4. Desmontaje de Placa Lógica y Módulos:** Orden de tornillería y flexes.
Organizar los tornillos por tamaño y posición en un organizador magnético. Desconectar los cables flex (pantalla, cámara, carga) con presión vertical suave y extraer la tarjeta madre.
