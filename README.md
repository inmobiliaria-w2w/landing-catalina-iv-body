# landing-catalina-iv-body
Aquí se encuentra el resto del código de la landing para el Proyecto Catalina IV

## Resolución del conflicto en `index.html`
Si GitHub muestra un conflicto en el bloque de estilos de la sección "Cerca de todo lo que necesitas" (alrededor de las líneas 550-670 de `index.html`), mantén esta versión:

```css
.catalina-location__lists {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: clamp(18px, 3vw, 32px);
}

@media (max-width: 960px) {
  .catalina-location__lists {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 520px) {
  .catalina-location__title {
    text-align: center;
    margin-inline: auto;
    margin-bottom: 28px;
  }

  .catalina-location__group {
    padding: 20px;
  }

  .catalina-location__map-frame {
    padding: 10px;
  }
}
```

Con ello conservas el diseño de dos columnas en desktop, el cambio a una columna en tablet y el centrado del título/padding reducido en móviles. Si hay dos bloques similares en el conflicto, escoge la opción "Accept incoming change" para el bloque móvil y "Accept current change" para el bloque de desktop para reproducir el resultado anterior.
