# Biochemical_signalling

This project provides a comprehensive framework for simulating geometric and biological tissues using polygonal representations. It includes functionalities for computing geometric properties of polygons, simulating tissue dynamics, and visualizing the results.

## Key Features

- **Geometric Calculations**: Functions to compute the center, area, perimeter, and other properties of polygons.
- **Tissue Simulation**: A `Polygon` class that encapsulates the behavior of polygonal cells, including methods to calculate their area, perimeter, and center.
- **Periodic Boundary Conditions**: Handles periodic boundaries in simulations to effectively model a continuous space.
- **Energy Calculations**: Computes various forms of energy within the system, including elasticity, adhesion, and contraction energy.
- **Visualization**: Functions to plot the network of vertices and polygons for visual analysis.

## Additional Biological Feedbacks in Tissue Growth

- **Actin-Myosin Contractility**: Actin-myosin interactions provide contractile forces within cells, contributing to tissue dynamics by regulating cell shape, movement, and structural stability. This interaction plays a key role in maintaining tissue tension and facilitates cellular rearrangements during growth.
  
- **Rho GTPase Activity**: Rho GTPases regulate the assembly of actin-myosin filaments, thereby influencing contractility and mechanical properties in tissues. This feedback loop also controls cell polarity and organization, affecting tissue morphogenesis and stabilization.
  
- **ROCK Pathway**: Rho-associated protein kinase (ROCK) activates downstream signaling that further enhances actin-myosin contractility. This pathway supports the modulation of tissue rigidity and contributes to controlled growth by dynamically adjusting cellular forces based on environmental and intrinsic signals.

- **Feedback Mechanism in Tissue Growth**: The actin-myosin, Rho, and ROCK feedbacks create a regulatory network, where cell contractility adapts to mechanical stresses, guiding tissue expansion and stability. These pathways collectively help distribute growth forces evenly across cells, promoting uniform tissue growth.

## Python Packages Used

- **NumPy**: For numerical operations and handling arrays.
- **Matplotlib**: For plotting and visualizing the simulation results.

## Class Descriptions

### Polygon Class

The `Polygon` class represents a polygon with methods to calculate its geometric properties:

- **Initialization**: Accepts parameters such as identifier, vertex indices, initial area, perimeter, and orientation angle.
- **Methods**:
  - `get_poly_vertices`: Returns vertices considering periodic boundaries.
  - `get_area`: Calculates the area of the polygon.
  - `get_perimeter`: Calculates the perimeter of the polygon.
  - `get_center`: Computes the geometric center of the polygon.

## Simulation Parameters

A function is provided to set up simulation parameters like box dimensions, coefficients for elasticity and contraction, and time steps. This is crucial for configuring the simulation environment.

## Usage Instructions

1. **Setup Environment**: Ensure you have Python 3.x installed along with NumPy and Matplotlib. Install the required packages using pip:
   ```bash
   pip install numpy matplotlib
