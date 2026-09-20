# ElBus_palmira v2

Sistema de gestión de estructura institucional para la campaña electoral de Palmira 2026.

## Producción

- **URL**: https://mrmtech.net/ElBus_palmira/
- **Servidor**: Hostinger srv690 (`us-imm-web690.main-hosting.eu`)
- **Ruta remota**: `domains/mrmtech.net/public_html/ElBus_palmira/`
- **Repositorio**: https://github.com/vicktore-zable/ElBus_palmira

## Características

- **Organigrama interactivo** con 43 nodos LNR + 28 subdependencias
- **Nombres reales 2026** de responsables y gerentes descentralizados
- **Tracking de cambios**: nombre actual tachado en rojo + nuevo nombre en verde
- **10 vacantes documentadas** con borde rojo y badge
- **8 vistas temáticas**: General, Despacho del Alcalde, Social, Desarrollo, Económico, Infraestructura, Constitucional, Descentralizados + Vacantes
- **Colores por eje temático** para identificación visual rápida
- **Drag & Drop** para reorganizar nodos
- **Reacomodar**: layout jerárquico automático inteligente
- **Edición de plazas**: asignar persona, padrino político, estado y notas
- **Persistencia local** vía localStorage
- **Exportación a Excel** con trazabilidad (responsable actual, vacantes, certeza, fuente)

## Uso

1. Abrir `index.html` en el navegador (o la URL de producción)
2. Navegar entre ejes temáticos desde la barra lateral
3. Click en un nodo LNR para asignar/editar plaza
4. Arrastrar nodos o usar "Reacomodar" para reorganizar
5. Exportar a Excel cuando sea necesario

## Estructura

```
ElBus_palmira/
├── index.html                              ← App principal (autocontenida)
├── data/
│   ├── estructura_lnr_v2.json              ← Datos LNR v2 (43 nodos + subdependencias)
│   ├── estructura_descentralizados_v2.json ← Entidades con gerentes 2026
│   ├── estructura_lnr.json                 ← Datos v1 (referencia)
│   └── estructura_descentralizados.json    ← Datos v1 (referencia)
└── README.md
```

## Colores Temáticos

| Eje | Color |
|-----|-------|
| Alcalde (Electivo) | Verde |
| Despacho del Alcalde | Rosa / Magenta |
| Eje Social | Púrpura |
| Eje Desarrollo | Azul |
| Eje Económico | Naranja |
| Infraestructura | Amarillo |
| Eje Constitucional | Rojo |
| Descentralizados | Teal |

## Despliegue

Los archivos se publican por SSH/SFTP al servidor Hostinger:

```
Servidor: 212.1.208.241:65002
Usuario:  u156469157
Ruta:     domains/mrmtech.net/public_html/ElBus_palmira/
```

> El `public_html` raíz del usuario es un symlink a `domains/igt.net.co/public_html`.
> Para este proyecto la publicación correcta es bajo `domains/mrmtech.net/public_html/`.

## Tecnologías

- HTML5 / CSS3 / Vanilla JavaScript
- SVG para renderizado de organigramas
- SheetJS (CDN) para exportación Excel
- localStorage para persistencia

## Licencia

Uso interno - Campaña electoral Palmira 2026
