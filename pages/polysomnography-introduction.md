# Polysomnography introduction

Data collection for PSG was standardized among various manufactured instruments by use of standardized collection and display montages. Each unit used for collection was certified before use to maximize signal quality integrity throughout the EDF conversion and import into Compumedics Profusion software used for scoring. Technicians performing CHAT studies also underwent a formal certification procedure.

Notes:

- [Montage and Sampling Rate Information](:pages_path:/equipment/montage-and-sampling-rate-information.md)
- [Polysomnography Data Guide](:pages_path:/psg-data-guide/3-00-psg-data-guide-toc.md.md)

## Signal and annotation files

[Raw polysomnography data](:files_path:/) are available for 453 randomized and 779 nonrandomized CHAT participants. Each recording has a signal file (.EDF) and two versions of the event scoring and epoch staging annotations (.XML).

1. **[EDF](:files_path:/polysomnography/edfs)** - Signal files in the [European Data Format](http://www.edfplus.info/) exported from Compumedics Profusion.
2. **[XML (Profusion)](:files_path:/polysomnography/annotations-events-profusion)** - Annotation files exported from Compumedics Profusion. ([Learn more...](https://github.com/nsrr/edf-editor-translator/wiki/Compumedics-Annotation-Format))
3. **[XML (NSRR)](:files_path:/polysomnography/annotations-events-nsrr)** - Annotation files processed in the [EDF Editor and Translator](https://www.sleepdata.org/community/tools/12) tool.

NSRR XML files can be overlaid onto EDF signal files using the [EDF Viewer tool](https://github.com/nsrr/edf-viewer). For more information about the XML translation (mapping) process, review the files available on the [EDF Editor and Translator Releases page](https://github.com/nsrr/edf-editor-translator/releases).

**Note:** Events using the `Unsure` tag are Mixed Apneas.

## Known issues

- *Oxygen saturation value reaches 101 (300051 baseline) in sleep* - These extraneous values stem back from the original recording equipment and could not be fixed upon re-exporting. ([See list of studies with values >100 in wake.](:pages_path:/polysomnography-sao2-exceeds-100.md))
- *Referenced signals (300051 baseline) and bipolar collection (300927 baseline)* - Original data collection did not conform to official CHAT montage.
- *Pulse signal contains incorrect physical dimension (mbar) (301117 nonrandomized)* - Issue could not be fixed with re-exporting; other signals appear intact.

## History / changelog

*December 19, 2016*
- `baseline`
  - 300420, 300100 replaced (signal labels incorrectly ordered in EDF header)
  - 300555, 300666, 300879, 301053 replaced (previously were actually followup files)
- `followup`
  - 300203 replaced (previously was duplicate of baseline)
  - 300555, 300666, 300879, 301053 replaced (previously were actually baseline files)
- `nonrandomized`
  - 300248, 300298, 300539, 300640, 301009, 301213 replaced (linked references, fixed with re-exporting)

*August 2014*
- Polysomnography data uploaded to sleepdata.org after exports from Compumedics Profusion

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
