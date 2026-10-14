<div align="center">

# El ciberpoder como variable estructural del poder marítimo

### *Un modelo multiplicativo normalizado para la evaluación multidominio del poder marítimo*

**Diego E. Cabuya-Padilla** · **Sergio Uribe-Cáceres** · **Carlos A. Castaneda-Marroquin**

Academia Naval de Estudios Estratégicos, Armada de Colombia · Escuela Superior de Guerra «General Rafael Reyes Prieto» · Escuela Naval de Cadetes «Almirante Padilla» (NAVTEG)

*Versión en español del artículo, revisada en octubre de 2026 · Versión en inglés en revisión en IEEE Access*

[![Sitio del proyecto (ES)](https://img.shields.io/badge/🌐_Sitio_del_proyecto-español-0D2A42?style=for-the-badge)](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/?lang=es)
[![Simulador (ES)](https://img.shields.io/badge/▶_Simulador-interactivo-185FA5?style=for-the-badge)](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/simulator/simulator.html?lang=es)
[![Repositorio en inglés](https://img.shields.io/badge/📦_Materiales-repositorio_en_inglés-0F6E56?style=for-the-badge)](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power)

</div>

---

> **Un solo sitio, dos idiomas.** El proyecto mantiene **una única página y un único simulador, bilingües (EN/ES)**, alojados en el repositorio en inglés. Su vista en español usa las siglas de este artículo (PM, IM, PN, VE, SM, CP). Este repositorio conserva el **artículo en español** y sus **materiales en español**, y su página redirige al sitio común con el español activado. El script de verificación y la búsqueda bibliográfica documentada viven en el repositorio en inglés.

## Resumen

La formulación clásica del poder marítimo —el producto de los intereses marítimos y el poder naval— resulta insuficiente para explicar las dinámicas de los entornos marítimos digitalizados. Este artículo propone una formulación ampliada que incorpora el ciberpoder, la voluntad estratégica y la seguridad marítima como variables estructurales, con una estructura multiplicativa normalizada en la que el colapso de cualquier dimensión restringe el agregado y cuyo resultado se interpreta en una escala de cinco niveles. La formulación se verifica en sus propiedades matemáticas, su sensibilidad y su robustez ante la incertidumbre; la calibración y la validación externa se distinguen de la verificación y se dejan como agenda. Colombia se emplea como caso ilustrativo: el modelo la sitúa en el nivel moderado y muestra qué componentes concentran las mayores brechas. Se concluye proponiendo un índice nacional de poder marítimo, acompañado de un simulador interactivo de acceso abierto.

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

- **[📄 Artículo en español, versión revisada (PDF)](docs/Articulo_Poder_Maritimo_y_Ciberpoder_v2_revisado_2026-10.pdf)** · [`.docx`](docs/Articulo_Poder_Maritimo_y_Ciberpoder_v2_revisado_2026-10.docx) — formato de la Revista Maris et Belli, con los cambios de la revisión de octubre de 2026.
- **[🌐 Sitio del proyecto en español](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/?lang=es)** — resumen, materiales, láminas de ecuaciones, reproducibilidad y notas de la revisión.
- **[▶ Simulador interactivo en español](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/simulator/simulator.html?lang=es)** — entradas de Nivel 1 y desagregación opcional de Nivel 2, elasticidades, retornos marginales, la condición de coste del Corolario 1, banda de incertidumbre por Monte Carlo y gráficas de comparación.
- **[🎞️ Presentación](presentacion/Presentacion_PM_Ciberpoder.pdf)** (18 diapositivas), **[guía del simulador](presentacion/Diapositivas_Simulador_PM.pdf)** (3 diapositivas) e **[infografía](infografia/Infografia_PM_Ciberpoder.pdf)**, regeneradas con la versión revisada.
- **[🧪 Script de verificación](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power/blob/main/verification/verify_model.py)** — regenera las cifras de las Tablas 4 a 7, la Proposición 1 y el Corolario 1. Solo biblioteca estándar de Python:

  ```bash
  python3 verification/verify_model.py 300000
  ```

- **[🔎 Búsqueda bibliográfica documentada](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power/tree/main/search)** — cadenas de búsqueda, registros crudos (OpenAlex y Scopus, 13 de octubre de 2026, 2014–2026) y el registro de cribado de los 812 registros únicos.

## Contenido de este repositorio

```
.
├── index.html                           ← Redirige al sitio bilingüe con el español activado
├── docs/
│   └── Articulo_..._v2_revisado_2026-10.{pdf,docx}   ← Artículo en español, versión revisada (octubre de 2026)
├── figuras/
│   ├── ecuaciones/                      ← Las 8 láminas de ecuaciones, con las siglas en español (PDF + PNG)
│   └── esquemas/                        ← Arquitectura de dos niveles (Figura 2) y síntesis bibliográfica (Tabla 8)
├── presentacion/
│   ├── Presentacion_PM_Ciberpoder.pdf   ← 18 diapositivas sobre el modelo revisado
│   └── Diapositivas_Simulador_PM.pdf    ← 3 diapositivas: arquitectura, 31 controles y uso del simulador
├── infografia/
│   └── Infografia_PM_Ciberpoder.{pdf,png}  ← El modelo revisado en una página
├── archivo/2026-08_pre-revision/        ← Versiones de agosto y septiembre (simulador v6, figuras, infografía, presentación, artículo)
├── LICENSE
└── README.md
```

> **Sobre el archivo.** Los materiales de `archivo/` son anteriores a la revisión: conservan el valor SM = 0,59 para Colombia y afirmaciones que la revisión corrigió (véase la tabla siguiente). Se mantienen solo como registro.

## Qué cambió en la revisión de octubre de 2026

| Tema | Versión anterior | Versión revisada |
|---|---|---|
| α | Índice de madurez cibernética y exponente a la vez | **Peso de la dependencia cibernética**; la madurez se lee en CP, en cinco tramos (Proposición 1) |
| Concavidad | Atribuida a α < 1 | Vale para cualquier α > 0: el exponente normalizado siempre es menor que uno, para todos los componentes |
| Eficiencia de la inversión | «El ciberpoder es el vector de inversión más eficiente» | **Retirado**; sustituido por la condición de costes del Corolario 1 |
| Colombia | SM = 0,59 (cuota porcentual), PM<sub>norm</sub> = 0,53, «misma escala» que el índice de referencia | SM = 0,24 (percentil de posición), PM<sub>norm</sub> = 0,455; sin escala común, sin calibración, sin validación |
| Verificación | «Validación» | Verificación, calibración y validación externa distinguidas (Sargent, 2011); análisis de incertidumbre con índices de Sobol; protocolo de calibración y validación externa; tabla de operacionalización |
| Componentes | Ciberresiliencia; ciberdiplomacia en CP y en la voluntad política; Σβ = 0,90 en el simulador | **Capacidad de recuperación marítima (CR<sub>m</sub>)**; ciberdiplomacia solo en CP; fronteras operacionales explícitas (Tabla 2); Σβ = 1 |
| Literatura | Búsqueda sin registro | Búsqueda documentada en OpenAlex y Scopus; se discuten las medidas compuestas existentes (todas aditivas, ninguna con ciberpoder) |

## Cómo citar

> Cabuya-Padilla, D. E., Uribe-Cáceres, S. y Castaneda-Marroquin, C. A. (2026). *El ciberpoder como variable estructural del poder marítimo: un modelo multiplicativo normalizado para la evaluación multidominio del poder marítimo* [Manuscrito]. Versión en inglés en revisión en *IEEE Access*. Materiales de apoyo: https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power

## Licencia

Los **materiales de investigación** se comparten bajo licencia [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es) y el **código** bajo licencia [MIT](https://opensource.org/licenses/MIT), según el archivo [`LICENSE`](LICENSE). Los materiales del repositorio en inglés se publican bajo CC BY 4.0.

---

<div align="center">

**Academia Naval de Estudios Estratégicos** · Armada de Colombia · Bogotá · 2026

</div>
