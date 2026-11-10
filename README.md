# Tutorial-Fusion-Fibra-Optica



TCB304-fusion-fibra-optica/
├── .gitignore
├── README.md
└── assets/
    └── img/
        ├── epp_seguridad.png
        ├── stripping_limpieza.png
        ├── corte_cleaver_90.png
        ├── fusion_arco_electrico.png
        └── manguito_termocontraible.png



        
# Archivos del sistema operativo
.DS_Store
Thumbs.db
desktop.ini

# Archivos de editores de código e IDEs
.vscode/
.idea/
*.swp
*.swo

# Archivos temporales y de registros
*.tmp
*.log



# Manual Técnico: Fusión de Fibra Óptica y Cálculo de Presupuesto Óptico

**Asignatura:** Infraestructura de Redes (TCB304)  
**Unidad:** Unidad 2 - Infraestructura de redes de fibra óptica  
**Institución:** INACAP Sede La Serena  
**Estudiante:** Dario Antonio Carvajal Reines  
**Carrera:** Ingeniería en Telecomunicaciones y Servicios Digitales  

---

## Glosario Técnico Exprés

* **Núcleo (Core):** Centro de vidrio ultra puro por donde viaja la luz mediante reflexión interna total[cite: 1].
* **Revestimiento (Cladding):** Capa exterior de vidrio (125 µm) con menor índice de refracción que confina la luz en el núcleo[cite: 1].
* **Cleaving (Corte de Precisión):** Proceso de fractura controlada del vidrio para lograr un extremo plano a 90° respecto al eje de la fibra[cite: 1].
* **Atenuación:** Pérdida de potencia óptica de la señal expresada en decibelios (dB) a lo largo del enlace[cite: 1].

---

## 1. Seguridad y Manejo de Materiales

El trabajo con fibra óptica requiere estrictas medidas de seguridad debido a los riesgos asociados a esquirlas de vidrio invisibles y luz láser inaudible.

### Equipos de Protección Personal (EPP) y Contención
1. **Lentes de Seguridad:** Protección ocular obligatoria en todo momento para evitar que las esquirlas salten a los ojos[cite: 1].
2. **Contenedor Rígido para Residuos:** Disposición inmediata de restos de fibra cortada en frascos metálicos o plásticos rígidos etiquetados[cite: 1]. Nunca botar restos al suelo o basureros comunes.

![Seguridad y EPP en Taller](assets/img/epp_seguridad.png)  
*Figura 1: Uso de lentes de protección ocular y depósito de residuos de vidrio en contenedor rígido.*

> [!WARNING]
> **ADVERTENCIA DE SEGURIDAD:** Las esquirlas de fibra de vidrio pueden penetrar la piel o ser ingeridas/inhaladas si no se recolectan adecuadamente. No consumir alimentos ni bebidas en la mesa de trabajo.

---

## 2. Preparación de la Fibra Óptica (Stripping y Limpieza)

### Paso 1: Stripping (Pelado de la Fibra)
1. Tomar la **pinza peladora tri-hole (3 muescas)** en el ángulo correcto.
2. Utilizar la muesca más pequeña para retirar el recubrimiento primario (acrilato de 250 µm) hasta exponer el vidrio desnudo de **125 µm**[cite: 1].
3. Realizar pases cortos de 2 a 3 cm para evitar mellar o fisurar el hilo de vidrio[cite: 1].

### Paso 2: Limpieza de Precisión
1. Humedecer un paño de limpieza libre de pelusa (*lint-free wipe*) con **alcohol isopropílico de 99.9% de pureza**[cite: 1].
2. Envolver el hilo expuesto con el paño y deslizar firmemente desde la base hacia el extremo.
3. Repetir hasta escuchar el "chirrido" característico que indica total ausencia de impurezas o grasas.

![Stripping y Limpieza de la Fibra](assets/img/stripping_limpieza.png)  
*Figura 2: Pelado de capa protectora a 125 µm y desinfección con alcohol isopropílico.*

> [!WARNING]
> **ADVERTENCIA TÉCNICA:** Jamás limpie la fibra desnudada DESPUÉS de haber realizado el corte (cleaving). La limpieza debe hacerse siempre ANTES del corte para no contaminar o fracturar el ángulo de corte.

---

## 3. Corte de Precisión (Cleaving)

El empalme por fusión requiere extremos rectos y planos para garantizar una unión de baja pérdida.

1. Deslizar previamente el **manguito termo-contraíble (heat shrink sleeve)** en una de las fibras[cite: 1].
2. Posicionar la fibra limpia en la guía milimétrica de la cortadora de precisión (*cleaver*)[cite: 1].
3. Fijar la fibra garantizando una longitud expuesta de stripping entre 10 mm y 16 mm.
4. Ejecutar el deslizamiento de la cuchilla giratoria de tungsteno para lograr un corte perpendicular con un ángulo **< 0.5° (cercano a los 90°)**[cite: 1].

```text
CORTE OPTIMO (90°):              CORTE DEFECTUOSO (Ángulo o Bisel):
+-----------------+              +-----------------/
|                 | 90°          |                /  Ángulo > 1.0°
+-----------------+              +---------------/
[Pérdida típica: 0.01 - 0.03 dB] [Pérdida alta o error de alineación]
```

![Corte con Cleaver](assets/img/corte_cleaver_90.png)  
*Figura 3: Operación de cortadora de precisión (cleaver) y verificación del ángulo perpendicular.*

---

## 4. Proceso de Termofusión

La termofusión une dos núcleos de vidrio utilizando un arco eléctrico de alta frecuencia[cite: 1].

