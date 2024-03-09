---
lab:
  title: "Laboratorio\_4: Compilación de la interfaz de usuario"
  module: 'Module 4: How to build the UI in a canvas app in Power Apps'
---

# Laboratorio de práctica 4: Compilación de la interfaz de usuario

En este laboratorio, cambiará los colores de los controles de la aplicación.

## Aprendizaje

- Uso de temas
- Personalización de la aplicación

## Pasos de alto nivel del laboratorio

- Seleccione un tema
- Personalización
  
## Requisitos previos

- Debe de haber completado la práctica **Laboratorio 3: Creación de una aplicación de lienzo**

## Pasos detallados

## Ejercicio 1: Tema

### Tarea 1.1: Edición de la aplicación

1. Vaya al portal de Power Apps Maker <https://make.powerapps.com>.

1. Asegúrese de que está en el entorno **Dev One**.

1. En el menú de la izquierda, seleccione la pestaña **Aplicaciones**.

1. Seleccione la **aplicación Solicitud de reserva**, los comandos (**...**) y **Editar > Editar en una pestaña nueva**.

### Tarea 1.2: Selección de un tema

1. En la barra de acciones de Power Apps Studio, seleccione **Tema**.

    ![Captura de pantalla de selección de temas.](../media/select-theme.png)

1. Seleccione el tema **Rojo**.

### Tarea 1.3: Controles de marca

1. En el menú de creación de aplicaciones, seleccione **Vista de árbol**.

1. Expanda la galería **BookingRequestList**.

1. Seleccione **NextArrow2**.

1. Establezca la propiedad **Color** de NextArrow en la barra de fórmulas como:

    ```powerappsfl
    RGBA(164, 38, 44, 1)
    ```

1. Seleccione **Body1**.

1. Establezca la propiedad **Color** de Body en la barra de fórmulas como:

    ```powerappsfl
    If(ThisItem.Cost > 1000, RGBA(164, 38, 44, 1), Color.Black)
    ```

1. Seleccione **Guardar** en la parte superior derecha de Power Apps Studio.


## Ejercicio 2: Personalización

### Tarea 2.1: Adición de etiqueta de usuario

1. Seleccione fuera de la galería en el lienzo en blanco o seleccione la **MainScreen**.

1. En el menú de creación de aplicaciones, seleccione **Insertar (+)**.

1. Seleccione **Etiqueta de texto**.

1. Arrastre la etiqueta a la parte superior derecha de la pantalla.

1. En el menú de creación de aplicaciones, seleccione **Vista de árbol**.

1. Cambie el nombre de la etiqueta a `UserLabel`.

1. Establezca las propiedades de la etiqueta en la barra de fórmulas de la manera siguiente:

   1. X=`1100`
   1. Y=`20`
   1. Altura=`40`
   1. Ancho=`250`
   1. Alineación=`Align.Right`
   1. Tamaño=`18`
   1. PaddingRight=`10`
   1. Color=`Color.White`
   1. Texto=`User().FullName`

    ![Captura de pantalla de la pantalla principal con personalización.](../media/main-screen-personalized.png)

1. Seleccione **Guardar** en la parte superior derecha de Power Apps Studio.

1. Seleccione el botón **<- Atrás** en la parte superior izquierda de la barra de comandos y seleccione **Salir** para salir de la aplicación.
