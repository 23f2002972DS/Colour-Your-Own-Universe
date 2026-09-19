# Colour-Your-Own-Universe
An interactive Python notebook for downloading, processing, and visualizing real astronomical survey images of galaxies, nebulae, and star clusters using Astropy and Astroquery.

An interactive Python project designed to retrieve and visualize real astronomical survey images. By leveraging Python's core astronomy libraries, this notebook allows users to download raw telescope data, enhance faint structural details, and apply scientific colormaps to famous deep-space objects.

## Features
- Real Astronomical Data: Fetches raw imagery from the DSS2 Red survey band using the SkyView interface.
- Curated Target Library: Includes a built-in dictionary of 15 predefined space objects, categorized into Galaxies, Nebulae, Star Clusters, and Supernova Remnants.
- Advanced Image Processing: Utilizes a 99.5% Percentile Interval and an Asinh stretch to reveal faint astronomical structures without overexposing bright core regions.
- Custom Visualization: Randomly pairs targets with distinct scientific colormaps (such as magma, plasma, viridis, twilight, and hot) to highlight structural differences in the single-band images.

## Prerequisites
This project is built for Jupyter Notebook or Google Colab environments. It requires the following Python packages:-
- `astropy`
- `astroquery`
- `numpy`
- `matplotlib`

## Installation & Usage
1. Open the notebook in your preferred *Jupyter environment* or *Google Colab*.
2. Run the first cell to install the required astronomy packages:
   ```bash
   !pip install astroquery astropy
   ```
6. Execute the setup cells to load the Python tools and initialize the target library.
7. Run the randomizer cell to automatically select one of the 15 targets and a specific colormap.
8. The notebook will automatically download the 700x700 pixel image data, apply the brightness stretch, and plot the final visualization.

## Included Targets
The target library comes pre-configured with the standard astronomical names, positional data, and optimal radius sizes for:-
- Galaxies: _Andromeda Galaxy (M31), Triangulum Galaxy (M33), Whirlpool Galaxy (M51), Bode's Galaxy (M81), Sombrero Galaxy (M104)_.
- Nebulae: _Orion Nebula (M42), Lagoon Nebula (M8), Trifid Nebula (M20), Dumbbell Nebula (M27), Ring Nebula (M57)_.
- Star Clusters: _Pleiades (M45), Hercules Globular Cluster (M13), Globular Cluster (M15)_.
- Supernova Remnants: _Crab Nebula (M1), Veil Nebula (NGC 6992)_.

