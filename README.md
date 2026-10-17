<div align="center">

# El ciberpoder como variable estructural del poder marítimo

### *Un modelo multiplicativo normalizado para la evaluación multidominio del poder marítimo*

**Diego E. Cabuya-Padilla** · **Sergio Uribe-Cáceres** · **Carlos A. Castaneda-Marroquin**

Academia Naval de Estudios Estratégicos, Armada de Colombia · Escuela Superior de Guerra «General Rafael Reyes Prieto» · Escuela Naval de Cadetes «Almirante Padilla» (NAVTEG)

*Versión en español del artículo · Versión en inglés en revisión en IEEE Access*

[![Sitio del proyecto (ES)](https://img.shields.io/badge/🌐_Sitio_del_proyecto-español-0D2A42?style=for-the-badge)](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/?lang=es)
[![Simulador (ES)](https://img.shields.io/badge/▶_Simulador-interactivo-185FA5?style=for-the-badge)](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/simulator/simulator.html?lang=es)
[![Repositorio en inglés](https://img.shields.io/badge/📦_Materiales-repositorio_en_inglés-0F6E56?style=for-the-badge)](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power)

</div>

---

> **Un solo sitio, dos idiomas.** El proyecto mantiene **una única página y un único simulador, bilingües (EN/ES)**, alojados en el repositorio en inglés. Su vista en español usa las siglas de este artículo (PM, IM, PN, VE, SM, CP). Este repositorio conserva el **artículo en español** y sus **materiales en español**, y su página redirige al sitio común con el español activado. El script de verificación y la búsqueda bibliográfica documentada viven en el repositorio en inglés.

## Resumen

La formulación clásica del poder marítimo —el producto de los intereses marítimos y el poder naval— resulta insuficiente para explicar las dinámicas de los entornos marítimos digitalizados, cuyas funciones de navegación, comunicaciones, puertos y vigilancia dependen de infraestructuras digitales interconectadas. A partir de una teoría del poder en la que el poder naval es la expresión del poder militar en el mar y el poder marítimo lo combina con intereses económicos, sociales y políticos, el artículo sostiene que el ciberpoder atraviesa ambos componentes y que, a diferencia del poder naval, no decae con la distancia. Propone una formulación ampliada que incorpora el ciberpoder, la voluntad estratégica y la seguridad marítima como variables estructurales, con una estructura multiplicativa normalizada en la que el colapso de cualquier dimensión restringe el agregado y cuyo resultado se interpreta en una escala de cinco niveles. La formulación se verifica en sus propiedades matemáticas, su sensibilidad y su robustez ante la incertidumbre; la calibración y la validación externa se distinguen de la verificación y se dejan como agenda. Colombia se emplea como caso ilustrativo: el modelo la sitúa en el nivel Moderado y muestra qué componentes concentran las mayores brechas, mientras que su política oceánica nacional, que enmarca los planes de desarrollo, no contempla la dimensión cibernética. Se concluye proponiendo un Índice de Poder Marítimo Nacional, acompañado de un simulador interactivo de acceso abierto.

## Marco teórico

El poder es la capacidad de afectar a otros para obtener los resultados que se desean (Nye, 2010). El poder nacional se ejerce mediante cuatro instrumentos: diplomático, informativo, militar y económico (OTAN, 2023). El **poder naval** es la expresión del poder militar en el mar, cuyas funciones Booth (1977/2014) concibe como una trinidad —militar, diplomática y policial— unificada por el uso del mar. El **poder marítimo** es más amplio: la capacidad de crear, desarrollar, explotar y defender los intereses marítimos de un país (CCO, 2018), de modo que combina el poder naval con intereses de naturaleza económica, social y política. El **ciberpoder** obtiene resultados dentro y fuera del ciberespacio (Nye, 2010) y por eso atraviesa ambos componentes; a diferencia del poder naval, cuya eficacia decae con la distancia (el gradiente de pérdida de poder de Booth), actúa con alcance global instantáneo (OTAN, 2025). Por eso entra en el modelo como un factor de todo el sistema.

En Colombia, la Política Nacional del Océano y de los Espacios Costeros (PNOEC), política de Estado que enmarca los planes de desarrollo nacional y sectoriales, apunta a una Potencia Media Oceánica y asocia esa meta a la posición, la voluntad política y los intereses marítimos; el Plan de Desarrollo Naval 2042 protege esos intereses mediante el poder naval. Ni la política ni los documentos que definen los dieciocho intereses marítimos mencionan la dimensión cibernética.

## El modelo

**Nivel 1 — expresión general normalizada (Ecs. 1, 1b y 1c):**

```
PM_norm = [ (IM × PN) × VE × SM^γ × CP^α ]^(1/n_eff)        con  n_eff = 3 + γ + α
```

| Sigla | Variable | Papel | Ec. | En inglés |
|:-----:|----------|-------|:---:|:---------:|
| **IM** | Intereses marítimos | El propósito del poder marítimo: subíndice ponderado | 2 | MI |
| **PN** | Poder naval | El instrumento: Fuerza × Posición × MDA^μ | 3 | NP |
| **VE** | Voluntad estratégica | Multiplicador de todo el sistema: política · institucional · social | 4 | SW |
| **SM** | Seguridad marítima | Condición del entorno: incidencia de amenazas, no capacidades; γ es su peso | 5 | MS |
| **CP** | Ciberpoder | Ciberseguridad (CS_m), ciberdefensa estratégica (CD_m) y capacidad de recuperación (CR_m), amplificadas por la ciberdiplomacia (CDb); α es **el peso de la dependencia cibernética**, no una medida de capacidad | 6 | CP |

La normalización es una media geométrica ponderada con pesos ω<sub>IM</sub> = ω<sub>PN</sub> = ω<sub>VE</sub> = 1/n<sub>eff</sub>, ω<sub>SM</sub> = γ/n<sub>eff</sub>, ω<sub>CP</sub> = α/n<sub>eff</sub>. **Proposición 1:** PM<sub>norm</sub> = G<sup>1−w</sup> · CP<sup>w</sup>, con G la media geométrica del resto del sistema y w = α/n<sub>eff</sub>; subir CP siempre sube el índice, mientras que subir α solo lo sube si CP > G, y el índice es estrictamente cóncavo en cada componente para todo α > 0. **Corolario 1:** el ciberpoder es el vector de inversión más eficiente si y solo si c<sub>k</sub>/c<sub>CP</sub> > (ω<sub>k</sub>/X<sub>k</sub>)/(ω<sub>CP</sub>/CP) para cada otro componente k: una condición comprobable sobre costes unitarios relativos, no un resultado.

Escala de interpretación: **Crítico** (0,00–0,20), **Bajo** (0,21–0,40), **Moderado** (0,41–0,60), **Significativo** (0,61–0,80), **Alto** (0,81–1,00).

## Caso ilustrativo: Colombia

| | IM | PN | VE | SM | CP | α | γ | PM<sub>norm</sub> |
|---|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Valor | 0,60 | 0,55 | 0,48 | **0,24** | 0,40 | 0,55 | 0,70 | **0,455** (Moderado) |

Solo **SM** procede de una fuente externa: el puesto 75 de Colombia entre 99 Estados en el índice de seguridad marítima de Vargas-Suárez et al. (2021), convertido en percentil de posición, (99 − 75)/98 ≈ 0,24. Los demás valores y los parámetros son elecciones ilustrativas de los autores, fijadas directamente en el Nivel 1. G = 0,464 > CP, así que una α mayor baja el índice (0,464 cuando α → 0; 0,450 con α = 1). Umbrales de coste del Corolario 1: 1,21 (IM), 1,32 (PN), 1,52 (VE), 2,12 (SM). El resultado es robusto a una incertidumbre moderada (±0,10) en los insumos, pero no a una grande (±0,20).

## Empieza aquí

- **[📄 Artículo en español (PDF)](docs/Articulo_Poder_Maritimo_y_Ciberpoder.pdf)** · [`.docx`](docs/Articulo_Poder_Maritimo_y_Ciberpoder.docx) — formato de la Revista Maris et Belli.
- **[🌐 Sitio del proyecto en español](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/?lang=es)** — resumen, marco teórico, materiales, láminas de ecuaciones y reproducibilidad.
- **[▶ Simulador interactivo en español](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/simulator/simulator.html?lang=es)** — entradas de Nivel 1 y desagregación opcional de Nivel 2, elasticidades, retornos marginales, la condición de coste del Corolario 1, banda de incertidumbre por Monte Carlo y gráficas de comparación.
- **[🎞️ Presentación](presentacion/Presentacion_PM_Ciberpoder.pdf)** — 24 diapositivas estructuradas para una sustentación académica: problema, objetivo general y objetivos específicos, marco teórico, método, resultados, discusión y conclusiones. También la **[guía del simulador](presentacion/Diapositivas_Simulador_PM.pdf)** (3 diapositivas) y la **[infografía](infografia/Infografia_PM_Ciberpoder.pdf)**.
- **[🧪 Script de verificación](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power/blob/main/verification/verify_model.py)** — regenera las cifras de las Tablas 4 a 7, la Proposición 1 y el Corolario 1. Solo biblioteca estándar de Python:

  ```bash
  python3 verification/verify_model.py 300000
  ```

- **[🔎 Búsqueda bibliográfica documentada](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power/tree/main/search)** — cadenas de búsqueda, registros recuperados (completos de OpenAlex, identificadores de Scopus; 13 de octubre de 2026, 2014–2026) y el registro de cribado de los 812 registros únicos.

## Contenido de este repositorio

```
.
├── index.html                           ← Redirige al sitio bilingüe con el español activado
├── docs/
│   └── Articulo_Poder_Maritimo_y_Ciberpoder.{pdf,docx}   ← Artículo en español (formato Maris et Belli)
├── figuras/
│   ├── ecuaciones/                      ← Las 8 láminas de ecuaciones, con las siglas en español (PDF + PNG)
│   └── esquemas/                        ← Arquitectura de dos niveles (Figura 2) y síntesis bibliográfica (Tabla 8)
├── presentacion/
│   ├── Presentacion_PM_Ciberpoder.pdf   ← 24 diapositivas para la sustentación
│   └── Diapositivas_Simulador_PM.pdf    ← 3 diapositivas: arquitectura, 31 controles y uso del simulador
├── infografia/
│   └── Infografia_PM_Ciberpoder.{pdf,png}  ← El modelo en una página
├── archivo/                            ← Versiones anteriores de los materiales, conservadas como registro
├── LICENSE
└── README.md
```

## Cómo citar

> Cabuya-Padilla, D. E., Uribe-Cáceres, S. y Castaneda-Marroquin, C. A. (2026). *El ciberpoder como variable estructural del poder marítimo: un modelo multiplicativo normalizado para la evaluación multidominio del poder marítimo* [Manuscrito]. Versión en inglés en revisión en *IEEE Access*. Materiales de apoyo: https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power

## Licencia

Los **materiales de investigación** (artículos, figuras, láminas de ecuaciones, infografía, presentaciones, y las consultas y registros de cribado de los autores) se comparten bajo licencia [**Creative Commons Atribución 4.0 Internacional (CC BY 4.0)**](https://creativecommons.org/licenses/by/4.0/deed.es), la misma con la que IEEE Access publica sus artículos: pueden compartirse y adaptarse con cualquier fin, citando la autoría. El **código** (simulador, sitio y scripts de verificación y de búsqueda) se comparte bajo licencia [**MIT**](https://opensource.org/licenses/MIT). Los registros bibliográficos de terceros del directorio `search/` del repositorio en inglés no están cubiertos: los datos de OpenAlex son CC0 y los de Scopus, publicados solo como identificadores, siguen sujetos a las condiciones de uso de Elsevier. Ver [`LICENSE`](LICENSE). Los dos repositorios usan las mismas licencias.

---

<div align="center">

**Academia Naval de Estudios Estratégicos** · Armada de Colombia · Bogotá · 2026

</div>
