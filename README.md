# Material Balance Solver UI

A responsive, browser-based front-end prototype for a chemical engineering material-balance project.

## Features
- Dynamic species, input-stream, output-stream and reaction counts
- Reactor diagram with live input/output arrow updates
- Editable species names
- Dynamic stream component-flow-rate tables
- Reaction order, stoichiometric coefficient and conversion inputs
- DOF calculation using the supplied formula: (Nin + Nout) * Nc + Nr - Nc
- Under-/over-specification warnings

## Run locally
Open `index.html` in a modern browser. No Python installation or server is required.

## Publish with GitHub Pages
1. Create a GitHub repository.
2. Upload `index.html` to the repository root and commit it.
3. Open Settings -> Pages.
4. Under Build and deployment, choose Deploy from a branch.
5. Select `main` and `/ (root)`, then Save.
6. Wait for deployment. GitHub will display the public URL in the Pages section.

## Important modelling note
This prototype counts non-empty stream component flow-rate fields plus non-empty reaction conversion fields as specified values. Reaction orders and stoichiometric coefficients are treated as reaction-model parameters, not independent specifications. Confirm this convention and the supplied DOF equation with your instructor before using the interface for formal process calculations.

This is a UI prototype only; it does not yet assemble or solve the material-balance equations.