### Paso a Paso de la Fusión
1. Encender la fusionadora y seleccionar el programa correspondiente al tipo de fibra (Ejemplo: *SM G.652* para Monomodo)[cite: 1].
2. Abrir la cubierta de la fusionadora y colocar cuidadosamente ambas fibras sobre las guías en V (*V-grooves*), asegurando que los extremos no queden tocando los electrodos[cite: 1].
3. Cerrar la cubierta para iniciar el proceso automático:
   * **Limpieza previa:** Un miniarco eléctrico elimina partículas residuales de micro-suciedad.
   * **Alineación:** Los motores paso a paso alinean los núcleos o claddings en los ejes X e Y[cite: 1].
   * **Arco de Fusión:** Funde las puntas y une mecánicamente ambas fibras[cite: 1].
4. Abrir la tapa y desplazar la funda termo-contraíble sobre el punto de fusión sin doblar la fibra[cite: 1].
5. Colocar el conjunto en el horno integrado de la máquina a 60 °C - 80 °C durante aproximadamente 20 segundos hasta que el tubo se encoja por completo[cite: 1].

![Proceso de Termofusión](assets/img/fusion_arco_electrico.png)  
*Figura 4: Alineación de fibras en fusionadora y horneado de manguito termocontraíble.*

---

## 5. Análisis de Resultados y Presupuesto Óptico

El **Presupuesto Óptico** (Power Budget) determina la pérdida máxima permitida en un enlace de telecomunicaciones para asegurar que la señal llegue con potencia suficiente al receptor[cite: 1].

### Fórmula Fundamental del Presupuesto Óptico

$$A_{total} = (L \cdot \alpha) + (N_{conn} \cdot A_{conn}) + (N_{fusion} \cdot A_{fusion}) + M_{GPON}$$

Donde:
* $L$: Longitud del enlace (km).
* $\alpha$: Atenuación atenuación lineal de la fibra ($\text{dB/km}$).
* $N_{conn}$: Número de conectores en el enlace.
* $A_{conn}$: Atenuación máxima por conector ($\text{dB}$).
* $N_{fusion}$: Número de empalmes por fusión.
* $A_{fusion}$: Atenuación máxima por empalme por fusión ($\text{dB}$).
* $M_{GPON}$: Margen de seguridad/diseño de la red ($\text{dB}$).

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

### Medición y Verificación de Resultados

Una vez finalizada la fusión, se registran y comparan los valores estimados por el equipo con los límites de la norma:

* **Estimación de la Fusionadora:** La fusionadora estimó una pérdida de **0.02 dB** en el punto de fusión.
* **Criterio de Aprobación:** Un empalme se considera **conforme (APROBADO)** si la pérdida medida es menor o igual a **0.05 dB** por fusión.
* **Conclusión del Enlace:** Al obtener $0.02\text{ dB} \le 0.05\text{ dB}$, se certifica que la fusión es de excelente calidad técnica y que el enlace cumple holgadamente los parámetros exigidos por la arquitectura GPON.

---

## 6. Advertencias sobre Errores Comunes en Taller

> [!WARNING]
> **ERROR 1: Olvidar introducir el protector termo-contraíble.**  
> Si fusiona las fibras sin haber deslizado antes el manguito en uno de los extremos, deberá cortar la fusión y repetir todo el proceso desde el stripping[cite: 1].

> [!WARNING]
> **ERROR 2: Tocar la fibra desnudada con los dedos.**  
> Los aceites corporales contaminan la superficie de sílice provocando arcos débiles y elevadas pérdidas por atenuaicón (> 0.5 dB).

> [!WARNING]
> **ERROR 3: Ángulo de corte inclinado (> 1.0°).**  
> Si la fusionadora arroja advertencia de ángulo de corte defectuoso en la pantalla LCD, no fuerce el disparo del arco; descarte el extremo y realice un nuevo corte en el cleaver[cite: 1].

---

## Referencias Técnicas
1. ITU-T Recommendation G.652 (11/2016): *Characteristics of a single-mode optical fibre and cable*.
2. Apuntes de Asignatura TCB304: *Infraestructura de Redes - Unidad 2: Planta Interna y Externa*, INACAP[cite: 1].





# 1. Inicializar el repositorio Git
git init

# 2. Configurar usuario local (si no está configurado)
git config user.name "Dario Carvajal"
git config user.email "dario.carvajal@inacapmail.cl"

# 3. Primer Commit: Estructura base y gitignore
git add .gitignore
git commit -m "docs: agregar .gitignore para omitir archivos temporales"

# 4. Segundo Commit: Creación del archivo README base
git add README.md
git commit -m "docs: agregar estructura inicial del manual tecnico en README.md"

# 5. Tercer Commit: Incorporar recursos visuales en la carpeta assets
git add assets/img/
git commit -m "feat(assets): incorporar esquemas e imagenes de seguridad, stripping y fusion"

# 6. Cuarto Commit: Completar Glosario y Sección de Seguridad
git add README.md
git commit -m "docs: completar glosario tecnico express y sección de EPP y seguridad"

# 7. Quinto Commit: Agregar detalles de Stripping, Cleaving y Fusión
git add README.md
git commit -m "docs: detallar pasos de pelado, corte a 90 grados y termofusion"

# 8. Sexto Commit: Agregar Tabla de Presupuesto Óptico y Mediciones
git add README.md
git commit -m "feat(presupuesto): incluir formula, tabla de presupuesto optico GPON y analisis de pérdidas"

# 9. Séptimo Commit: Revisión final y advertencias técnicas
git add README.md
git commit -m "style: agregar advertencias de errores comunes y referencias normativas ITU-T"
