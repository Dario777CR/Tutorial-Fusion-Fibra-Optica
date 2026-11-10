# Sistema Operativo
.DS_Store
Thumbs.db
desktop.ini

# Editores e IDEs
.vscode/
.idea/
*.swp
*.swo

# Temporales y Logs
*.tmp
*.log


# 📡 Manual Técnico: Fusión de Fibra Óptica y Presupuesto Óptico

**Asignatura:** Infraestructura de Redes (TCB304)  
**Unidad:** Unidad 2 - Infraestructura de redes de fibra óptica  
**Sede:** INACAP Sede La Serena  
**Estudiante:** Dario Antonio Carvajal Reines  
**Carrera:** Ingeniería en Telecomunicaciones y Servicios Digitales  

---

## 📚 Glosario Técnico Exprés

* **Núcleo (Core):** Centro de vidrio ultra puro por donde viaja la luz mediante el fenómeno de reflexión interna total.
* **Revestimiento (Cladding):** Capa exterior de vidrio (125 µm) con menor índice de refracción que confina la luz en el núcleo.
* **Cleaving (Corte de Precisión):** Proceso de fractura controlada del vidrio para lograr un extremo plano a 90° respecto al eje de la fibra.
* **Atenuación:** Pérdida de potencia óptica de la señal expresada en decibelios (dB) a lo largo del enlace.

---

## 🥽 1. Seguridad y Manejo de Materiales

El trabajo con fibra óptica exige el cumplimiento riguroso de protocolos de seguridad para prevenir lesiones por esquirlas de vidrio invisibles.

### Protocolos Obligatorios
1. **Lentes de Seguridad:** Uso permanente de protección ocular para evitar el impacto de esquirlas de vidrio en los ojos.
2. **Contenedor Rígido de Residuos:** Disposición inmediata de restos de fibra cortada en recipientes plásticos o metálicos rígidos debidamente rotulados.

![Seguridad y EPP en Taller](assets/img/epp_seguridad.png)  
*Figura 1: Uso de EPP obligatorio y manejo seguro de residuos de vidrio en contenedor rígido.*

> [!WARNING]
> **ADVERTENCIA DE SEGURIDAD:** Las esquirlas de vidrio pueden penetrar la piel o ser ingeridas/inhaladas si no se recolectan adecuadamente. Queda estrictamente prohibido consumir alimentos o bebidas en el área de trabajo.

---

## ✂️ 2. Preparación de la Fibra Óptica (Stripping y Limpieza)

### Paso 1: Stripping (Pelado de la Fibra)
1. Utilizar la pinza peladora tri-hole (3 muescas) en la posición adecuada.
2. Usar la muesca más pequeña para remover el recubrimiento primario (acrilato de 250 µm) hasta exponer la fibra desnuda a **125 µm** sin mellar el vidrio.
3. Realizar el pelado en tramos cortos de 2 a 3 cm.

### Paso 2: Limpieza de Precisión
1. Humedecer un paño libre de pelusa (*lint-free wipe*) con **alcohol isopropílico al 99.9% de pureza**.
2. Envolver la fibra expuesta y deslizar el paño desde la base hacia la punta.
3. Repetir la limpieza hasta escuchar el chirrido característico que confirma la ausencia de impurezas y grasas.

![Stripping y Limpieza de la Fibra](assets/img/stripping_limpieza.png)  
*Figura 2: Pelado de capa protectora a 125 µm y limpieza de precisión con alcohol isopropílico.*

> [!WARNING]
> **ADVERTENCIA TÉCNICA:** La limpieza debe ejecutarse SIEMPRE antes del corte con la cortadora de precisión (cleaver). Nunca limpie la fibra después de cortada, ya que recontaminará o fisurará el extremo del vidrio.

---

## 🔪 3. Corte de Precisión (Cleaving)

1. Insertar con anticipación el **manguito termo-contraíble (heat shrink sleeve)** en uno de los hilos de fibra.
2. Colocar la fibra limpia en la guía milimétrica de la cortadora de precisión (*cleaver*), asegurando un largo expuesto de 10 mm a 16 mm.
3. Presionar la tapa y deslizar el carro con disco de tungsteno para realizar una fractura plana perpendicular cercana a los **90° (< 0.5° de inclinación)**.

```text
CORTE ÓPTIMO (90°):              CORTE DEFECTUOSO (Ángulo o Bisel):
+-----------------+              +-----------------/
|                 | 90°          |                /  Ángulo > 1.0°
+-----------------+              +---------------/
[Pérdida típica: 0.01 - 0.03 dB] [Rechazado por la fusionadora]
```

