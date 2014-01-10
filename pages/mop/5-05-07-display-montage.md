## 5.5.7 Display Montage

- Post acquisition filters will be used for display screen settings.
- Because of the variability of peak-to-peak settings between equipment the display sensitivity should be set so that signals are clear and desired waveforms can be seen.
- If a 60 Hz filter was not on for acquisition it may be used on the display montage.
- EOGs will be displayed to the reference electrode in order to check the signal quality of the reference electrode as well as to map eye movements.
- Sites may choose to employ split screen to display leg EMG, respiratory channels and SpO2 signal at a different time base (2 or 5 min.) if the acquisition system allows.  If this is not possible, all signals will be displayed on 30 sec time base.


### Display Montage 1 (REF is located at FPz)

|  Channel Name  |  Low Filter (Hz)  |  High Filter (Hz)  |  Display Polarity  |  Display Amplitude  |
|:--------------:|:-----------------:|:------------------:|:------------------:|:-------------------:|
|  E1-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  E2-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  Lchin-REF     |  10               |  70                |  Negative ↑        |    \*               |
|  Rchin-REF     |   0.3             |  35                |  Negative ↑        |    \*               |
|  Cchin-REF     |   0.3             |  35                |  Negative ↑        |    \*               |
|  C3-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  C4-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  O1-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  O2-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  F3-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  F4-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  T3-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  T4-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  M1-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  M2-REF        |   0.3             |  35                |  Negative ↑        |    \*               |
|  ECG1-REF      |   1.0             |  35                |  Positive ↑        |    \*               |
|  ECG2-REF      |   1.0             |  35                |  Positive ↑        |    \*               |
|  ECG3-REF      |   1.0             |  35                |  Positive ↑        |    \*               |
|  LLeg1-REF     |  10               |  70                |  Negative ↑        |    \*               |
|  LLeg2-REF     |  10               |  70                |  Negative ↑        |    \*               |
|  RLeg1-REF     |  10               |  70                |  Negative ↑        |    \*               |
|  RLeg2-REF     |  10               |  70                |  Negative ↑        |    \*               |
|  Airflow       |   1.0             |  15                |  Positive ↑        |    \*               |
|  CannulaFlow   |   0.05            |  15                |  Positive ↑        |    \*               |
|  SUM           |   0.05            |  15                |  Positive ↑        |    \*               |
|  Chest         |   0.05            |  15                |  Positive ↑        |    \*               |
|  ABD           |   0.05            |  15                |  Positive ↑        |    \*               |

\* Set Display Amplitude to adequately visualize all waveforms


### Display Montage 2

- EOGs will be displayed to the reference electrode in order to check the signal quality of the reference electrode as well as to map eye movements.
- Sites may choose to employ split screen to display leg EMG, respiratory channels and SpO2 signal at a different time base (2 or 5 min.) if the acquisition system allows. If this is not possible, all signals will be displayed on 30 sec time base.

|  Signal Type          |  Signal Inputs  |  Channel Name  |  Low Filter (Hz)  |  High Filter (Hz)  |  Display Polarity  |  Display Amplitude  |
|:---------------------:|:---------------:|:--------------:|:-----------------:|:------------------:|:------------------:|:-------------------:|
|  EOG                  |  E1-REF         |  E1            |  0.3              |  35                |  Negative ↑        |  \*                 |
|  EOG                  |  E2-REF         |  E2            |  0.3              |  35                |  Negative ↑        |  \*                 |
|  Chin EMG             |  Lchin-Cchin    |  Chin          |  10               |  70                |  Negative ↑        |  \*                 |
|  EEG                  |  F4-M1          |  F4-M1         |  0.3              |  35                |  Negative ↑        |  \*                 |
|  EEG                  |  C4-M1          |  C4-M1         |  0.3              |  35                |  Negative ↑        |  \*                 |
|  EEG                  |  O2-M1          |  O2-M1         |  0.3              |  35                |  Negative ↑        |  \*                 |
|  EEG                  |  T4-M1          |  T4-M1         |  0.3              |  35                |  Negative ↑        |  \*                 |
|  EEG                  |  F3-M2          |  F3-M2         |  0.3              |  35                |  Negative ↑        |  \*                 |
|  EEG                  |  C3-M2          |  C3-M2         |  0.3              |  35                |  Negative ↑        |  \*                 |
|  EEG                  |  O1-M2          |  O1-M2         |  0.3              |  35                |  Negative ↑        |  \*                 |
|  EEG                  |  T3-M2          |  T3-M2         |  0.3              |  35                |  Negative ↑        |  \*                 |
|  ECG                  |  ECG3-ECG1      |  ECG           |  1.0              |  35                |  Positive ↑        |  \*                 |
|  Oximetry-Pulse       |  Internal DC    |  Pulse         |                   |                    |                    |  \*                 |
|  Oximetry Plethysmography Waveform or other quality indicator  |  Pleth (from Oximetry) or other quality indicator  |  Pleth or name of quality indicator  |  |  |  |  \*  |
|  Limb EMG             |  LLeg1-LLeg2    |  LLeg          |  10               |  70                |  Negative ↑        |  \*                 |
|  Limb EMG             |  RLeg1-RLeg2    |  RLeg          |  10               |  70                |  Negative ↑        |  \*                 |
|  Snore Mic (if used)  |  Bipolar        |  Snore         |  20               |  100               |  Positive ↑        |  \*                 |
|  Nasal/Oral Flow      |  Bipolar        |  Airflow       |  1.0              |  15                |  Positive ↑        |  \*                 |
|  Nasal Pressure       |  Pressure Transducer  |  CannulaFlow  |  0.05        |  15                |  Positive ↑        |  \*                 |
|  IP SUM               |  Bipolar        |  SUM           |  0.05             |  15                |  Positive ↑        |  \*                 |
|  IP Chest Effort      |  Bipolar        |  Chest         |  0.05             |  15                |  Positive ↑        |  \*                 |
|  IP Abdominal Effort  |  Bipolar        |  ABD           |  0.05             |  15                |  Positive ↑        |  \*                 |
|  Oximetry numerical   |  Internal DC    |  SAO2          |                   |                    |                    |  \*                 |
|  capnography          |  Auxiliary DC   |  Cap           |                   |                    |                    |  \*                 |
|  capnography          |  Auxiliary DC   |  EtCO2         |                   |                    |                    |  \*                 |
|  Body Position        |  Internal DC    |  Position      |                   |                    |                    |  \*                 |

\* Set Display Amplitude to adequately visualize all signals









<hr class="soften" style="margin-top: 20px;margin-bottom: 20px;"/>

<div class="center">
<div class="btn-group">
  <a href=":pages_path:/mop/5-05-06-chat-standardized-recording-montage.md" class="btn btn-default">
    <span class="glyphicon glyphicon-chevron-left"></span>
    5.5.6 CHAT Standardized Recording Montage
  </a>

  <a href=":pages_path:/mop/5-00-mop-toc.md" class="btn btn-default">
    <span class="glyphicon glyphicon-chevron-up"></span>
    Manual of Operations
  </a>

  <a href=":pages_path:/mop/5-05-08-psg-equipment-care-and-disinfection.md" class="btn btn-success">
    5.5.8 PSG Equipment Care and Disinfection
    <span class="glyphicon glyphicon-chevron-right"></span>
  </a>
</div>
</div>
