# Polysomnography introduction

Data collection for PSG was standardized among various manufactured instruments by use of standardized collection and display montages. Each unit used for collection was certified before use to maximize signal quality integrity throughout the EDF conversion and import into Compumedics Profusion software used for scoring. Technicians performing CHAT studies also underwent a formal certification procedure.

Notes:

- [Montage and Sampling Rate Information](:pages_path:/equipment/montage-and-sampling-rate-information.md)
- [Polysomnography Data Guide](:pages_path:/psg-data-guide/3-00-psg-data-guide-toc.md.md)

## Original signal and annotation files

[Raw polysomnography data](:files_path:/polysomnography) are available for 453 randomized and 779 nonrandomized CHAT participants. Each recording has a signal file (.EDF) and two versions of the event scoring and epoch staging annotations (.XML).

1. **[EDF](:files_path:/polysomnography/edfs)** - Signal files in the [European Data Format](http://www.edfplus.info/) exported from Compumedics Profusion.
2. **[XML (Profusion)](:files_path:/polysomnography/annotations-events-profusion)** - Annotation files exported from Compumedics Profusion. ([Learn more...](https://github.com/nsrr/edf-editor-translator/wiki/Compumedics-Annotation-Format))
3. **[XML (NSRR)](:files_path:/polysomnography/annotations-events-nsrr)** - Annotation files processed in the [EDF Editor and Translator](https://github.com/nsrr/edf-editor-translator) tool.

NSRR XML files can be overlaid onto EDF signal files using the [EDF Viewer tool](https://github.com/nsrr/edf-viewer). For more information about the XML translation (mapping) process, review the files available on the [EDF Editor and Translator Releases page](https://github.com/nsrr/edf-editor-translator/releases).

**Note:** Events using the `Unsure` tag are Mixed Apneas.

## Harmonization

The CHAT polysomnography recordings ([browse files here](:files_path:/harmonized)) were harmonized using [Luna](https://zzz-luna.org/luna/). Of the original 1639 original EDFs, 1637 were of sufficient quality for inclusion in the harmonized set. Signal and annotation labels were standardized across recordings, and signals were re-referenced as needed, rescaled and checked for reasonable sample rates. A single ECG channel was constructed from unreferenced ECG leads after validating its correspondence to an existing referenced ECG within a subset of the sample. Chin EMGs were generally referenced to a center chin EMG in most cases, with exceptions documented in the issues file. Lastly, in some cases, EDFs had multiple SpO2, plethysmography, and CO2 channels. In these cases, we consulted with study coordinators on which channels to include in the harmonized set.

Automated quality control of the harmonized signals was performed using [Luna's QC command](https://zzz-luna.org/luna/ref/artifacts/#qc), and flagged channels are documented in the issues file. The SpO2 channel showed elevated rates of automated quality-control flags, largely due to calibration errors rather than gross artifact. Additionally, the nasal pressure channel was flagged by automated quality-control across 23% of EDFs. Consequently, users performing analyses that depend heavily on airflow or O2 signals are encouraged to consult the issues file and consider applying additional study-specific quality filtering before analysis.

An in-depth presentation of the harmonization workflow can be found here: https://gitlab-scm.partners.org/zzz-public/nsrr/-/tree/master/studies

## Known issues

- *Oxygen saturation value reaches 101 (300051 baseline) in sleep* - These extraneous values stem back from the original recording equipment and could not be fixed upon re-exporting. ([See list of studies with values >100 in wake.](:pages_path:/polysomnography-sao2-exceeds-100.md))
- *Referenced signals (300051 baseline) and bipolar collection (300927 baseline)* - Original data collection did not conform to official CHAT montage.
- *Pulse signal contains incorrect physical dimension (mbar) (301117 nonrandomized)* - Issue could not be fixed with re-exporting; other signals appear intact.

## History / changelog

*August 4, 2026*
- Add description of [harmonized PSG files](:files_path:/harmonized)

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
