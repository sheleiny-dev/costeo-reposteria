# Costeo de recetas

Calculadora web para reposteros y emprendedores de repostería. Sirve para saber cuánto cuesta realmente cada receta y a qué precio venderla, sin hojas de cálculo ni cuentas a ojo.

**Pruébala aquí:** https://sheleiny-dev.github.io/costeo-reposteria/

## El problema que resuelve

Muchos reposteros caseros cobran "lo que le parece" y no saben si están ganando o perdiendo. Esta herramienta calcula el costo de cada ingrediente según lo que realmente se usa en la receta y sugiere un precio de venta con el margen de ganancia que cada persona elija.

## Qué puedes hacer

- **Costear ingredientes con unidades reales.** Registra cuánto compraste, cuánto pagaste y cuánto usas. Acepta g, kg, lb, oz, ml, litros, tazas, cucharadas, cucharaditas, unidades y docenas, y convierte entre unidades del mismo tipo.
- **Definir cómo vendes cada receta.** Por porción, galleta, cupcake, unidad o torta entera. Los textos y los precios se ajustan solos.
- **Agregar otros costos y tu ganancia.** Empaque, gas, mano de obra y el porcentaje de ganancia que quieras.
- **Guardar varias recetas.** Una lista con todas tus recetas y su precio sugerido, para ver tu carta completa de un vistazo.
- **Duplicar recetas** para hacer variantes sin escribir todo de nuevo.
- **Enviar precios por WhatsApp.** Un mensaje listo con el precio de una receta, o una lista de precios de toda tu carta. Los mensajes solo incluyen precios, nunca tus costos ni tu ganancia.
- **Guardar en la nube.** Con inicio de sesión de Google, tus recetas aparecen en tu computador y en tu celular.

## Cómo se usa

1. Abre la página y, si quieres guardar tus recetas en la nube, toca **Iniciar sesión con Google**.
2. Escribe el nombre de la receta y agrega sus ingredientes.
3. Indica cuántas unidades salen, cómo las vendes y el porcentaje de ganancia.
4. Mira el precio sugerido y envíalo por WhatsApp si quieres.

Sin iniciar sesión también funciona: las recetas se guardan en el navegador de ese dispositivo.

## Tecnologías

- HTML, CSS y JavaScript, sin librerías ni herramientas de compilación
- [Firebase Authentication](https://firebase.google.com/products/auth) para el inicio de sesión con Google
- [Cloud Firestore](https://firebase.google.com/products/firestore) para guardar las recetas en la nube
- [GitHub Pages](https://pages.github.com/) para publicar la página

Todo el proyecto está en un solo archivo, `index.html`.

## Cómo funciona el guardado

Las recetas se guardan siempre en el navegador. Si inicias sesión, también se guardan en un documento privado de Firestore. Las reglas de seguridad permiten que cada persona lea y escriba solo su propio documento.

## Cómo ejecutarlo en tu computador

1. Descarga o clona este repositorio.
2. Abre `index.html` en tu navegador.

El inicio de sesión con Google solo funciona desde la página publicada, porque Firebase solo acepta los dominios autorizados.

## Ideas para más adelante

- Ajustar el precio según el tamaño de cada pedido
- Exportar la lista de precios como imagen o PDF
- Registrar pedidos y abonos de clientes

## Autora

**Sheleiny Gonzalez** — estudiante de Tecnología en Análisis y Desarrollo de Software, con experiencia en repostería y artes gráficas.

Proyecto creado como práctica de desarrollo web y para resolver una necesidad real del sector.
