# OpenQARP hands-on — LHC QC Workshop 2026

Hands-on material for exploring high-energy-physics applications with
[OpenQARP](https://github.com/OpenQARP/openqarp), a Python framework for
building and running quantum algorithms.

The examples are deliberately small enough to run on a laptop with the local
OpenQARP simulator. No cloud account or quantum-hardware access is required.

## Notebooks

The workshop material covers:

- **OpenQARP tutorial:** circuits, primitives, engines, variational loops, VQE,
  and QAOA in one sequential notebook.
- **Neutrino oscillations:** two-flavour oscillations and interacting-neutrino
  dynamics.
- **Jet thrust with QAOA:** partitioning a toy collider event into two jet
  hemispheres.
- **Track reconstruction with QAOA:** selecting compatible three-hit track
  candidates in a toy layered detector.

The notebooks use exact local simulation so that their results are
deterministic and reproducible. Exhaustive classical calculations are included
where appropriate as small-instance reference solutions; they are validation
tools, not scalable parts of the proposed quantum workflows.

## Installation

OpenQARP supports Python 3.11–3.14. We recommend creating a fresh virtual
environment:

```bash
git clone https://github.com/OpenQARP/lhc-qc-workshop-2026.git
cd lhc-qc-workshop-2026

python -m venv lhc_env
source lhc_env/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

On Windows PowerShell, activate the environment with:

```powershell
lhc_env\Scripts\Activate.ps1
```

Then start JupyterLab:

```bash
jupyter lab
```

Open a notebook and run its cells from top to bottom. The first optimization
run may take a little longer while numerical libraries initialize.

## Resources

- [OpenQARP repository](https://github.com/OpenQARP/openqarp)
- [OpenQARP documentation](https://docs.openqarp.com/)
- [OpenQARP tutorial](https://docs.openqarp.com/source/tutorial.html)
- [OpenQARP on PyPI](https://pypi.org/project/openqarp/)

## License and citation

OpenQARP is distributed under the Apache License 2.0. See the main OpenQARP
repository for its license, notices, and citation information. Add a license to
this repository before distributing or accepting contributions to the workshop
material.
