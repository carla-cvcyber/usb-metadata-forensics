# Autopsy Timeline Analysis – USB Forensics Case

This document provides a step-by-step breakdown of how Autopsy was used to identify metadata anomalies in a suspicious death investigation. The analysis focuses on MACtimes (Modified, Accessed, Created), author metadata, and filename structures to challenge the integrity of key digital evidence.

## Key Steps:
- Created a new case in Autopsy and added the USB image (`C1Prj01.E01`) as the data source
- Enabled all ingest modules for comprehensive timeline and metadata analysis
- Identified two notable files in the Documents folder: `suicide1.txt` and `Sylvia's Assets.xls`
- Examined inconsistencies in:
  - Timestamp ranges (2002 → 2005 → 2017)
  - Author field ("Amelia Phillips" instead of victim)
  - Filename structure (`SYLVIA~1.XLS` suggests legacy OS format)
- Extracted full file metadata and correlated access patterns
- Assessed the likelihood of digital staging based on timing, authorship, and file behavior

This analysis supports the conclusion that the digital evidence had been manipulated and was inconsistent with the presumed timeline of events.
