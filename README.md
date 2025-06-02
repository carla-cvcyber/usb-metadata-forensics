# USB Metadata Forensics – Autopsy Case Investigation

This repository documents a digital forensic investigation into a suspicious death, focusing on USB metadata manipulation and its implications for legal and business contexts.

## Executive Summary

Digital evidence integrity is a business survival issue. In this forensic case, metadata anomalies in two files—alleged to be a suicide note and financial document—revealed signs of staged evidence. Misinterpretation of timestamps could have misled the entire investigation. This scenario simulates real-world stakes faced by legal firms, HR departments, and insurance investigators where file origin verification is essential for avoiding reputational, regulatory, or financial fallout.

## Threat Overview

Digital documents are easily manipulated. When timestamps are accepted at face value, staged evidence can go undetected. In this case, files saved in 2005 with metadata dating back to 2002 were presented in a 2017 investigation, creating a misleading timeline intended to validate a false suicide narrative.

## Lab Environment

- **Disk Image:** C1Prj01.E01 (USB)
- **Tool Used:** Autopsy (Sleuth Kit)
- **Ingest Modules:** All enabled for timeline, metadata, and file analysis
- **Time Zone:** GMT-5:00 (US Eastern)

## Execution Steps

1. Created a new Autopsy case using USB disk image
2. Enabled all ingest modules to ensure full parsing
3. Located significant files: `suicide1.txt` and `Sylvia's Assets.xls`
4. Cross-referenced timestamps using MACtimes and metadata fields
5. Extracted and verified author data and filename conventions
6. Identified timeline inconsistencies and misspellings suggesting evidence fabrication

## Results

- Files last modified in 2002
- Saved onto USB in 2005
- Accessed just before 2017 incident
- Authorship attribution to “Amelia Phillips,” not the victim
- Misspelled name within Excel sheet undermines authenticity

## Business Impact Assessment

Had this evidence been accepted without analysis:
- **Legal exposure:** Wrongful death assumption could exonerate a suspect ($500k–$1M in liability)
- **Insurance fraud risk:** Misleading claims could trigger multi-million payouts
- **Compliance failure:** Mishandled digital evidence could breach legal protocols (GDPR, HIPAA)

## Mitigation Strategies

- Mandate metadata validation for all digital evidence
- Incorporate forensic tools like Autopsy in internal investigation playbooks
- Train legal and HR teams on metadata deception patterns
- Implement forensic readiness frameworks for litigation response

## Compliance Relevance

- **ISO/IEC 27037**: Guidelines for identification and preservation of digital evidence
- **GDPR Article 5**: Data integrity and accuracy
- **Chain of Custody**: Maintained throughout investigation process

## License

MIT License.
