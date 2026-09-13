<!-- Gemini 09/13/26 -->
# Supplementary Material: Inert Zones in L1 Regression

**Authors:** Botan Çıtıl and José H. Dulá

This repository contains the computational scripts, data generation routines, and interactive visualization models accompanying the paper *Inert Zones in L1 Regression*.

The interactive models allow inspecting 2D and 3D simplex projections, cross-sections, and barycenters in detail directly within the browser.

---

## Interactive Visualizations

### Burned Patient Dataset

| Figure Reference | Description | Interactive Link |
| :--- | :--- | :--- |
| **Figure \ref{fig:BurnedPatientData+1AboveSimplexes}** | Burned Patient Data (+1 Above Simplexes) | [View Model](https://220724burnedpatientdataabovesimplexes.netlify.app/) |
| **Figure \ref{fig:BurnedPatientDataAboveSimplexes}** | Burned Patient Data (Above Simplexes) | [View Model](https://220724burnedpatientdata-1belowsimplexes.netlify.app/) |
| **Figure \ref{fig:BurnedPatientData-1AboveSimplexes}** | Burned Patient Data (-1 Above Simplexes) | [View Model](https://220724burnedpatientdataplus1abovesimplexes.netlify.app/) |
| **Figure \ref{fig:BurnedPatientData-2AboveSimplexes}** | Burned Patient Data (-2 Above Simplexes) | [View Model](https://220724burnedpatientdata-1abovesimplexes.netlify.app/) |
| **Figure \ref{fig:BurnedPatientData-1BelowSimplexes}** | Burned Patient Data (-1 Below Simplexes) | [View Model](https://220724burnedpatientdata-2abovesimplexes.netlify.app/) |
| **Figure \ref{fig:BurnedPatientData-2AboveInertZoneCrossSection}** | Burned Patient Data (-2 Above Inert Zone Cross-Section) | [View Model](https://220812burnedpatientdata-2aboveinertzo.netlify.app/) |
| **Figure \ref{fig:BurnedPatientData-1InertZoneCrossSection}** | Burned Patient Data (-1 Below Inert Zone Cross-Section) | [View Model](https://220812burnedpatientdata-1belowinertzo.netlify.app/) |

### Synthetic / 10-Point Dataset

| Figure Reference | Description | Interactive Link |
| :--- | :--- | :--- |
| **Figure \ref{fig:DataSet_1_InertZonesAboveAndBelow}** | 10-Point Inert Zones (Above and Below) | [View Model](https://inert10pts001.netlify.app/) |
| **Figure \ref{fig:DataSet_1_SimplexesAbove}** | 10-Point Simplexes (Above) | [View Model](https://inert10pts001simplexesabove.netlify.app/) |
| **Figure \ref{fig:DataSet_1_SimplexesBelow}** | 10-Point Simplexes (Below) | [View Model](https://inert10pts001simplexesbelow.netlify.app/) |
| **Figure \ref{fig:DataSet_1_InertZonesAbove_2D}** | 10-Point Inert Zones (Above, 2D Cross-Section) | [View Model](https://inert10pts0012dabove.netlify.app/) |
| **Figure \ref{fig:DataSet_1_InertZonesBelow_2D}** | 10-Point Inert Zones (Below, 2D Cross-Section) | [View Model](https://inert10pts0012dbelow.netlify.app/) |

---

## Repository Structure and Setup

### Prerequisites

The computations and visualizations are implemented in Python using the following core scientific packages:

* `numpy` (vector arithmetic and coordinate transformations)
* `scipy` (halfspace intersection, convex hulls, and linear programs)
* `plotly` (interactive HTML 2D/3D visualizations)

Install all requirements via `pip`:

```bash
pip install numpy scipy plotly
