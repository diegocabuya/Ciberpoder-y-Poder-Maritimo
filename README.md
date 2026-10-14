<div align="center">

# El ciberpoder como variable estructural del poder marítimo

### *Un modelo multiplicativo normalizado para la evaluación multidominio del poder marítimo*

**Diego E. Cabuya-Padilla** · **Sergio Uribe-Cáceres** · **Carlos A. Castaneda-Marroquin**

Academia Naval de Estudios Estratégicos, Armada de Colombia · Escuela Superior de Guerra «General Rafael Reyes Prieto» · Escuela Naval de Cadetes «Almirante Padilla» (NAVTEG)

*Manuscrito en revisión — IEEE Access (versión revisada, octubre de 2026)*

[![Sitio del proyecto (ES)](https://img.shields.io/badge/🌐_Sitio_del_proyecto-español-0D2A42?style=for-the-badge)](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/?lang=es)
[![Simulador (ES)](https://img.shields.io/badge/▶_Simulador-interactivo-185FA5?style=for-the-badge)](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/simulator/simulator.html?lang=es)
[![Repositorio canónico](https://img.shields.io/badge/📦_Materiales-repositorio_en_inglés-0F6E56?style=for-the-badge)](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power)

</div>

---

> **Un solo sitio, dos idiomas.** Desde octubre de 2026 el proyecto mantiene **una única página y un único simulador, bilingües (EN/ES)**, alojados en el repositorio en inglés. Este repositorio conserva la versión en español del artículo y redirige al sitio común con el idioma español activado. Los materiales de apoyo del manuscrito —script de verificación, búsqueda bibliográfica documentada, figuras— viven en el repositorio canónico:
> **https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power**

## Resumen

La formulación clásica del poder marítimo —el producto de los **intereses marítimos** y el **poder naval**— resulta insuficiente para explicar las dinámicas de los entornos marítimos digitalizados. Este artículo propone una formulación extendida que incorpora el **ciberpoder**, la **voluntad estratégica** y la **seguridad marítima** como variables estructurales del poder marítimo. El modelo adopta una estructura multiplicativa normalizada en la que el colapso de cualquier dimensión restringe el agregado, y cuyo resultado se sitúa en (0, 1], lo que permite una escala de cinco niveles directamente interpretable.

La formulación se **verifica** en tres etapas —propiedades lógico-matemáticas, análisis de sensibilidad y perfiles construidos— y un análisis de sensibilidad global identifica la seguridad marítima (su valor y su peso) como la principal fuente de incertidumbre; **la calibración y la validación externa se distinguen de la verificación y se dejan para trabajo futuro**. Colombia se emplea como caso ilustrativo: tomando su puesto en seguridad marítima del índice de poder marítimo más sistemático disponible en la literatura latinoamericana y valores ilustrativos para los demás componentes, el modelo sitúa al país en el nivel Moderado y descompone el resultado para mostrar qué componentes concentran las mayores brechas; un corolario enuncia la condición de costes relativos bajo la cual el ciberpoder sería el vector de inversión más eficiente.

## El modelo

**Nivel 1 — expresión general normalizada (Ecs. 1–3):**

```
MP_norm = [ (MI × NP) × SW × MS^γ × CP^α ]^(1/n_eff)        con  n_eff = 3 + γ + α
```

| Símbolo (artículo en inglés) | Equivalente en español | Variable | Papel |
|:------:|:------:|----------|------|
| **MI** | IM | Intereses marítimos | El fin que da sentido al poder marítimo (Ec. 4: subíndice ponderado) |
| **NP** | PN | Poder naval | El instrumento: Fuerza × Posición × MDA^μ (Ec. 5) |
| **SW** | VE | Voluntad estratégica | Multiplicador de todo el sistema: política · institucional · social (Ec. 6) |
| **MS** | SM | Seguridad marítima | Condición del entorno — incidencia de amenazas, no capacidades (Ec. 7); γ es su peso |
| **CP** | CP | Ciberpoder | Variable estructural: ciberseguridad, ciberdefensa estratégica, capacidad de recuperación, amplificada por la ciberdiplomacia (Ec. 8); α es **el peso de la dependencia cibernética**, no una medida de capacidad |

La normalización es una media geométrica ponderada con pesos ω<sub>MI</sub> = ω<sub>NP</sub> = ω<sub>SW</sub> = 1/n<sub>eff</sub>, ω<sub>MS</sub> = γ/n<sub>eff</sub>, ω<sub>CP</sub> = α/n<sub>eff</sub>. **Proposición 1:** MP<sub>norm</sub> = G<sup>1−w</sup> · CP<sup>w</sup>, donde G es la media geométrica del resto del sistema y w = α/n<sub>eff</sub>; por tanto, subir CP siempre sube el índice, mientras que subir α solo lo sube si CP > G, y el índice es estrictamente cóncavo en cada componente para cualquier α > 0. **Corolario 1:** el ciberpoder es el vector de inversión más eficiente si y solo si c<sub>k</sub>/c<sub>CP</sub> > (ω<sub>k</sub>/X<sub>k</sub>)/(ω<sub>CP</sub>/CP) para cada otro componente k — una condición comprobable sobre costes unitarios relativos, no un resultado.

Escala de interpretación: **Crítico** (0,00–0,20), **Bajo** (0,21–0,40), **Moderado** (0,41–0,60), **Significativo** (0,61–0,80), **Alto** (0,81–1,00).

## Caso de referencia: Colombia

| | MI | NP | SW | MS | CP | α | γ | MP<sub>norm</sub> |
|---|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Valor | 0,60 | 0,55 | 0,48 | **0,24** | 0,40 | 0,55 | 0,70 | **0,455** (Moderado) |

Solo **MS** procede de una fuente externa: el puesto 75 de Colombia entre 99 Estados en el índice de seguridad marítima de Vargas-Suárez et al. (2021), convertido en percentil de posición, (99 − 75)/98 ≈ 0,24. Los demás valores y los parámetros son elecciones ilustrativas de los autores, fijadas directamente en el Nivel 1. G = 0,464 > CP, así que una α mayor baja el índice (0,464 cuando α → 0; 0,450 con α = 1). Umbrales de coste del Corolario 1: 1,21 (MI), 1,32 (NP), 1,52 (SW), 2,12 (MS). El resultado es robusto a una incertidumbre moderada (±0,10) en los insumos, pero no a una grande (±0,20).

## Empieza aquí

- **[🌐 Sitio del proyecto en español](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/?lang=es)** — resumen, materiales, láminas de ecuaciones, reproducibilidad y notas de la revisión. El selector EN/ES de la cabecera cambia el idioma de toda la página.
- **[▶ Simulador interactivo en español](https://diegocabuya.github.io/Cyber_Power_and_Maritime_Power/simulator/simulator.html?lang=es)** — entradas de Nivel 1 y desagregación opcional de Nivel 2, elasticidades, retornos marginales, la condición de coste del Corolario 1, banda de incertidumbre por Monte Carlo y gráficas de comparación. Precargado con el caso colombiano y los perfiles construidos del artículo.
- **[🧪 Script de verificación](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power/blob/main/verification/verify_model.py)** — regenera todas las cifras de las secciones de verificación y del caso de estudio (Tablas 4–7, Proposición 1, Corolario 1). Solo biblioteca estándar de Python:

  ```bash
  python3 verification/verify_model.py 300000   # corrida canónica citada en el artículo (~1 min)
  ```

- **[🔎 Búsqueda bibliográfica documentada](https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power/tree/main/search)** — cadenas de búsqueda, registros crudos (OpenAlex y Scopus, 13 de octubre de 2026, 2014–2026) y el registro de cribado de los 812 registros únicos.

## Contenido de este repositorio

```
.
├── index.html                           ← Redirige al sitio bilingüe con el español activado
├── docs/
│   └── Articulo_Poder_Maritimo_y_Ciberpoder_Diego_Cabuya.pdf   ← Versión en español (7-sep-2026, anterior a la revisión)
├── archivo/2026-08_pre-revision/        ← Simulador v6, figuras, infografía y presentación anteriores a la revisión
├── LICENSE
└── README.md
```

> **Sobre la versión en español del artículo.** El PDF de `docs/` es la versión del 7 de septiembre de 2026, **anterior a la revisión de octubre**: conserva la notación IM/PN/VE/SM/CP, el valor SM = 0,59 para Colombia y las afirmaciones que el manuscrito en inglés revisado corrigió (véase la sección *Qué cambió en la revisión* del sitio). Se publicará aquí la versión actualizada cuando esté lista. Los materiales de `archivo/` se conservan solo como registro.

## Qué cambió en la revisión de octubre de 2026

| Tema | Versión enviada | Versión revisada |
|---|---|---|
| α | Índice de madurez cibernética y exponente a la vez | **Peso de la dependencia cibernética**; la madurez se lee en CP, en cinco tramos (Proposición 1) |
| Concavidad | Atribuida a α < 1 | Vale para cualquier α > 0: el exponente normalizado siempre es menor que uno, para todos los componentes |
| Eficiencia de la inversión | «El ciberpoder es el vector de inversión más eficiente» | **Retirado**; sustituido por la condición de costes del Corolario 1 |
| Colombia | SM = 0,59 (cuota porcentual), MP<sub>norm</sub> = 0,53, «misma escala» que el índice de referencia | MS = 0,24 (percentil de posición), MP<sub>norm</sub> = 0,455; sin escala común, sin calibración, sin validación |
| Verificación | «Validación» | Verificación, calibración y validación externa distinguidas (Sargent, 2011); análisis de incertidumbre con índices de Sobol'; protocolo de calibración y validación externa; tabla de operacionalización |
| Componentes | Ciberresiliencia (CR<sub>m</sub>); ciberdiplomacia en CP y en la voluntad política; Σβ = 0,90 en el simulador | **Capacidad de recuperación marítima (RC<sub>m</sub>)**; ciberdiplomacia solo en CP; fronteras operacionales explícitas; Σβ = 1 |
| Literatura | Búsqueda sin registro | Búsqueda documentada en OpenAlex y Scopus; se discuten las medidas compuestas existentes (todas aditivas, ninguna con ciberpoder) |

## Cómo citar

> Cabuya-Padilla, D. E., Uribe-Cáceres, S. y Castaneda-Marroquin, C. A. (2026). *Cyber power as a structural variable of maritime power: A normalized multiplicative model for multidomain assessment of maritime power* [El ciberpoder como variable estructural del poder marítimo: un modelo multiplicativo normalizado para la evaluación multidominio del poder marítimo]. Manuscrito en revisión, IEEE Access. Materiales de apoyo: https://github.com/diegocabuya/Cyber_Power_and_Maritime_Power

## Licencia

Los **materiales de investigación** se comparten bajo licencia [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es) y el **código** bajo licencia [MIT](https://opensource.org/licenses/MIT), según el archivo [`LICENSE`](LICENSE). Los materiales del repositorio en inglés se publican bajo CC BY 4.0.

---

<div align="center">

**Academia Naval de Estudios Estratégicos** · Armada de Colombia · Bogotá · 2026

</div>
