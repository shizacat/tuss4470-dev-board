# TUSS4470 Homemade Evaluation Board

This project aims to design and build a PCB evaluation board for the **TUSS4470** ultrasonic driver that can be manufactured in a home workshop environment.

The main objective is to create a simple, low-cost board that allows testing and characterization of the TUSS4470 in real operating conditions without relying on expensive commercial development kits.

The board will:
- Provide proper power supply and decoupling for the TUSS4470
- Allow connection of an external ultrasonic transducer
- Include basic protection and filtering components
- Be optimized for manual PCB fabrication and soldering (through-hole where possible, reasonable trace widths, minimal layer complexity). Two layer board will be needed.

Requirements:
- Created in KiCad 9.x

## CI/CD — Jobs for home fabrication

On release or manual run, the **KiCad PCB Jobs** workflow produces the **main** artifact (folder `main/` in `kicad-job-main.zip`). It is set up for **home PCB fabrication using the film photoresist method**:

| Layer | Processing | Purpose |
|-------|------------|--------|
| **F (front)** | Inverted and mirrored (mirror + negative) | Print on transparent film for top-side photoresist exposure |
| **B (back)** | Inverted only (negative) | Print on film for bottom-side exposure |

The **main** job outputs layer PDFs (F.Cu, B.Cu), drill files (Excellon), and BOM (CSV). Use them to print masks on transparent film and then UV-expose the photoresist-coated blank.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