![Corte con Cleaver](assets/img/corte_cleaver_90.png)  
*Figura 3: Operación de cortadora de precisión (cleaver) y verificación del ángulo perpendicular.*

---

## ⚡ 4. Proceso de Termofusión

1. Encender la fusionadora de arco eléctrico y seleccionar el programa de alineación según el tipo de fibra (ej. Monomodo ITU-T G.652).
2. Posicionar los extremos de ambas fibras en las guías en V (*V-grooves*), asegurando que queden dentro del campo visual de las cámaras pero sin tocar los electrodos.
3. Cerrar la cubierta para ejecutar la secuencia automática:
   * **Limpieza por arco:** Descarga eléctrica breve para eliminar micro-polvo.
   * **Alineación:** Motores de alta precisión alinean los núcleos/claddings en los ejes X e Y.
   * **Fusión:** Descarga principal de arco eléctrico que funde y une de forma homogénea ambos hilos.
4. Deslizar la funda termo-contraíble sobre la zona empalmada y posicionarla en el horno integrado de la máquina (60 °C - 80 °C durante 20 segundos) para brindar protección mecánica.

![Proceso de Termofusión](assets/img/fusion_arco_electrico.png)  
*Figura 4: Alineación de núcleos en fusionadora por arco eléctrico y protección termo-contraíble.*

---

## 📊 5. Análisis de Resultados y Presupuesto Óptico

El **Presupuesto Óptico** determina la atenuación máxima total permitida en el enlace para garantizar la potencia adecuada en la recepción de la señal.

### Fórmula del Presupuesto Óptico

$$A_{total} = (L \cdot \alpha) + (N_{conn} \cdot A_{conn}) + (N_{fusion} \cdot A_{fusion}) + M_{GPON}$$

Donde:
* $L$: Longitud total de la fibra (km).
* $\alpha$: Atenuación lineal del hilo ($\text{dB/km}$).
* $N_{conn}$: Número de conectores en el trayecto.
* $A_{conn}$: Pérdida individual por conector ($\text{dB}$).
* $N_{fusion}$: Número de empalmes por fusión.
* $A_{fusion}$: Pérdida individual por fusión ($\text{dB}$).
* $M_{GPON}$: Margen de seguridad y diseño para red GPON ($\text{dB}$).

---

### Tabla de Presupuesto Óptico (Enlace Modelo GPON Monomodo a 1310 nm)

| Elemento de la Red | Cantidad / Unidad | Valor Unitario Teórico | Pérdida Total Teórica (dB) |
| :--- | :--- | :--- | :--- |
| **Fibra Monomodo (ITU-T G.652.D @ 1310nm)** | 2.5 km | 0.35 dB/km | **0.875 dB** |
| **Conectores Ópticos (SC/APC)** | 2 unidades | 0.30 dB/conector | **0.600 dB** |
| **Empalmes por Fusión** | 2 empalmes | 0.05 dB/empalme | **0.100 dB** |
| **Margen de Seguridad / GPON** | 1 sistema | 3.00 dB | **3.000 dB** |
| **ATENUACIÓN TOTAL TEÓRICA PERMITIDA** | - | - | **4.575 dB** |

---

### Medición y Verificación de Resultados en Taller

* **Estimación de la Fusionadora:** **0.02 dB**[cite: 1, 2].
* **Criterio de Aprobación Standard:** Pérdida $\le 0.05\text{ dB}$ por empalme[cite: 2].
* **Evaluación:** Dado que $0.02\text{ dB} \le 0.05\text{ dB}$, el empalme resulta **APROBADO**, garantizando la viabilidad técnica y operativa del enlace GPON[cite: 1, 2].

---

## ⚠️ 6. Advertencias sobre Errores Comunes

> [!WARNING]
> **ERROR 1: Omitir la inserción del termo-contraíble.**  
> Si se realiza la fusión sin haber colocado previamente el manguito en el hilo, habrá que cortar la fibra y repetir todo el proceso.

> [!WARNING]
> **ERROR 2: Contacto manual con la fibra desnudada.**  
> Tocar el vidrio expuesto deja residuos grasos corporales que alteran el arco eléctrico y causan atenuaciones superiores a 0.5 dB.

> [!WARNING]
> **ERROR 3: Ángulo de cleaving fuera de norma (> 1.0°).**  
> Si la fusionadora indica fallo en el ángulo de corte, cancele el ciclo, descarte el extremo y realice un nuevo corte en la cleaver.

---

## 📑 Referencias Técnicas
1. Recommendation ITU-T G.652 (11/2016): *Characteristics of a single-mode optical fibre and cable*.
2. Manual de Asignatura TCB304: *Infraestructura de Redes - Unidad 2: Planta Interna y Externa*, INACAP[cite: 1].
