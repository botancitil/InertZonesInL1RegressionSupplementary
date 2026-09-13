<!-- Gemini 09/13/26 -->
# Supplementary Material: Inert Zones in L1 Regression

**Authors:** Botan Çıtıl and José H. Dulá

This repository contains computational scripts, empirical and synthetic data suites, and interactive visualization models accompanying the paper *Inert Zones in L1 Regression*.

The interactive models allow inspecting 2D and 3D simplex projections, cross-sections, and barycenters in detail directly within the browser.

---

## Interactive Visualizations

### Burned Patient Dataset ($m=4$)
Empirical data source: [`RealDataSets`](https://github.com/botancitil/RealDataSets)

| Figure Reference | Description | Interactive Link |
| :--- | :--- | :--- |
| **Figure 1a** | Upper simplex pair ($\Delta=3$); interior simplex collapses to a point | [View Figure](https://220724burnedpatientdataabovesimplexes.netlify.app/) |
| **Figure 1b** | Upper simplex pair ($\Delta=2$); interior simplex fully contained | [View Figure](https://220724burnedpatientdata-1belowsimplexes.netlify.app/) |
| **Figure 1c** | Upper simplex pair ($\Delta=1$); extreme points touch exterior facets | [View Figure](https://220724burnedpatientdataplus1abovesimplexes.netlify.app/) |
| **Figure 1d** | Upper simplex pair ($\Delta=0$); truncated simplex intersection | [View Figure](https://220724burnedpatientdata-1abovesimplexes.netlify.app/) |
| **Figure 1e** | Lower simplex pair ($\Delta=1$); 3D orthoplex intersection | [View Figure](https://220724burnedpatientdata-2abovesimplexes.netlify.app/) |
| **Figure 1f** | Cross section of upper inert zone ($\Delta=0$) in isolation (truncated simplex) | [View Figure](https://220812burnedpatientdata-2aboveinertzo.netlify.app/) |
| **Figure 1g** | Cross section of lower inert zone ($\Delta=1$) in isolation (3D orthoplex / octahedron) | [View Figure](https://220812burnedpatientdata-1belowinertzo.netlify.app/) |

### Numerical Example / `DataSet_1` ($m=3, n=10, \Delta=1$)

| Figure Reference | Description | Interactive Link |
| :--- | :--- | :--- |
| **Figure 2** | Upper (green) and lower (magenta) inert zones as 3D unbounded prisms | [View Figure](https://inert10pts001.netlify.app/) |
| **Figure 3a** | Upper simplex pair and shared barycenter cross sections | [View Figure](https://inert10pts001simplexesabove.netlify.app/) |
| **Figure 3b** | Lower simplex pair and shared barycenter cross sections | [View Figure](https://inert10pts001simplexesbelow.netlify.app/) |
| **Figure 3c** | 2D triangular cross section of upper inert zone on $X_1, X_2$ subspace | [View Figure](https://inert10pts0012dabove.netlify.app/) |
| **Figure 3d** | 2D hexagonal cross section (orthoplex) of lower inert zone on $X_1, X_2$ subspace | [View Figure](https://inert10pts0012dbelow.netlify.app/) |

---

## Datasets and Data Suites

* **[Burned Patient Dataset (`RealDataSets`)](https://github.com/botancitil/RealDataSets):** Contains the empirical dataset used to generate the 3D simplex pair intersections and cross-sections shown in Figure 1.
* **[Synthetic Data Suites (`SyntheticDataSuites`)](https://github.com/botancitil/SyntheticDataSuites):** Contains the 1,200 generated benchmark suites across dimensions $m \in \{5, 10, 15, 20\}$, cardinalities $n \in \{512, 1024, 2048, 4096, 8192\}$, and five continuous distributions (Laplace, Normal, Cauchy, Uniform, Triangular) utilized for empirical volume estimation and dynamic streaming time-reduction experiments.

---

## Computational Implementation and Setup

Geometric computations for inert zones, convex hulls, halfspace intersections, and interactive vector graphics are implemented in Python.

### Dependencies

* `numpy`
* `scipy`
* `plotly`

Install required packages:

```bash
pip install numpy scipy plotly
