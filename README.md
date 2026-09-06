# Inventario Casa

Sistema simple de inventario con etiquetas NFC.

Cada NFC apunta a la misma web con un `id` distinto en la URL; la página lee
ese `id` de `inventario.json` y muestra la lista de contenido.

## URLs de las ubicaciones

- Canapé cama: `?id=canape-cama`
- Armario dormitorio: `?id=armario-dormitorio`

Ejemplo completo (tras activar GitHub Pages):

```
https://iarazuska.github.io/Inventario-NFC/?id=canape-cama
https://iarazuska.github.io/Inventario-NFC/?id=armario-dormitorio
```

## Añadir o editar ubicaciones

Edita `inventario.json` (desde el móvil se puede hacer directamente en GitHub):

```json
"clave-ubicacion": {
  "nombre": "Nombre visible",
  "contenido": [
    "Objeto 1",
    "Objeto 2"
  ]
}
```

Graba un NFC nuevo con `.../Inventario-NFC/?id=clave-ubicacion`.

## Activar GitHub Pages

1. Settings → Pages
2. Source → Deploy from branch
3. Branch → `main` / `root`
4. Save
