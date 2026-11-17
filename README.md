# PolarGrid EnergyLab

An interactive energy management and predictive dispatch prototype designed for polar research stations.

PolarGrid explores how renewable energy, battery storage, and diesel generation can be coordinated to support reliable power management in extreme environments.

## Features

- **Dual operating modes:** Connect a telemetry gateway or configure custom test conditions.
- **Equipment configuration:** Adjust generator, battery, and renewable energy system constraints.
- **Energy monitoring:** View load, battery state of charge, fuel consumption, and energy mix.
- **24-hour dispatch comparison:** Compare a simple dispatch strategy with a predictive planner.
- **Weather scenarios:** Test illustrative storm, winter, and summer operating conditions.
- **Telemetry support:** Read live JSON telemetry from a compatible HTTP/HTTPS gateway.
- **Data export:** Download hourly comparison evidence and telemetry CSV data.
- **Operator review:** Review, approve, or reject generated recommendations with an audit record.

## Technology Stack

- HTML5
- CSS3
- JavaScript
- HTML Canvas for custom charts
- Fetch API for telemetry and backend communication
- CSV for telemetry data import and export

## Operating Modes

### 1. Live Hardware Mode
Connects to a station gateway through an HTTP/HTTPS JSON telemetry endpoint. The dashboard reads telemetry at regular intervals and displays the latest available readings.

### 2. Custom Test Mode
Allows users to configure demand, temperature, solar irradiance, and wind speed to explore different operating conditions.

## Important Notes

- This repository currently contains the frontend prototype (`index.html`).
- Live hardware mode requires a compatible telemetry gateway with CORS access enabled.
- The AI forecasting and telemetry-history features expect a separate Python backend and its API endpoints.
- Forecasts and dispatch comparisons are modelled results, not certified real-world performance measurements.
- Operator approval records do not send control commands to generators or inverters.

## Run Locally

1. Clone this repository:

   ```bash
   git clone https://github.com/2025ee42f-cmd/PolarGrid-EnergyLab.git
   ```

2. Open the project folder.
3. Open `index.html` in a modern web browser.

The frontend interface and custom simulation features can be explored locally. Hardware and backend-dependent features require their respective services.

## Project Status

Interactive prototype — under development.

## Author

Developed as an independent engineering and software project.
