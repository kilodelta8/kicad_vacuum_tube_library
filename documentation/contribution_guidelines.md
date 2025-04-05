# Contribution Guidelines

Thank you for your interest in contributing to the KiCAD Vacuum Tube Amplifier Library! Your help in expanding and improving this resource is greatly appreciated.

Please take a moment to read through these guidelines before submitting your contributions. Following these steps will help ensure the quality and consistency of the library.

## How to Contribute

There are several ways you can contribute:

* **Adding New Components:** Creating symbols, footprints, and 3D models for vacuum tubes, transformers, capacitors, resistors, and other relevant components.
* **Improving Existing Components:** Correcting errors, adding missing information (like datasheet links), refining the visual appearance of symbols or footprints, or providing better 3D models.
* **Documentation:** Helping to improve the README, adding more detailed component descriptions, or creating tutorials on using the library.
* **Reporting Issues:** Identifying bugs, inconsistencies, or missing components by creating issues on the GitHub repository.
* **Suggesting Enhancements:** Proposing new features, organizational improvements, or other ideas to make the library better.

## Steps for Contributing New Components

If you would like to contribute a new component (symbol, footprint, and optionally a 3D model), please follow these steps:

1.  **Check for Existing Components:** Before creating a new component, please check the existing library to ensure it doesn't already exist. Use the search functionality on the GitHub repository or browse the library directories.

2.  **Follow the Library Structure:** Adhere to the directory structure outlined in the main `README.md` file. Place your new component files in the appropriate subdirectories based on the component type and (where applicable) manufacturer.

3.  **Naming Conventions:** Follow the established naming conventions for symbols, footprints, and 3D models. Consistency is key!
    * **Symbols:** Generally, use a descriptive name including the part number and optionally the manufacturer (e.g., `12AX7`, `JJ_ECC83S`, `Hammond_272HX`).
    * **Footprints:** Use a descriptive name including the package type, pin count/arrangement, and potentially manufacturer-specific details (e.g., `Tube_Socket_Noval_9Pin`, `Transformer_Mount_Hammond_Style_X`).
    * **3D Models:** Ideally, the 3D model filename should closely match the footprint name.

4.  **Symbol Creation:**
    * Use the KiCAD Symbol Editor.
    * Create a clear and logical symbol representation. Follow common schematic drawing conventions.
    * Include all necessary pins and label them correctly according to the datasheet.
    * Add relevant metadata:
        * **Description:** A concise description of the component.
        * **Keywords:** Terms that users might use to search for the component.
        * **Datasheet:** Include a PDF copy of the datasheet or provide a link to the official datasheet if possible.
        * **Reference:** Include a reference to the manufacturer and part number.
    * Ensure the symbol is correctly linked to a corresponding footprint (if one exists or you are creating one).

5.  **Footprint Creation:**
    * Use the KiCAD Footprint Editor.
    * Create an accurate footprint based on the component's datasheet. Pay close attention to dimensions, pad shapes, and spacing.
    * Include a silkscreen outline, courtyard, and fabrication layers.
    * Add relevant metadata:
        * **Description:** A concise description of the footprint.
        * **Keywords:** Terms that users might use to search for the footprint.
        * **Datasheet:** Provide a link to the official datasheet if possible.
        * **Reference:** Include a reference to the manufacturer and part number or package name.
    * If a 3D model exists, link it to the footprint. Ensure the scaling and orientation are correct.

6.  **3D Model Contribution (Optional but Encouraged):**
    * If you are providing a 3D model, use a common format like STEP (`.step`) or VRML (`.wrl`).
    * Ensure the model is dimensionally accurate and visually representative of the component.
    * Place the 3D model file in the appropriate subdirectory within the `3dmodels` directory, mirroring the symbol and footprint structure.

7.  **Testing:** Thoroughly test your new component(s) by:
    * Placing the symbol in a schematic.
    * Assigning the footprint to the symbol.
    * Viewing the component in the 3D Viewer.
    * Ideally, using the component in a small test project to ensure it functions as expected and include it with your submission.

8.  **Submitting Your Contribution:**
    * Fork the repository on GitHub.
    * Create a new branch in your forked repository for your contribution. Give it a descriptive name (e.g., `add_12AX7_JJ`, `fix_el34_footprint`).
    * Commit your changes to your branch. Make sure your commit messages are clear and concise, describing what you have added or changed.
    * Submit a Pull Request (PR) to the main repository. In your PR description, clearly explain what your contribution is, why you are submitting it, and any relevant information for review.

## Guidelines for Improving Existing Components

If you find an issue with an existing component or have suggestions for improvement:

1.  **Report an Issue:** If it's a bug or missing information, please create a new issue on the GitHub repository, clearly describing the problem or your suggestion.

2.  **Submit a Pull Request (Optional):** If you have the fix or improvement ready, you can fork the repository, create a new branch, make your changes, and submit a Pull Request. Reference the issue number in your PR description if you are addressing an existing issue.

## General Guidelines

* **Datasheets are Your Friend:** Always refer to the official datasheets for accurate dimensions, pinouts, and electrical characteristics.
* **Be Consistent:** Follow the existing style and conventions of the library.
* **Be Clear and Concise:** When creating symbols, footprints, and documentation, aim for clarity and avoid unnecessary complexity.
* **Respect Licensing:** Ensure that any external resources you use (e.g., 3D models from other sources) are compatible with the library's license. If you create something entirely yourself, it will be covered by the library's license upon contribution.
* **Be Patient:** Library maintainers will review your contributions as soon as possible. Please be patient during the review process and be open to feedback.

By following these guidelines, you will help ensure that the KiCAD Vacuum Tube Amplifier Library remains a high-quality and valuable resource for the community. We look forward to your contributions!