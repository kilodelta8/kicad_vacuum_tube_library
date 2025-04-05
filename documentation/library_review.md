# Library Contribution Review Guidelines

This document outlines the guidelines for reviewing contributions (Pull Requests) submitted to the KiCAD Vacuum Tube Amplifier Library. The goal is to ensure that all additions adhere to the established standards for quality, consistency, and usability.

## General Principles

* **Respectful and Constructive Feedback:** Provide feedback in a polite and helpful manner. Focus on the technical aspects of the contribution and avoid personal comments.
* **Adherence to Contribution Guidelines:** Verify that the contribution follows the guidelines outlined in `contribution_guidelines.md`.
* **Accuracy and Completeness:** Ensure that the new components are accurate based on datasheets and include all necessary information.
* **Consistency:** Check that the naming conventions, visual styles, and metadata are consistent with the existing library.
* **Usability:** Evaluate whether the new components are easy to use and understand in KiCAD.

## Review Checklist for New Components

When reviewing a Pull Request that adds new components (symbols, footprints, and/or 3D models), please go through the following checklist:

### Symbol Review

* **[ ] File Location:** The symbol file (`.kicad_sym`) is placed in the correct subdirectory according to the library structure.
* **[ ] Naming Convention:** The symbol name follows the established naming conventions.
* **[ ] Visual Clarity:** The symbol is drawn clearly and logically, following common schematic drawing conventions.
* **[ ] Pin Placement and Numbering:** Pins are placed correctly and numbered according to the datasheet.
* **[ ] Pin Names:** Pin names are accurate and match the datasheet.
* **[ ] Unit Division (If Applicable):** Multi-unit components (e.g., dual triodes) are correctly divided into units.
* **[ ] Power Pins:** Power input and output pins are correctly designated as power types.
* **[ ] Metadata:**
    * **[ ] Description:** A concise and accurate description is present.
    * **[ ] Keywords:** Relevant keywords are included for searching.
    * **[ ] Datasheet Link:** A valid link to the official datasheet is provided (if available).
    * **[ ] Reference:** The manufacturer and part number are included in the reference field.
* **[ ] Footprint Association:** The symbol is correctly linked to a corresponding footprint (or multiple footprints if applicable). The footprint name(s) are accurate.

### Footprint Review

* **[ ] File Location:** The footprint file (`.kicad_mod` or within a `.pretty` directory) is placed in the correct subdirectory according to the library structure.
* **[ ] Naming Convention:** The footprint name follows the established naming conventions.
* **[ ] Dimensional Accuracy:** The footprint dimensions (pad sizes, spacing, overall size) match the datasheet.
* **[ ] Pad Shapes and Layers:** Pads have appropriate shapes and are on the correct copper layer.
* **[ ] Silkscreen:** A clear and non-overlapping silkscreen outline is present.
* **[ ] Courtyard:** A properly sized courtyard is defined.
* **[ ] Fabrication Layers:** Necessary information is present on fabrication layers (e.g., pin 1 indicator).
* **[ ] 3D Model Association (If Applicable):** A 3D model is linked, and its scaling and orientation are correct.
* **[ ] Metadata:**
    * **[ ] Description:** A concise and accurate description is present.
    * **[ ] Keywords:** Relevant keywords are included for searching.
    * **[ ] Datasheet Link:** A valid link to the official datasheet is provided (if available).
    * **[ ] Reference:** The manufacturer and part number or package name are included in the reference field.

### 3D Model Review (If Included)

* **[ ] File Location:** The 3D model file is placed in the correct subdirectory according to the library structure.
* **[ ] File Format:** The model is in a supported format (`.step` or `.wrl` preferred).
* **[ ] Accuracy:** The model visually represents the component and appears to be dimensionally accurate.
* **[ ] Origin and Orientation:** The model's origin and orientation are appropriate for alignment with the footprint.
* **[ ] File Size:** The file size is reasonable.

### General Review

* **[ ] Testing:** The contributor ideally indicates that they have tested the component(s) in KiCAD. (You may want to perform your own quick test as well).
* **[ ] Commit Messages:** The commit messages in the Pull Request are clear and descriptive.
* **[ ] PR Description:** The Pull Request description clearly explains the contribution and any relevant details.

## Review Process

1.  **Initial Assessment:** When a new Pull Request is submitted, perform a quick initial assessment to ensure it's a valid contribution and generally aligns with the project's goals.
2.  **Detailed Review:** Go through the relevant sections of the checklist above, carefully examining the submitted files.
3.  **Provide Feedback:** If any issues are found or improvements can be made, leave clear and specific comments on the Pull Request. Be polite and explain the reasoning behind your feedback.
4.  **Request Changes (If Necessary):** If the contribution does not meet the library standards, request the contributor to make the necessary changes.
5.  **Approve and Merge:** Once the contribution meets all the requirements and you are satisfied with the quality, approve the Pull Request and merge it into the main branch.
6.  **Thank the Contributor:** Acknowledge and thank the contributor for their effort.

## Addressing Issues and Suggestions

When reviewing Pull Requests that address existing issues or propose enhancements:

* **Verify the Issue:** Ensure the contribution effectively addresses the reported issue or implements the suggested enhancement.
* **Evaluate the Solution:** Assess the quality and appropriateness of the solution.
* **Provide Feedback:** Offer constructive feedback as needed.

## Maintaining Consistency

* Refer to existing well-made components in the library as examples of the desired style and quality.
* Communicate any changes to the library's style or guidelines to potential contributors.

By following these review guidelines, we can maintain a high standard for the KiCAD Vacuum Tube Amplifier Library and ensure that it remains a reliable and valuable resource for the community.