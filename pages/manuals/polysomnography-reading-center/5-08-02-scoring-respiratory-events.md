## 5.8.2 Scoring Respiratory Events

Scorer will identify the following categories of discrete breathing events: obstructive apneas, central apneas, mixed apneas and hypopneas. Additionally, periodic breathing and periodic large breaths will be identified. Central hypopneas and increased upper airway resistance (RERAs) will not be identified because of controversies in the defining these events and the probable need to use invasive monitoring to identify these accurately.

**<u>Obstructive Apneas</u>** are identified when the amplitude (peak to trough) of the airflow signal decreases to a flat or almost flat signal (showing a 90% reduction of the amplitude of “baseline” breathing for 90% of the duration, this will be known as the 90% criteria) if this change lasts for > duration of two missed breaths and is associated with continued or increased inspiratory effort throughout the entire period of absent airflow. _Baseline breathing_ is defined as a period of regular breathing with stable oxygen levels. The duration of two missed breaths is determined during the first period of N3 sleep (baseline breathing pattern) but will not be less than 5 seconds duration. When airflow is missing or uninterpretable, the nasal pressure signal [CannulaFlow] can be used as an alternative signal for scoring Obstructive Apnea. Without reliable airflow or cannula, the event will default to hypopnea if the event meets the rules for hypopnea. Identification of an apnea does not require a desat, arousal, or awakening.

**<u>Hypopneas</u>** will be identified if ≥50% reduction of amplitude is visualized on either the nasal cannula or the respiratory SUM channel for a duration of at least two missed breaths and associated with ≥3% desaturation, arousal or awakening. The duration of two missed breaths is determined during the first period of N3 sleep (baseline breathing pattern) but will not be less than 5 seconds duration. If the SUM and nasal cannula are not present, if a 50% reduction is seen on both belts (thoracic and abdominal), or 50% reduction on the airflow, and associated with ≥3% desaturation, arousal, or awakening, then a hypopnea may be scored. Discernable change with desaturations that do not meet the rules of hypopnea are NOT scored as hypopnea. Identification of a hypopnea does require a minimum desaturation ≥3%, or association with an arousal or awakening.

- <u>Distinguishing Between Hypopneas and Apneas.</u> This distinction only can be made for events in which airflow by thermistry [or cannula as backup] is interpretable. (If airflow and cannula are uninterpretable, the event-based on inductance data is considered by default to be a hypopnea but must be associated with ≥3% desat, arousal or awakening to be scored as a hypopnea.). Apneas are marked if >90% of the event shows absent or nearly absent airflow on the thermistor channel (and this reduction is 90% the amplitude of the surrounding breaths).

A **<u>Mixed Apnea</u>** event is scored if it meets apnea criteria and is associated with absent inspiratory effort in the initial portion of the event [central apnea portion of the event], followed by resumption of inspiratory effort in the second portion of the event [obstructive apnea portion of the event]. The duration of the event must be at least two missed breaths. The duration of two missed breaths is determined during the first period of N3 sleep (baseline breathing pattern) but will not be less than 5 seconds duration. Mixed Apnea requires reliable airflow [cannula as backup] and belts. Identification of an apnea does not require a desat, arousal or awakening.

A **<u>Central Apnea</u>** event is scored if NO displacement is noted on both chest and the abdominal inductance channels which is associated with absent inspiratory effort throughout the entire period of absent airflow. Otherwise, an event will be noted as “obstructive” or Hypopnea if the event meets the rules. Central events cannot be designated if both band data are missing or uninterpretable. Central events can be scored if one band is missing or uninterpretable, provided that the airflow and nasal cannula are flat [these will be noted as one belt CA on QS comments. The Central Apnea must last for ≥ 20 seconds or the duration of two missed breaths and is associated with ≥3% desaturation, arousal, or an awakening. The duration of two missed breaths is determined during the first period of N3 sleep (baseline breathing pattern) but will not be less than 5 seconds duration.

- <u>Distinguishing Between Central and Obstructive Events.</u> Only events in which there is clear data from both the abdominal and chest signals can be distinguished as “central” or “obstructive”. (Events where one or both of these channels are missing or contain artifact, are considered obstructive or hypopnea if the event meets the rules for Obstructive Apnea or hypopnea). Determining whether an event is central or obstructive in areas of periodic breathing can be difficult because of uncertainties in deciding when to start and end such events. Often, these areas contain breaths that gradually increase and decrease, sometimes decreasing to an imperceptible level. Marking “longer” events in these areas would result in identifying “obstructive” events; “shorter” events are more likely to appear “central.” When it is unclear as to when to start an event, look for evidence of paradoxical breathing. Change in phase angle between thoracic and abdomen is an indicator of upper airway obstruction (such events will be designated as obstructive). When still unclear, the event duration will be marked using the airflow channel. Identify the areas where airflow stops and starts, then assess whether the period is also associated with effort on either channel/band. Then, the inductance channels will be visualized to decide whether during this period, any effort occurred. If any effort was visualized, the event will be considered “obstructive”, otherwise, “central.”

_Duration criteria:_ The beginning of an Apnea/Hypopnea is marked at the end of the last “normal” breath; the end of the event is identified as the beginning of the first breath that exceeds the amplitude of the first reduced breath used to mark the beginning of the event. Duration is based on a “trough to trough” marking lasting at least two missed breaths. The duration of two missed breaths is determined during the first period of N3 sleep (baseline breathing pattern) but will not be less than 5 seconds duration.

Additional notes re Central Apnea scoring:

- Clarification of Amplitude threshold relative to baseline: If one non-artifactual deflection less than 25% of baseline breathing then it is a central. If two deflections less than 25% of baseline breathing providing airflow flat than it is obstructive or mixed. Flat excludes cardiogenic oscillation.


<hr class="soften" style="margin-top: 20px;margin-bottom: 20px;"/>

<div class="center">
<div class="btn-group">
  <a href=":pages_path:/manuals/polysomnography-reading-center/5-08-01-scoring-sleep-stages-and-arousals.md" class="btn btn-default">
    <span class="glyphicon glyphicon-chevron-left"></span>
    5.8.1 Scoring Sleep Stages and Arousals
  </a>

  <a href=":pages_path:/manuals/polysomnography-reading-center/5-00-mop-toc.md" class="btn btn-default">
    <span class="glyphicon glyphicon-chevron-up"></span>
    Manual of Operations
  </a>

  <a href=":pages_path:/manuals/polysomnography-reading-center/5-08-03-nasal-flow-limitation.md" class="btn btn-success">
    5.8.3 Nasal Flow Limitation
    <span class="glyphicon glyphicon-chevron-right"></span>
  </a>
</div>
</div>
