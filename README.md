# ElBus_palmira

Sistema de gestión de estructura institucional para la campaña electoral de Palmira 2026.

## Características

- **Organigrama interactivo** con 42 plazas LNR de la Administración Central
- **7 vistas temáticas**: General, Social, Desarrollo, Económico, Infraestructura, Constitucional, Descentralizados
- **Colores por eje temático** para identificación visual rápida
- **Drag & Drop** para reorganizar nodos con reestructuración inteligente
- **Edición de plazas**: Asignar persona, padrino político, estado y notas
- **Persistencia local** via localStorage
- **Exportación a Excel** con toda la información
- **6 entidades descentralizadas**: IMDER, IMDESEPAL, Hospital HROB, CDAP, CORFEPALMIRA, Aguas de Palmira

## Uso

1. Abrir `index.html` en el navegador
2. Navegar entre ejes temáticos desde la barra lateral
3. Click en un nodo LNR para asignar/editar plaza
4. Arrastrar nodos para reorganizar el organigrama
5. Exportar a Excel cuando sea necesario

## Estructura

```
ElBus_palmira/
├── index.html                              ← App principal
├── data/
│   ├── estructura_lnr.json                 ← Datos LNR (42 plazas)
│   └── estructura_descentralizados.json    ← Datos entidades
└── README.md
```

## Colores Temáticos

| Eje | Color |
|-----|-------|
| Alcalde (Electivo) | Verde |
| Eje Social | Púrpura |
| Eje Desarrollo | Azul |
| Eje Económico | Naranja |
| Infraestructura | Amarillo |
| Eje Constitucional | Rojo |
| Descentralizados | Teal |

## Tecnologías

- HTML5 / CSS3 / Vanilla JavaScript
- SVG para renderizado de organigramas
- SheetJS para exportación Excel
- localStorage para persistencia

## Licencia

Uso interno - Campaña electoral Palmira 2026
