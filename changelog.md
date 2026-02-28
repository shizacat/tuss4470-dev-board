# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.1] - 2026-02-28

### Added

- **KiCad Interactive BOM** workflow: generates interactive BOM (ibom) on release and uploads `interactive-bom.zip` to release.


## [0.1.0] - 2026-02-27

### Added

- KiCad 9.x project for TUSS4470 evaluation board (schematic and PCB).
- **KiCad PCB Jobs** workflow: runs jobset on release or manual trigger, produces `kicad-job-main.zip` with layer PDFs (F.Cu, B.Cu), drill files (Excellon), and BOM (CSV) for home film photoresist fabrication.
- **KiCad PCB render (PDF)** workflow: exports PCB to PDF (front/back), STEP and STL 3D models; uploads `pcb-export.zip` to release.
- README with project description, requirements, and CI/CD documentation for home fabrication.
- MIT License.
