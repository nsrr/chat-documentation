# Polysomnography introduction

Data collection for PSG was standardized among various manufactured instruments by use of standardized collection and display montages. Each unit used for collection was certified before use to maximize signal quality integrity throughout the EDF conversion and import into Compumedics Profusion software used for scoring. Technicians performing CHAT studies also underwent a formal certification procedure.

Notes:

- [Montage and Sampling Rate Information](:pages_path:/equipment/montage-and-sampling-rate-information.md)
- [Polysomnography Data Guide](:pages_path:/psg-data-guide/3-00-psg-data-guide-toc.md.md)

## Signal and annotation files

[Raw polysomnography data](:files_path:/) is available for 453 randomized and 779 nonrandomized CHAT participants. Each recording has a signal file (.EDF) and two versions of the event scoring and epoch staging annotations (.XML).

1. **[EDF](:files_path:/polysomnography/edfs)** - Signal files in the [European Data Format](http://www.edfplus.info/) exported from Compumedics Profusion.
2. **[XML (Profusion)](:files_path:/polysomnography/annotations-events-profusion)** - Annotation files exported from Compumedics Profusion. ([Learn more...](https://www.sleepdata.org/tools/edf-editor-and-translator/pages/2-11-compumedics-format.md))
3. **[XML (NSRR)](:files_path:/polysomnography/annotations-events-nsrr)** - Annotation files processed in the [EDF Editor and Translator](https://www.sleepdata.org/tools/edf-editor-and-translator) tool.

## Data notes and updates

CHAT PSG data were originally uploaded in mid-2014.

*December 19, 2016*
- `baseline`
  - 300555, 300666, 300879, 301053 replaced (previously were actually followup files)
- `followup`
  - 300203 replaced (previously was duplicate of baseline)
  - 300555, 300666, 300879, 301053 replaced (previously were actually baseline files)

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.