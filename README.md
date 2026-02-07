# Movie Catalog
_Movie Catalog_ is a **Movie Catalog REST Service** developed as part of the course "[Servicios de Internet](https://secretaria.uvigo.gal/docnet-nuevo/guia_docent/?centre=305&ensenyament=V05G301V01&assignatura=V05G301V01301&any_academic=2024_25)" in the Telecommunications Engineering Degree at the Universidad de Vigo (2024 - 2025).

## About The Project
This project implements a web-based movie information service that allows users to explore films through a multi-phase query process. The system provides a browser-based and REST interfaces where users can select a language, choose an actor or actress, and retrieve the list of related movies in a structured JSON format.

The project features:
- Multi-phase query workflow for guided information retrieval.
- REST-style service accessible from both browser and programmatic clients.
- JSON-formatted responses with ordered results at each phase.
- Language-based filtering followed by actor/actress and movie selection.
- Simple web interface demonstrating each step of the query process.

## How To Run
### Requirements
Make sure you have [Apache Tomcat](https://tomcat.apache.org/) installed and configured on your system, as described in Section 5 of [`Especificaciones.pdf`](docs/Especificaciones.pdf).

Place the required library [`json.jar`](lib/json.jar) inside `public_html/webapps/WEB-INF/lib`.

### Compilation
Make sure you have a [Java JDK](https://www.oracle.com/java/technologies/downloads/) installed on your system. Then compile all Java classes and generate the `.class` files with:
```bash
javac -cp <TOMCAT_HOME>/lib/servlet-api.jar:$HOME/public_html/webapps/WEB-INF/lib/json.jar -d $HOME/public_html/webapps/WEB-INF/classes/ src/*.java
```
This command creates the compiled files inside the `$HOME/public_html/webapps/WEB-INF/classes/` directory.

### Execution
Once compiled, start the Tomcat server.

Then, open your web browser and navigate to `http://localhost:7000/sintX/P2M`.

## About The Code
Refer to [`Especificaciones.pdf`](docs/Especificaciones.pdf), [`Modificaciones.pdf`](docs/Modificaciones.pdf), and [`Screens.pdf`](docs/Screens.pdf) for an in-depth explanation of the project, how it works, how to set up the environment, example outputs, and more.

_The URL used to retrieve the movie catalog may no longer be available._