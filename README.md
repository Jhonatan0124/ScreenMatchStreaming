# Screen Match - Servicio de Streaming

Este es un proyecto Java que implementa un servicio de streaming utilizando el framework de Java Spring. El proyecto maneja listas de series, temporadas y episodios, utilizando varias características avanzadas de Java 8.

## Funcionalidades

- Gestión de series y temporadas.
- Representación de temporadas como listas de episodios.
- Uso de expresiones lambda y streams para el manejo eficiente de listas.
- Manejo de fechas mediante la API de fechas de Java 8.
- Integración de dependencias mediante Maven.

## Requisitos

- Java 8 o superior.
- Spring Framework.
- Maven (gestor de dependencias).

## Instalación y Uso

1. Clona este repositorio en tu máquina local.
   ```bash
   git clone https://github.com/tu-usuario/screen-match.git
2.Abre el proyecto en tu entorno de desarrollo Java (por ejemplo, IntelliJ IDEA).

3.Asegúrate de tener configurado Maven en tu entorno de desarrollo.

4.Ejecuta el comando Maven para instalar las dependencias:
  mvn clean install
5.Configura las propiedades necesarias en el archivo application.properties.

6.Ejecuta la aplicación desde la clase principal ScreenMatchApplication.java.

## Ejemplos de Uso
### Gestión de Series y Temporadas

Series serie = new Series("Breaking Bad");
Temporada temporada1 = new Temporada(1);
temporada1.agregarEpisodio(new Episodio("Piloto", 1));
serie.agregarTemporada(temporada1);

### Uso de Streams y Lambda

List<Series> series = obtenerSeries();
series.stream()
    .filter(serie -> serie.getNombre().startsWith("B"))
    .forEach(System.out::println);





