# docker-rstudio-bigquery
RStudio Server image ready for BigQuery
# Using the rocker/rstudio container

## Quickstart

    docker run -d -p 8787:8787 jsalvarredy/rstudio-bigquery

Visit `localhost:8787` in your browser and log in with username:password as `rstudio:rstudio`.



#### Use a custom password by specifying the `PASSWORD` environmental variable, Link a local volume (in this example, the current working directory, `$(pwd)`) to the rstudio container:


    docker run -d -p 8787:8787 -e PASSWORD=yourpasswordhere -v $(pwd):/home/rstudio  jsalvarredy/rstudio-bigquery
