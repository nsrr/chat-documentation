## 5.7 Scoring Procedures

<div class="bs-callout bs-callout-info">
  <strong>Note:</strong> Scoring procedures have been modified to be in compliance with recent Pediatric rules that have been updated by the American Academy of Sleep Medicine. Additional locally introduced rules, based on discussions among the PRC staff and outside consultations may be introduced as the new rules are implemented.
</div>

### 5.7.1 Overview of Scoring

The scorer will review the record using a montage in two passes. First, computer generated scoring of respiratory events during the “offline” processing will be deleted. Then during the first pass, sleep stages and arousals will be marked manually on a (30 s. time base) epoch by epoch basis. During the second pass, respiratory signals will be displayed (2 or 5 min. time base), respiratory events will be manually marked, and oxygen saturation data edited, if necessary.

During manual scoring, the following are primary “events” that are identified:

<u>Sleep stages and Arousals</u> will be identified for each 30 second epoch using updated AASM staging criteria. Obstructive Apneas will be identified if the amplitude (peak to trough) of the airflow signal is flat or nearly flat. This is noted when amplitude of airflow decreases below at least 90% of the amplitude of “baseline” breathing, i.e. to < 10% of the baseline for 90% of the event duration, (identified during a period of regular breathing with stable oxygen levels), and if this change lasts for at least two missed breaths (but not less than 5 seconds duration). The event is associated with continued or increased inspiratory effort throughout the entire period of decreased airflow. Based on newer AASM rule when thermistry is missing or uninterpretable, the nasal pressure signal [CannulaFlow] can be used as an alternative signal for scoring Obstructive Apnea if airflow is bad or missing.

<u>Hypopneas</u> will be identified if the amplitude of nasal pressure or IP Sum channel decreases by at least 50% of the amplitude of “baseline” (identified during a period of regular breathing with stable oxygen levels), if this change lasts for at least two breaths (but not less than 5 seconds duration) and is associated with a >=3% desaturation, arousal, or awakening [at least 90% of the event’s duration must meet the amplitude reduction criteria for hypopnea]. If the nasal pressure or IP Sum channel is poor or missing, secondary signals of both effort bands or airflow with a 50% or more reduction of amplitude can be scored as hypopnea. Discernable change with desaturations that do not meet the rules of hypopnea are NOT scored as hypopneas.

<u>Central Apneas</u> will be noted if no displacement is seen on both the chest and abdominal inductance channels which is associated with absent inspiratory effort throughout the entire period of absent airflow. Otherwise, an event will be noted as “obstructive” or Hypopnea if the event meets the rules. Central events cannot be designated if both band data are missing or uninterpretable. Central events can be scored if one band is missing or uninterpretable, provided that the airflow and nasal cannula are flat. The Central Apnea must last for >= 20 seconds or the duration of two missed breaths (not less than 5 seconds) and is associated with >=3% desaturation, arousal, or an awakening.

<u>Mixed Apnea</u> will be identified if the amplitude of the airflow signal is flat or nearly flat for at least two missed breaths (but not less than 5 seconds duration). The airflow must decrease below at least 90% of the amplitude of baseline breathing for at least 90% of the event duration. The mixed apnea has a central apnea portion followed by an obstructive apnea portion.

<u>Desaturation Events:</u> The proprietary scoring software has the ability to independently score desaturation events from the oxygen saturation channel.

Computer analysis will link data from varying channels to identify desaturation levels, sleep summary data, and various Respiratory Disturbance Indices (RDIs). The following describe how these data are used:

- The <u>desaturation associated with any respiratory event</u> will be based on the nadir desaturation reached within a user defined amount of the time (usually within 30 sec) of the end of the event. The magnitude of the desaturation for an event is the difference between the greatest saturation level observed during the event and this minimum. The scorer will manually check events to assure that the appropriate desaturation is identified and modify as needed.


Each study will be manually scored in the two passes:

- During the first pass:
    - Verify Lights Off, Lights On, Sleep Onset and End of Sleep are set correctly.
    - The EEG, EMG, ECG and EOG signals from each study will be reviewed on an epoch by epoch (30 sec screen) basis. Each epoch will be assigned a sleep stage. Periods of EEG change that meet the criteria for arousal will be marked.
- During second pass:
    - Respiratory data (airflow/cannula/snore/abdominal/chest/sum/Cap/EtCO2/saturation) and leg EMG will be reviewed on 5 or 2 minute page. The saturation channel will be edited for artifact and respiratory events will be marked manually according to the rules stated below.
- Finally, the following will be done:
    - The QS Form will be completed, indicating unusual patterns, reliability problems, and signal/study QA grades.
    - A SAS outlier program will be run, to identify implausible values.
    - Participant Feedback Sleep Reports will be generated.
    - The raw and scored files and summary reports will be saved to the appropriate scored sections on the Network.

<hr class="soften" style="margin-top: 20px;margin-bottom: 20px;"/>

<div class="center">
<div class="btn-group">
  <a href=":pages_path:/mop/5-06-12-archival-of-data.md" class="btn btn-default">
    <span class="glyphicon glyphicon-chevron-left"></span>
    5.6.12 Archival of Data
  </a>

  <a href=":pages_path:/mop/5-00-mop-toc.md" class="btn btn-default">
    <span class="glyphicon glyphicon-chevron-up"></span>
    Manual of Operations
  </a>

  <a href=":pages_path:/mop/5-08-01-scoring-sleep-stages-and-arousals.md" class="btn btn-success">
    5.8.1 Scoring Sleep Stages and Arousals
    <span class="glyphicon glyphicon-chevron-right"></span>
  </a>
</div>
</div>
