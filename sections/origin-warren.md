# Warren is born with xAPI

How to make dataviz with an LRS?

## Architecture

📦 Backend as PyPI package: API for learning indicators computing <br>
📊 Frontend as a React component library based on Apache E-Charts

## Distribution

🛠 SDK for learning analytics visualization <br>
🔌 Plugin architecture

::right::

```mermaid {scale: 0.7}
flowchart TB

  lrs[(LRS)]

  subgraph warren [Warren]
    backend[Backend]
    component[Components]
    apache_airflow["Apache Airflow"]
    persistence[(Persistence)]

  end
  charts["📊 📉 📈"]
  lrs -. xAPI .-> backend
  backend --> component
  backend -. Indicator computing persistence .-> persistence
  persistence --> apache_airflow --> component
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
</style>