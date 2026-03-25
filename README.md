# Parcial Práctico — Entornos de Desarrollo de Software

Resumen
- Proyecto de apoyo para el parcial práctico de Entornos de Desarrollo de Software.
- Contiene un script principal `main.py` y un entorno virtual local en `enotorno_virtual/`.

Requisitos
- Linux (probado en Ubuntu/Debian)
- Python 3.12

Instalación y configuración
1. Activar el entorno virtual incluido:

```bash
source enotorno_virtual/bin/activate
```

2. (Opcional) Si necesita instalar dependencias en otro entorno, crear uno nuevo y usar `requirements.txt` si existe:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Uso
- Ejecutar el script principal:

```bash
python main.py
```

- Si el proyecto usa variables de entorno, revise el archivo `.env` en la raíz y ajuste según corresponda.

Estructura del proyecto
- `main.py` — Punto de entrada del proyecto.
- `enotorno_virtual/` — Entorno virtual incluido (no es necesario recrearlo si ya está configurado).
- `.env` — Archivo con variables de entorno (si aplica).

Documentación adicional
- Ver `docs/USAGE.md` para instrucciones de uso y ejemplos.

Contribuir
- Hacer fork y abrir un pull request con cambios claros.

Contacto
- Autor / Responsable del repositorio: revisa los comentarios del código o contáctame para más detalles.

Licencia
- Añadir aquí la licencia del proyecto si aplica (por ejemplo, MIT).