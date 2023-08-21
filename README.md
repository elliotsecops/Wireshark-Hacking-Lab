# Wireshark Hacking Lab 
This repository contains a minimal web app designed for network capture and analysis. It consists of a form that submits credentials, displays a response, and allows testing tools such as Wireshark, is hosted on Nginx server, and includes instructions for cloning, running and learning about network security in an ethical way.

# Wireshark Hacking Lab

Este repositorio es un laboratorio de prácticas para capturar y analizar paquetes HTTP en el puerto 8080 con Wireshark, utilizando un servidor Nginx.

## Pre-requisitos

Antes de empezar con este laboratorio, es fundamental tener conocimientos previos sobre Nginx. Si eres nuevo en este tema, te recomendamos revisar la documentación oficial o recursos educativos sobre Nginx antes de continuar.

## Contenido del Repositorio

- Archivo de configuración de Nginx.
- `index.html`: Página principal del servidor.

## Uso del Laboratorio

1. **Clonar el repositorio**:
    ```
    git clone https://github.com/[elliott-fibonacci]/wireshark-hacking-lab.git
    cd wireshark-hacking-lab
    ```

2. **Configurar y ejecutar el servidor Nginx**:
    - Coloca el archivo de configuración de Nginx en el lugar adecuado de tu sistema.
    - Asegúrate de que Nginx sirva el archivo `index.html`.
    - Inicia Nginx.

3. **Captura de paquetes con Wireshark**:
    a. Inicia Wireshark.

    b. Selecciona la interfaz de red por la cual está pasando el tráfico que deseas capturar (comúnmente eth0 para Ethernet o algo similar para Wi-Fi).

    c. Haz clic en el botón "Iniciar" para comenzar a capturar paquetes.

    d. Visita http://localhost (o la dirección que hayas configurado en tu servidor) para generar tráfico.

    e. Una vez que hayas generado suficiente tráfico, detén la captura en Wireshark.

    f. Utiliza los filtros de Wireshark para aislar el tráfico HTTP. Puedes usar el filtro http para este propósito.

    g. Explora los paquetes y presta atención a los detalles, como los encabezados, el cuerpo del mensaje y otros meta datos que te puedan interesar.

    h. Puedes hacer clic derecho en cualquier paquete y seleccionar "Seguir > Flujo TCP" para ver la conversación completa entre el cliente y el servidor.

Análisis en Wireshark

    GET y POST: Estos son los métodos HTTP más comunes. Mira cómo aparecen en Wireshark y qué datos envían o solicitan.
    Encabezados HTTP: Estos contienen información sobre el navegador del usuario, el servidor, las cookies y más.
    Datos de Formulario: Si hay algún formulario en tu index.html, envía datos a través de él y observa cómo se transmiten estos datos.

Contribuciones

Las contribuciones son bienvenidas. Si encuentras algún error o tienes sugerencias, no dudes en abrir un issue o hacer un pull request.

