# 🛡️ RECRIPEI-CR: Modelo de Ciberresiliencia para PyMEs

**Autora:** Saray Blanco Alzola  
**Empresa:** DCS Consulting (@dcs_consulting) 

---

## ¿Qué es RECRIPEI-CR?

El **Modelo RECRIPEI-CR** (RECRIPEI Cyber Resilience) es un modelo estratégico de ciberresiliencia para pequeñas y medianas empresas (PyMEs) que fusiona:

- **RECRIPEI** (Blanco, 2018): modelo de seguridad física concéntrica desarrollado originalmente para la Siderúrgica del Orinoco "Alfredo Maneiro" (SIDOR), Venezuela.
- **Modelo de Madurez de Druva** (2025): cinco niveles de madurez para la protección y recuperación de datos en entornos de nube.

Alineado con el marco normativo europeo: **NIS2**, **RGPD**, **LOPDGDD** y el **Código Penal español** (arts. 197 bis, 264, 264 quater, 31 bis).

---

## Estructura del repositorio

```
recripei-cr/
├── RECRIPEI_CR_Analysis.ipynb    # Notebook principal de análisis
├── cybersecurity_incidents.csv   # Base de datos de incidentes (fuentes oficiales)
├── output/                       # Gráficos generados
│   ├── 01_tendencias_espana.png
│   ├── 02_sistemas_vulnerables.png
│   ├── 03_comparativa_global.png
│   └── 04_nivel_recripei_cr.png
└── README.md
```

---

## Los 5 niveles del modelo RECRIPEI-CR

| Nivel | Área RECRIPEI | Nombre digital | Normativa |
|---|---|---|---|
| 1 | Área Restringida | Inmutabilidad de datos | Art. 32 RGPD |
| 2 | Área Crítica | Seguridad en las copias | Art. 21 NIS2 |
| 3 | Área Protegida | Remediación cibernética | Art. 33 RGPD |
| 4 | Área de Exclusión | Investigación cibernética | Art. 264 CP |
| 5 | Área de Influencia | Detección mejorada | Art. 31 bis CP |

---

## Cómo usar la calculadora

```python
from RECRIPEI_CR_Analysis import calcular_nivel_recripei_cr

mi_empresa = {
    'tiene_backup_inmutable': True,
    'backup_aislado': True,
    'tiene_mfa': True,
    'tiene_cifrado': False,
    'tiene_sandbox': False,
    'verifica_backups': False,
    'tiene_logs': False,
    'analisis_forense': False,
    'monitoreo_continuo': False,
    'coordina_incibe': False
}

resultado = calcular_nivel_recripei_cr(mi_empresa)
print(resultado)
```

---

## Fuentes de datos oficiales

| Fuente | Región | Datos |
|---|---|---|
| INCIBE (2022-2025) | España | Balances anuales de ciberseguridad |
| ENISA Threat Landscape 2025 | UE | 4.875 incidentes analizados |
| FBI IC3 Annual Report 2024 | EE.UU. | 880.418 denuncias |
| INTERPOL Cybercrime Report 2024 | Global | Asia-Pacífico y África |

---

## Pendiente (v2.0 — DCS Consulting)

- [ ] Dashboard interactivo con Plotly
- [ ] Datos Asia-Pacífico y África verificados
- [ ] Análisis específico de ataques en entornos cloud
- [ ] Generador de informe PDF con marca DCS Consulting
- [ ] API REST para integración con herramientas de clientes

---

## Cita académica

> Blanco Alzola, S. (2026). *Ciberresiliencia en PyMEs: modelo estratégico para la protección y recuperación de datos en entornos de nube*. Trabajo de Fin de Máster, Máster Universitario en Ciberdelincuencia, UNIR.



