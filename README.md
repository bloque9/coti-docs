# Documentación de [COTI](https://coti.mx/)

La documentación utiliza [mkdocs-material](https://squidfunk.github.io/mkdocs-material/getting-started/) y se actualiza cada que se actualiza el repo.

## Instalación

```bash
pip install mkdocs-material
```

## Uso

```bash
# Start the live-reloading docs server.
mkdocs serve
```

## Agregar página
Para agregar una pagina nueva solo tienes que agregar un archivo de markdown en el directorio `source`, utilizar el formato `nuevo-documento.md`
```
├── mkdocs.yml
└── source
    ├── CNAME
    ├── index.md
    ├── nuevo-documento.md
    └── primeros-pasos.md
```
Después de agregar el archivo, tienes que agregar la pagina al menú, en el archivo `mkdocs.yml`, para esto tines que agregar en la parte de nav: un texto con el formato `- Titulo: nuevo-documento.md`, tienes que cuidar la indentación
```yaml
nav:
  - Inicio:
    - Welcome: index.md
  - Primeros Pasos: primeros-pasos.md
  - Nuevo documento: nuevo-documento.md
```
Puedes ver los resultados ejecutando el comando `mkdocs serve`


## Contributing
At the moment we do not accept pull requests.
