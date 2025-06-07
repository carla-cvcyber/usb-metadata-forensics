# Autopsy Timeline Analysis – USB Forensics Case

This document provides a step-by-step breakdown of how Autopsy was used to identify metadata anomalies in a suspicious death investigation. The analysis focuses on MACtimes (Modified, Accessed, Created), author metadata, and filename structures to challenge the integrity of key digital evidence.

## Key Steps:
- Created a new case in Autopsy and added the USB image (`CaseUSB.E01`) as the data source
- Enabled all ingest modules for comprehensive timeline and metadata analysis
- Identified two notable files in the Documents folder: `suic***1.txt` and `Donna's Assets.xls`
- Examined inconsistencies in:
  - Timestamp ranges (2002 → 2005 → 2017)
  - Author field ("Samantha Key" instead of victim)
  - Filename structure (`DANA~1.XLS` suggests legacy OS format)
- Extracted full file metadata and correlated access patterns
![image](https://github.com/user-attachments/assets/64dee779-4fbb-4a56-b32c-02d16d42e232)

- MODIFIED TIME: the last time the file content was updated and saved. Same day, seconds apart for both files.
- ACCESSED TIME: when the file was last viewed or opened by the user or accessed by the system. They're both accessed at the same time.
- CREATED TIME: when the file was created in the system, or saved to the USB stick in this case. Once again, the files were manipulated at the same time, just seconds apart.
- CHANGED TIME: When the MFT entry was last modified in a NTFS filed system, but we're dealing with FAT32 here, so it's all zero.
  
- I then assessed the likelihood of digital staging based on timing, authorship, and file behavior

This analysis supports the conclusion that the digital evidence had been manipulated and was inconsistent with the presumed timeline of events.
