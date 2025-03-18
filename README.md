# Quarto Dashboard with Docker and Shiny Server

This repository contains the necessary files to deploy a Quarto dashboard with an R Shiny backend, hosted via Shiny Server on a cloud platform (e.g., Google Cloud Run).

The dashboard is defined in `index.qmd` and is based on [an example from the Shiny Gallery](https://shiny.posit.co/r/gallery/start-simple/kmeans-example/).

To serve the dashboard locally, run: `quarto::quarto_serve("index.qmd")`.

The Dockerfile is configured to render the dashboard inside the container, eliminating the need to commit the rendered output to the repository. The dashboard is served using Shiny Server.
