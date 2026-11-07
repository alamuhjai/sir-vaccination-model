# SIR Vaccination and Non-Inferiority Model

**Live app:** [alamuhjai.github.io/sir-vaccination-model](https://alamuhjai.github.io/sir-vaccination-model/)

An interactive SIR epidemic simulator built in Python and compiled to WebAssembly with Shinylive so it runs directly in the browser. Developed in 2022 during a placement at the **MRC Unit The Gambia at the London School of Hygiene & Tropical Medicine (LSHTM)** under the guidance of and in collaboration with **Dr. David Jeffries**.

The application implements both the standard SIR model and the modified transmission model of Law et al. Users can adjust the basic reproduction number ($R_0$), recovery period, daily vaccination coverage, vaccination start day, vaccine efficacy ($\text{VE}$), and the non-inferiority ($\text{NI}$) margin. It then plots the epidemic curves and summary tables side by side for actual vaccine efficacy ($\text{VE}$) versus the reduced efficacy at the non-inferiority limit ($\text{VE} - \text{NI}$), showing when herd immunity is reached under each scenario.

## Running locally

The source code is in `myapp/app.py`, and the compiled Shinylive bundle is in `site/`.

```bash
shiny run myapp/app.py
```

Or serve the pre-built static site in `site/`:

```bash
cd site
python -m http.server 8000
```
