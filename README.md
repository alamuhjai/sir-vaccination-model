# SIR Vaccination Model

Interactive epidemic simulator exploring herd immunity thresholds, vaccine efficacy, and non-inferiority limits. Built in 2022 with Python (Shiny, SciPy, Matplotlib) and deployed entirely in the browser via Shinylive/WebAssembly — no server required.

**[Live Demo →](https://<USERNAME>.github.io/sir-vaccination-model/)**

## Features

- SIR compartmental model solved with `scipy.integrate.odeint`
- Adjustable R₀, vaccine efficacy, coverage rate, and non-inferiority margin
- Side-by-side comparison of actual VE vs VE−NI limit scenarios
- Herd immunity day calculation via interpolation
- Runs 100% client-side (Python in the browser via Pyodide/WASM)

## Run Locally

```bash
cd site
python -m http.server 8000
```

Then open `http://localhost:8000`.
