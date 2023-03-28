# Warren is born with xAPI

How to make data visualization with an LRS?

## Architecture

💾 LRS as the primary data source <br />
📦 FastAPI backend serving indicators <br />
🧮 Apache Airflow for complex indicators calculation <br />
📊 React frontend components for charts

## Extensibility

- plugin architecture (backend)
- npm packages (frontend)

::right::

```mermaid {scale: 0.7}
flowchart TB

  lrs[(LRS)]

  subgraph warren [Warren]
    backend[FastAPI]
    component[React components]
    apache_airflow["Apache Airflow"]
    persistence[(Warren database)]

  end
  charts["Frontend 📊 📉 📈"]
  lrs -. xAPI .-> backend
  lrs -. xAPI .-> apache_airflow
  backend --> component
  apache_airflow --> persistence
  persistence --> backend
  component --> charts

```

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

.mermaid {
  text-align: center;
}
</style>
