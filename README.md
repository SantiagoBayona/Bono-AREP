# Bono Parcial

Estas instrucciones te ayudarán a obtener una copia del proyecto en funcionamiento en tu máquina local para desarrollo y pruebas. Consulta la sección de "Despliegue" para obtener notas sobre cómo implementar el proyecto en un sistema en vivo.

### Prerrequisitos
- Java
- Maven

### Instalación

1. Clonar el repositorio

```
git clone https://github.com/SantiagoBayona/Bono-AREP
```

2. Dentro del directorio del proyecto lo construimos

```
mvn package
```

## Ejecución

1. Corremos el servidor en local

```
java -cp "target/classes;target/dependency/*" edu.escuelaing.SparkWebServer
```

2. Ingresamos a la página mediante esta URL en un navegador

```
https://localhost:4567
```
## Pruebas

Para probar se puede hacer con la imagen de docker desde el repositorio. Para esto corremos el comando

```
docker run -d -p 34000:6000 --name [nombre de la instancia] santiagobayona04/arepbono
```
Al hacerlo vemos que el recurso solicitado carga en el navegador

![bono arep](https://github.com/SantiagoBayona/Bono-AREP/assets/64861204/d498f832-07db-4b2f-9b78-7df81dece4ad)

## Construido con

* Java
* Maven
* Git
