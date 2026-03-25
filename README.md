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

Gestor de dependencias
- **Archivo**: `requirements.txt` — Lista de dependencias del proyecto.
- **Script gestor**: `scripts/manage_deps.py` — Pequeño gestor que usa `pip` para instalar, desinstalar y sincronizar dependencias.

Ejemplos de uso

```bash
# Instalar un paquete y actualizar requirements.txt
python scripts/manage_deps.py install fastapi --sync

# Desinstalar un paquete y actualizar requirements.txt
python scripts/manage_deps.py uninstall fastapi --sync

# Generar/actualizar requirements.txt desde el entorno actual
python scripts/manage_deps.py freeze

# Instalar desde requirements.txt
python scripts/manage_deps.py install-file

# Ver paquetes instalados
python scripts/manage_deps.py list
```