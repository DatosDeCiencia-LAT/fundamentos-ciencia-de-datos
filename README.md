# Datos de Ciencia — Fundamentos de Data Science/ML

Series progresivas de notebooks sobre fundamentos de Data Science, Machine Learning e Ingeniería de ML, usando datasets científicos reales como punto de partida.

Cada bloque cubre un dominio científico distinto (calidad del aire, epidemiología, etc.) y demuestra que los mismos problemas que resuelven investigadores en ciencia son los que la industria paga por resolver: detección en bajo SNR, inferencia en datos escasos e irregulares, reproducibilidad y escalabilidad.

## Estructura del repositorio

```
datos-de-ciencia-fundamentos/
├── README.md
├── pyproject.toml
├── bloque-1-python-basico/
│   ├── 01_fundamentos_python.ipynb
│   ├── 02_numpy_arrays.ipynb
│   ├── 03_pandas_limpieza.ipynb
│   └── 04_visualizacion.ipynb
├── bloque-2-estadistica-probabilidad/
│   ├── 05_eda_descriptiva.ipynb
│   ├── 06_probabilidad_bayes.ipynb
│   ├── 07_hipotesis_tests.ipynb
│   └── 08_correlacion_causalidad.ipynb
└── bloque-3-ml-supervisado/
    └── (próximamente)
```

## Requisitos previos

Necesitas tener Python 3.9+ instalado. Aquí hay tutoriales para configurar tu ambiente:

- [Cómo instalar Conda (Miniconda)](https://youtu.be/TJor7z8g8FA?si=7-VUSQJiew6Hu_gW)
- [VS Code + Jupyter Notebooks](https://youtu.be/rL1usXq4bgE?si=2b5REnUzVBMDxWfF)
- [Instalación de UV](https://youtu.be/YzOLOlH1jQk?si=2hFk6aAh8gCoMvuo)

## Configuración del ambiente

### Opción 1: Con UV (recomendado para proyectos Python puro)

```bash
# Clonar el repositorio
git clone https://github.com/DatosDeCiencia-LAT/datos-de-ciencia-fundamentos.git
cd datos-de-ciencia-fundamentos

# Crear el ambiente
uv sync

# Activar el ambiente
source .venv/bin/activate  # En Linux/Mac
# o
.venv\Scripts\activate  # En Windows
```

### Opción 2: Con Conda

```bash
# Clonar el repositorio
git clone https://github.com/DatosDeCiencia-LAT/datos-de-ciencia-fundamentos.git
cd datos-de-ciencia-fundamentos

# Crear el ambiente desde pyproject.toml
conda create -n datos-de-ciencia python=3.9
conda activate datos-de-ciencia

# Instalar dependencias
pip install -e .
```

## Dependencias agnósticas

Este proyecto usa `pyproject.toml` (estándar PEP 621) en lugar de `requirements.txt` para manejar dependencias. Esto significa que **funciona con conda, uv, pip o Poetry** sin cambios de configuración.

Ventajas:
- **Reproducibilidad:** Colaboradores con distintas herramientas necesitan el mismo ambiente
- **Agnósticidad:** Migrar de conda a uv (o viceversa) sin reescribir nada
- **Estándar moderno:** Compatible con el ecosistema Python actual (2025+)

## Usar los notebooks

### En VS Code

1. Abre VS Code
2. Abre la carpeta del repositorio
3. Selecciona el kernel del proyecto en la esquina superior derecha del notebook
4. Ejecuta las celdas

### En Jupyter desde terminal

```bash
jupyter notebook
```

Luego navega a la carpeta del proyecto y abre el notebook deseado.

## Estructura de los notebooks

Cada notebook sigue este formato:

1. **Header:** Título, autor, descripción y dataset
2. **Sección 0:** Prerrequisitos y setup
3. **Secciones temáticas:** Explicación + código + ejemplos
4. **Prompts de profundización:** Preguntas opcionales para explorar más allá del contenido (cópiables a tu IA de confianza)

## Público objetivo

1. **Investigadores en ciencia** interesados en herramientas de ML/AI
2. **Personas aprendiendo Data Science/ML** para entrar o avanzar en industria
3. **Desarrolladores** que quieren entender cómo los científicos resuelven problemas de datos

## Contenido disponible

### Bloque 1 — Fundamentos de Python y manejo de datos
Dominio: Calidad del aire (OpenAQ)

- `01_fundamentos_python.ipynb` — Tipos de datos, variables, control de flujo, loops, funciones y librerías

### Bloque 2 — Estadística y Probabilidad (próximamente)
Dominio: Vigilancia epidemiológica

### Bloque 3 — Machine Learning Supervisado (próximamente)

## Citar este trabajo

Si usas estos notebooks en tu trabajo o investigación, por favor cita:

```
Agudelo Ortiz, J. E. (2026). Datos de Ciencia — Fundamentos de Data Science/ML.
GitHub: https://github.com/DatosDeCiencia-LAT/datos-de-ciencia-fundamentos
```

## Licencia

Este proyecto está bajo licencia [Creative Commons Attribution 4.0 International](LICENSE).

## Contacto y redes

- **YouTube:** [@Datos.DeCiencia](https://www.youtube.com/@Datos.DeCiencia)
- **GitHub:** [DatosDeCiencia-LAT](https://github.com/DatosDeCiencia-LAT)
- **LinkedIn:** [Juan Esteban Agudelo Ortiz](https://linkedin.com/in/juanessao)
- **Instagram:** [@datos.deciencia](https://instagram.com/datos.deciencia)

## Contribuciones

Las contribuciones son bienvenidas. Si encuentras errores, tienes sugerencias o quieres mejorar el contenido, abre un issue o un pull request.

---

*Última actualización: julio 2026*