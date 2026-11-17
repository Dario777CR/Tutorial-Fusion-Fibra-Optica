# 🔌 Manual Técnico: Termofusión de Fibra Óptica y Presupuesto Óptico

* 📘 **Asignatura:** Infraestructura de Redes (TCB304)
* 🎓 Carrera:** Ingeniería en Telecomunicaciones y Servicios Digitales
* 👨‍💻 Autor: Darío Antonio Carvajal Reines
* 📅 **Fecha: 14 Noviembre 2026
* ⚡ Equipo Utilizado:** Fusionadora por Arco Eléctrico **Vcnex VFS-30** (Modo `SM00`)

---

## 📖 1. Glosario Técnico Exprés

* 🔦 **Núcleo (Core):Región central de vidrio de sílice dopado , por donde viaja la luz mediante reflexión interna total.
* 🛡️ **Cladding (Revestimiento): Capa de vidrio con menor índice de refracción que rodea al núcleo para confinar el haz óptico.
* ✂️ **Cleaving (Corte de Precisión):** Marcado y fractura mecánica controlada del vidrio para lograr una cara transversal limpia cercana 
* 📉 **Atenuación:** Pérdida de potencia óptica a lo largo del enlace producida por absorción, dispersión, empalmes y conectores.

---

## 🦺 2. Seguridad, EPP y Gestión de Residuos

Antes de intervenir el cable de fibra óptica, se prepara la estación de trabajo verificando los Elementos de Protección Personal (EPP) y los contenedores de seguridad.

![Estación de trabajo y EPP]
<table>
  <tr>
    <td align="center">
      <img src="assets/img/02-remocion-chaqueta-kevlar.jpg" alt="Remoción de chaqueta" width="350" /><br>
      <sub><b>Fig 1.</b> Remoción de chaqueta y Kevlar</sub>
    </td>
    <td align="center">
      <img src="assets/img/03-extraccion-buffer-hilos.jpg" alt="Aislamiento de tubos holgados" width="350" /><br>
      <sub><b>Fig 2.</b> Aislamiento de tubos holgados</sub>
    </td>
  </tr>
</table>


1. 🥽 **Protección Ocular y Manual:** Uso obligatorio de **lentes de seguridad transparentes** (visibles junto a la fusionadora) para proteger contra microfragmentos de vidrio y **guantes de precisión (*HyFlex*)** para manipular herramientas de corte con firmeza y sensibilidad táctil.
2. 🗑️ **Disposición Segura de Residuos:** Todos los recortes de fibra desnuda de $125\ \mu\text{m}$ se depositan de inmediato en el **contenedor blanco con tapa amarilla** del kit (junto al dispensador de alcohol), evitando riesgos de punción cutánea.

> **⚠️ ADVERTENCIA DE SEGURIDAD:** Nunca mire directamente el extremo de una fibra conectada ni limpie restos de vidrio sobre la ropa o la mesa. Los fragmentos microscópicos de sílice pueden penetrar la piel o el globo ocular.

---

## 🛠️ 3. Guía Paso a Paso: Preparación y Termofusión por Arco Eléctrico

### 🔹 Paso 1: Remoción de Chaqueta Exterior y Elementos de Tracción
1. Sujete el cable troncal de planta externa utilizando guantes de seguridad y realice un corte anular superficial en la cubierta negra de polietileno (PE) con cortacables o cuchillo retráctil.
2. Tire del **hilo de rasgado rojo (*ripcord*)** en sentido longitudinal para abrir la cubierta sin dañar los tubos internos y recorte las fibras de aramida (Kevlar) amarillas.

![Remoción de chaqueta y exposición de Kevlar](assets/img/02-remocion-chaqueta-kevlar.jpg)
![Aislamiento de tubos holgados en estación](assets/img/03-extraccion-buffer-hilos.jpg)

> **🚨 ERROR COMÚN:** Profundizar demasiado el corte inicial de la chaqueta exterior puede mellar o seccionar el tubo holgado (*buffer tube*) y quebrar los hilos internos antes de prepararlos.

---

### 🔹 Paso 2: Manguito Termo-contraíble, Stripping ($125\ \mu\text{m}$) y Limpieza
1. **Antes de pelar el recubrimiento primario**, inserte el manguito termo-contraíble (*heat shrink sleeve*) por uno de los extremos del hilo.
2. Emplee la pinza peladora (*stripper*) calibrada para retirar el acrilato de $250\ \mu\text{m}$ y dejar expuesto el **vidrio (cladding) de $125\ \mu\text{m}$** en un tramo de $30\text{ a }40\ \text{mm}$.
3. Humedezca un paño libre de pelusa (**Kimwipes**) con **alcohol isopropílico de alta pureza ($\ge 99.5\%$)** y limpie el vidrio en un solo sentido desde el recubrimiento hacia la punta.

![Fibra desnuda y paños Kimwipes](assets/img/04-limpieza-alcohol-kimwipes.jpg)

> **🚨 ERROR COMÚN:** Apoyar el hilo limpio sobre la mesa o tocarlo con los guantes contamina el vidrio con polvo o grasa, generando burbujas en el arco eléctrico y pérdidas superiores a $0.1\ \text{dB}$.

---

