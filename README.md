# kicad_vacuum_tube_library
A complete vacuum tube amplifier library for KiCAD, finally.

This is a work in progress and being completed in my spare time, so bare with it......

# KiCAD Vacuum Tube Amplifier Library

#### This library provides a comprehensive collection of symbols, footprints, and 3D models for designing vacuum tube amplifiers in KiCAD.

## Installation

There are two main ways to install this library: globally or for a specific project.

### Global Installation

1.  **Download the Repository:** Clone this repository to your local machine.
2.  **Open KiCAD:** Launch the KiCAD application.
3.  **Open the Symbol Library Manager:** Go to `Preferences` -> `Configure Paths...` and add a new path pointing to the `symbols` directory in your cloned repository (e.g., `KISYS3DMOD`). Then, go to `Tools` -> `Symbol Library Editor` -> `Preferences` -> `Manage Symbol Libraries...` and click "Add existing library". Browse to the `kicad-tube-amp-library.kicad_sym` file (if provided) or add the `symbols` directory as a new library path.
4.  **Open the Footprint Library Manager:** Go to `Tools` -> `Footprint Editor` -> `Preferences` -> `Manage Footprint Libraries...` and click "Add existing library". Browse to the `kicad-tube-amp-library.pretty` directory (if footprints are in a `.pretty` repository) or add the `footprints` directory as a new library path.

### Project-Specific Installation

1.  **Copy Library Files:** Copy the `symbols`, `footprints` (and `3dmodels` if desired) directories into your KiCAD project folder.
2.  **Open Project in KiCAD:** Open your KiCAD project.
3.  **Add Symbol Library:** In the Schematic Editor, go to `Preferences` -> `Manage Project Libraries...` under the "Symbol Libraries" tab, click "Add existing library", and browse to the `symbols` directory within your project.
4.  **Add Footprint Library:** In the PCB Editor, go to `Preferences` -> `Manage Project Libraries...` under the "Footprint Libraries" tab, click "Add existing library", and browse to the `footprints` directory within your project.

## Directory Structure

* `symbols/`: Contains KiCAD symbol library files (`.kicad_sym`). Organized by component type (e.g., `tubes/triodes/`, `transformers/power/`, `capacitors/electrolytic/`).
* `footprints/`: Contains KiCAD footprint library files (`.pretty` directories or individual `.kicad_mod` files). Organized by component type (e.g., `tube_sockets/noval/`, `transformer_mounts/`).
* `3dmodels/`: Contains 3D models (`.step`, `.wrl`) for the components. The directory structure mirrors the `symbols` and `footprints` directories for easy linking.
* `documentation/`: Contains additional documentation about the library.
* `LICENSE`: Contains the license under which the library is distributed.

## Contributing

[Link to your contribution guidelines if you plan to accept contributions]

## License

[GPLv3]