### 🔹 Paso 3: Corte de Precisión (Cleaving a $90^\circ$)
1. Abra la cortadora de precisión (*cleaver*) y verifique que la cuchilla de carburo de tungsteno esté retraída.
2. Coloque la fibra limpia en la canaleta guía ($250\ \mu\text{m}$ / $900\ \mu\text{m}$) dejando $10\text{ a }16\ \text{mm}$ de vidrio expuesto según la regla graduada.
3. Cierre la prensa, accione el carro de corte en un movimiento continuo y deposite el sobrante en el recipiente de desechos.

![Corte de precisión en cleaver](assets/img/05-corte-precision-cleaver.jpg)

> **⚠️ ADVERTENCIA DE CALIDAD:** Un ángulo de corte defectuoso ($> 1.5^\circ$), astillado o con rebabas provocará que la fusionadora detenga el proceso y exija repetir el pelado, limpieza y corte.

---

### 🔹 Paso 4: Alineación de Núcleos y Termofusión (Vcnex VFS-30)
1. Levante la cubierta protectora y las prensas de la fusionadora **Vcnex VFS-30**.
2. Posicione cuidadosamente ambos extremos sobre las **ranuras en V (*V-grooves*)**, ubicando las puntas entre los electrodos sin tocar las guías cerámicas.
3. Cierre las prensas y la tapa superior para ejecutar el ciclo automático en modo `SM00`: limpieza por pre-arco, medición angular, **alineación de núcleos en ejes X/Y** y descarga del arco eléctrico.

![Posicionamiento de fibras en V-grooves](assets/img/06-posicionamiento-fusionadora.jpg)
![Resultado en pantalla VFS-30: Pérdida 0.01 dB](assets/img/07-resultado-pantalla-001db.jpg)

---

### 🔹 Paso 5: Protección Mecánica con Manguito Termo-contraíble
1. Retire suavemente la fibra fusionada manteniendo leve tensión axial y deslice el manguito termo-contraíble hasta centrar la aguja de acero inoxidable sobre el punto de empalme.
2. Introduzca el conjunto en el **horno calefactor izquierdo** de la VFS-30 y presione el botón térmico (indicador LED rojo encendido) hasta completar el sellado.

![Horno termo-contraíble activo](assets/img/08-horno-termocontraible.jpg)
![Empalme finalizado con manguito curado](assets/img/09-empalme-final-protegido.jpg)

---

## 📊 4. Análisis de Resultados y Presupuesto Óptico (Enlace GPON)

Para validar la viabilidad del enlace bajo estándar **ITU-T G.984 (GPON Clase B+)**, se calcula la atenuación teórica total considerando fibra monomodo OS2 ($1310/1490\ \text{nm}$), empalmes por fusión, conectores y margen operativo.

### 🧮 4.1. Tabla de Cálculo del Presupuesto Óptico

| Componente del Enlace | Cantidad | Atenuación Unitaria Estándar | Pérdida Total ($\text{dB}$) | Referencia / Norma |
| :--- | :---: | :---: | :---: | :--- |
| 🌐 Fibra Óptica Monomodo ($1310\ \text{nm}$) | $2.5\ \text{km}$ | $0.35\ \text{dB/km}$ | $0.88\ \text{dB}$ | ITU-T G.652.D |
| ⚡ Empalmes por Termofusión | $2\ \text{unid.}$ | $0.05\ \text{dB/empalme}$ | $0.10\ \text{dB}$ | TIA-568.3-D |
| 🔌 Conectores Ópticos (SC/APC) | $2\ \text{pares}$ | $0.30\ \text{dB/par}$ | $0.60\ \text{dB}$ | TIA-568.3-D |
| 🔀 Divisor Óptico (Splitter $1:8$) | $1\ \text{unid.}$ | $10.50\ \text{dB}$ | $10.50\ \text{dB}$ | Arquitectura FTTH/GPON |
| 🛡️ Margen de Seguridad y Envejecimiento | $1\ \text{global}$ | $3.00\ \text{dB}$ | $3.00\ \text{dB}$ | Buena práctica Planta Externa |
| **🎯 ATENUACIÓN TOTAL ESTIMADA** | — | — | **$15.08\ \text{dB}$** | **✅ Cumple GPON Clase B+ ($\le 28\ \text{dB}$)** |

### 🔬 4.2. Registro de Medición y Verificación en Taller

| Parámetro Evaluado | Valor Obtenido en Taller | Umbral Máximo Permitido | Estado |
| :--- | :---: | :---: | :---: |
| ⚙️ **Perfil de Fusión Utilizado** | `SM00` (Monomodo estándar) | Compatible ITU-T G.652 | ✅ Aprobado |
| 📉 **Pérdida estimada por fusionadora** | **$0.01\ \text{dB}$** | $\le 0.05\ \text{dB}$ | 🌟 Sobresaliente |
| 🔍 **Integridad física del manguito** | Centrado, transparente y sin burbujas | Sin burbujas ni exposición | ✅ Aprobado |

> **💡 Conclusión Técnica:** La termofusión ejecutada en la **Vcnex VFS-30** obtuvo una pérdida estimada de **$0.01\ \text{dB}$** (cinco veces inferior al umbral máximo normativo de $0.05\ \text{dB}$), evidenciando un corte perpendicular limpio y una alineación de núcleos óptima. Integrado en el enlace GPON de $2.5\ \text{km}$ con splitter $1:8$ (**$15.08\ \text{dB}$** de pérdida total), el sistema mantiene un margen de seguridad superior a $12.9\ \text{dB}$ respecto al presupuesto máximo de $28\ \text{dB}$ de la Clase B+.
