**Report on**

**AI-POWERED AUTOMATED UNDERWATER MARINE DEBRIS AND ANOMALY DETECTION**

**Smart India Hackathon 2026**\
**Problem Statement ID:** [S26057]{.underline}\
**Theme:** Disaster Management\
**PS Category:** Software\
**Team ID:** SIH26-21\
**Team Name:** Cognexa 2. O

![](marine_marine_media/media/marine_media/media/image1.jpeg){width="6.5in" height="3.33125in"}

**[INTRODUCTION]{.underline}**

**Background**

Abandoned, lost and discarded fishing gear (ALDFG), commonly known as ghost gear, includes lost nets, traps, ropes and other fishing equipment. It can continue catching marine life, damage habitats and create hazards for vessels and fishers. Ghost gear affects approximately **66% of marine mammal species, 50% of seabird species and all sea-turtle species**. [[WWF, 2020]{.underline}](https://wwfint.awsassets.panda.org/downloads/wwfintl_ghost_gear_report_1.pdf)

The issue is also significant in India. A Kerala study estimated annual gear loss at approximately **167.5 kg per vessel**, including gear that was lost, abandoned or discarded. [[Kerala ALDFG study]{.underline}](https://link.springer.com/article/10.1007/s12601-022-00074-y)

**Problem Statement**

Side-scan sonar can survey large areas of the seabed, but manually reviewing the resulting imagery is slow, subjective and difficult to scale. Reviewers may miss targets or interpret the same object differently. In addition, a sonar detection alone does not provide a recovery priority, risk level or complete location record.

**Proposed Solution**

Abyssal Scan is an AI-assisted side-scan-sonar system that detects likely marine debris and abandoned fishing gear. It assigns each target a location, confidence score, object fingerprint and risk level. Human reviewers can confirm or correct the AI results before the system creates hotspot maps and a prioritised recovery list.

**Scope**

Abyssal Scan focuses on sonar-image analysis, AI detection, human validation, risk mapping and recovery prioritisation. It supports recovery teams but does not replace physical recovery operations. Factors such as depth, weather, currents and available equipment will still determine whether a target can be removed.

**Expected Contribution**

The project connects:

**Sonar survey → AI detection → Human validation → Risk scoring → Hotspot map → Recovery priority → Recycling or follow-up survey**

This converts raw sonar imagery into practical information for protecting marine life, supporting fishers and improving marine-debris recovery.

**PROBLEM SIGNIFICANCE**

Abandoned, lost and discarded fishing gear---known as ghost gear---continues to catch marine animals, damage habitats and create hazards for fishers and vessels even after it is lost. It affects approximately **66% of marine mammal species, 50% of seabird species and all sea-turtle species**. [[WWF, 2020wwfint.awsassets.panda]{.underline}](https://wwfint.awsassets.panda.org/downloads/wwfintl_ghost_gear_report_1.pdf)

The problem is also significant in India. A study of 390 fishing crews in Kerala estimated annual gear loss at **167.5 kg per vessel**, with 11.6% of gear lost, 7.5% abandoned and 2.3% discarded. [[Kumar et al., 2022](https://doi.org/10.1007/s12601-022-00074-y)[adsabs.harvard](https://ui.adsabs.harvard.edu/abs/2022OSJ....57..398D/abstract)]{.underline}

India's fisheries are economically important, with seafood exports valued at **₹62,408.45 crore in FY 2024--25**. Continued gear loss can affect fish stocks, fishing efficiency and coastal livelihoods. [[MPEDA/PIBpib.gov]{.underline}](https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=2160131&reg=3&lang=2)

Side-scan sonar can help survey large seabed areas, but manually reviewing sonar imagery is slow, subjective and difficult to scale. This creates a gap between **detecting debris** and **deciding what should be recovered first**. Abyssal Scan addresses this gap by using AI to identify potential debris, validate detections through human review, map risk hotspots and produce a prioritised recovery list.

**[EXISTING GAPS]{.underline}**

**1. Slow manual review**

Side-scan-sonar imagery is commonly examined manually, which is time-consuming, inefficient and highly dependent on reviewer experience. Large surveys can contain extensive imagery, making it difficult to maintain attention and consistency throughout the review process. [[BHP-UNet study, 2023](https://link.springer.com/article/10.1186/s13634-023-01040-z)[link.springer](https://link.springer.com/article/10.1186/s13634-023-01040-z?error=cookies_not_supported&code=36459d07-6f63-4aae-a08d-53114e2cde18)]{.underline}

**2. Missed and inconsistent detections**

Sonar images may contain noise, shadows, seabed patterns and overlapping targets. Natural structures can resemble fishing gear, while partially buried or poorly positioned objects may be missed. Interpretation can therefore vary between reviewers, especially in complex seabed environments. [[WWF Baltic ghost-gear study, 2022frontiersin]{.underline}](https://www.frontiersin.org/journals/marine-science/articles/10.3389/fmars.2022.981840/full)

**3. Detection does not guarantee recovery**

Identifying a possible object is only the first step. Recovery teams also need accurate coordinates, target information and a practical priority order. One side-scan-sonar study identified **114 potential gear targets**, but only **one item was confirmed recovered**, demonstrating the difficulty of converting detections into successful recovery. [[Foley et al.ecce.esri]{.underline}](https://ecce.esri.ca/dal-blog/2022/02/17/the-deeper-picture-on-ghost-gear/)

**4. Lack of structured target information**

Traditional sonar review may produce image annotations or target points, but not always a complete recovery-ready record. Important information such as object type, confidence, estimated size, ecological risk and recovery status may be recorded inconsistently or not at all.

**5. No risk-based prioritisation**

A simple map of detected objects does not show which targets pose the greatest threat to marine life or which are most practical to recover. Without risk scoring, teams may spend resources on low-priority targets while more damaging ghost gear remains underwater.

**6. Limited follow-up tracking**

Without persistent object IDs, it is difficult to determine whether the same debris appears in later surveys, whether it has been removed or whether it has shifted location. This limits long-term monitoring and makes cleanup impact difficult to measure.

**7. Weak connection between detection and recycling**

Sonar surveys may identify submerged fishing gear, while collection and recycling programmes operate separately. Without a clear handoff from detected target to recovery team and collection centre, identified debris may not reach the next stage of removal or recycling.

These gaps show that the challenge is not only detecting marine debris. The larger need is an integrated system that can screen sonar imagery efficiently, reduce inconsistent interpretation, organise detections into recovery-ready records, rank targets by risk and connect confirmed debris with recovery and recycling operations. Abyssal Scan is designed to address this detection-to-action gap.

![https://cdn.discordapp.com/attachments/1541430820642754602/1545476714858151946/file_00000000693c8211a666f1a9c3ca7ab9.png?ex=6abbecda&is=6aba9b5a&hm=5601836a377b2d05a0d4e529a17314823e00ed4d50edb9413ed08b6ffee912f0&](marine_marine_media/media/marine_media/media/image2.png){width="1.5659722222222223in" height="1.5659722222222223in"}

**[PROPOSED SOLUTION]{.underline}**

Abyssal Scan is an AI-assisted side-scan-sonar analysis and recovery-prioritisation system designed to identify abandoned, lost and discarded fishing gear and other marine debris. It addresses the gap between collecting sonar imagery and producing practical recovery decisions.

![](marine_marine_media/media/marine_media/media/image3.jpeg){width="4.027777777777778in" height="2.6979166666666665in"}The system begins with side-scan-sonar imagery collected from a survey vessel or obtained from an existing survey dataset. The imagery is preprocessed to improve consistency and divided into smaller sections suitable for AI analysis. A computer-vision model then identifies possible nets, traps, ropes and other debris by analysing their acoustic patterns, shapes and shadows.

Each detected object is converted into a structured target record containing:

-   Georeferenced location.

-   Possible object category.

-   Detection confidence.

-   Estimated size or extent.

-   Acoustic and visual characteristics.

-   Ecological-risk level.

-   Recovery accessibility.

-   Human-review status.

-   Persistent object fingerprint.

A human reviewer validates the AI output by confirming, rejecting or correcting detections. This human-in-the-loop approach is important because sonar images may contain rocks, seabed features, shadows and partially buried objects that can resemble fishing gear. Human corrections can also be stored as feedback for future model improvement.

After validation, Abyssal Scan assigns each target a recovery-priority score. The score can combine detection confidence, object type, estimated size, potential threat to marine life, proximity to fishing or sensitive habitats and ease of recovery. This allows recovery teams to focus first on targets that are both environmentally important and practically recoverable.

The system produces two main outputs:

1.  **Risk-weighted hotspot map:** Shows areas where marine debris is concentrated and where it presents the greatest ecological or operational risk.

2.  **Prioritised recovery list:** Provides recovery teams with ranked targets, coordinates, object information and review status.

Each target is assigned a persistent fingerprint based on features such as location, shape, size, acoustic intensity and shadow pattern. This allows the same object to be compared across repeated surveys and marked as recovered, relocated or still unresolved.

The final output can be shared with fisheries agencies, ports, survey teams, conservation organisations and fishnet collection centres. This creates a complete workflow:

**Sonar survey → AI detection → Human validation → Object fingerprinting → Risk scoring → Hotspot mapping → Recovery prioritisation → Recycling or follow-up survey**

Abyssal Scan is not intended to replace divers, vessels or recovery equipment. Instead, it supports these teams by reducing the amount of imagery they must review and directing them towards the targets most likely to produce environmental and operational benefits. Its recovery outputs can also support Tamil Nadu's Fishnet Initiative, which provides collection and recycling infrastructure for discarded fishing nets across the state. [[TNPCB/TNGCC, Tamil Nadu Fishnet Initiativetngcc.tn]{.underline}](https://tngcc.tn.gov.in/wp-content/uploads/2025/11/envfor_e_122_ms_2025-FIshnet-2025.pdf)

The proposed workflow is supported by existing ghost-gear detection projects that use high-resolution side-scan sonar, AI-based target identification, expert validation, georeferencing and field recovery. GhostNetZero, for example, uses AI to highlight likely ghost-net locations for expert review before divers verify and retrieve confirmed targets. [[Microsoft, GhostNetZero]{.underline}](https://unlocked.microsoft.com/ghostnetzeroai/) This establishes a practical precedent for Abyssal Scan while leaving room for local adaptation to Indian coastal conditions.

**[SYSTEM WORKFLOW]{.underline}**

### Purpose

The system ingests side-scan sonar (SSS) data, cleans it, detects known objects (debris nets, pipes/cylinders, shipwrecks) and unknown anomalies, scores each detection, assigns real-world coordinates, and presents everything in a dashboard with JSON/CSV export. It runs on CPU, so it can be used at the edge without a cloud dependency.

**What happens at each step ?**

  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Step**                    **What the system does**                                                                                                                     **What the operator sees / gets**
  --------------------------- -------------------------------------------------------------------------------------------------------------------------------------------- --------------------------------------------------------------------------------------------
  1\. Upload / Select         Accepts a real .xtf log, a PNG/JPG sonar image, or the bundled demo image.                                                                   File picker and a \'use bundled demo image\' tick box.

  2\. Input Guard             Checks that the image really looks like sonar (sonar_guard.py). Ordinary photos are blocked from the sonar models.                           A warning, and the option to use Optical triage mode instead.

  3\. Preprocessing           Masks the nadir gap, inpaints motion-dropout rows, removes speckle noise, boosts contrast in shadows (CLAHE), resizes to a canonical size.   A cleaner viewport image. Display palettes (Deep Cyan, Sepia, Phosphor) are cosmetic only.

  4\. Detection               Three detectors run side by side: baseline debris YOLO11-Nano, real-data shipwreck YOLO, and a CNN autoencoder for shapes with no label.     Raw candidate boxes.

  5\. Fusion + noise filter   Merges the candidates, discounts likely rock/shadow false positives, and produces a 0-100% confidence.                                       Confidence % on each card; confidence gate defaults to 0.30.

  6\. Quality scoring         Adds quality_score, quality_tier and supporting evidence fields to every detection.                                                          Ranked, traceable detection cards.

  7\. Geotagging              Converts pixel boxes to latitude/longitude using ping index (along-track) and pixel column (across-track).                                   Detections plotted on the Folium map.

  8\. Report export           Writes geotagged detections to JSON and CSV.                                                                                                 Download buttons (the only real export in this build).

  9\. Review                  Operator reviews cards, map and telemetry (count, confidence, measured latency).                                                             Decision: confirm, investigate, or dismiss each target.
  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Two input modes

  -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Mode**                 **Pipeline**                                                                                                                                         **Status**
  ------------------------ ---------------------------------------------------------------------------------------------------------------------------------------------------- -----------------------------------------------------------
  Side-scan sonar          Full pipeline above (YOLO + autoencoder + fusion + geotagging).                                                                                      Primary system.

  Optical / camera photo   Pretrained COCO-YOLO used as a generic object proposer (its class name is only a secondary hint) plus a classical heuristic for plastic bags/film.   Assistive triage only. Not a trained specialist detector.
  -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Operating rules built into the workflow

-   Confidence gate defaults to **0.30**, chosen because it maximizes recall-weighted F2 on the held-out set.

-   Non-sonar images never reach the sonar models.

-   Every figure on the dashboard is derived from the real pipeline. There is no PDF export or GIS/ROS2 sync.

Detections from sequential frames can be merged into track-like records with aggregate_detections(), only when frames share the same pixel geometry.

## 

## 

## 

## 

## 

## 

## [TECHNICAL WORKFLOW (ENGINEERING VIEW)]{.underline}

## ![](marine_marine_media/media/marine_media/media/image4.png){width="2.792361111111111in" height="6.726388888888889in"}![](marine_marine_media/media/marine_media/media/image5.png){width="0.1111111111111111in" height="0.1597222222222222in"}![](marine_marine_media/media/marine_media/media/image6.png){width="0.1111111111111111in" height="0.1597222222222222in"}![](marine_marine_media/media/marine_media/media/image5.png){width="0.1111111111111111in" height="0.1597222222222222in"}![](marine_marine_media/media/marine_media/media/image6.png){width="0.1111111111111111in" height="0.1597222222222222in"}Module-level data flow. Left column is the code path; right column shows what is produced or decided at each stage.

## 

**Component Specification**

+--------+---------------+------------------------------+-------------+
| **S    | **File /      | > **Technique**              | >           |
| tage** | model**       |                              |  **Output** |
+========+===============+==============================+=============+
| Ing    | src/          | > pyxtf parses XTF ping      | > Grayscale |
| estion | xtf_loader.py | > headers (nav, swath data); | > array +   |
|        |               | > images read via OpenCV.    | >           |
|        |               |                              |  navigation |
|        |               |                              | > info      |
+--------+---------------+------------------------------+-------------+
| Input  | src/s         | > Statistical check that the | > Accept /  |
| guard  | onar_guard.py | > input resembles acoustic   | > reject    |
|        |               | > imagery.                   |             |
+--------+---------------+------------------------------+-------------+
| P      | src/pre       | > Nadir masking; row-dropout | > Enhanced  |
| reproc | processing.py | > detection + inpainting;    | > array     |
| essing |               | > median                     |             |
|        |               | >                            |             |
|        |               | > \+ non-local-means         |             |
|        |               | > denoise; CLAHE; canonical  |             |
|        |               | > resize.                    |             |
+--------+---------------+------------------------------+-------------+
| Ba     | models/yolo_  | > YOLO11-Nano (\~2.6M        | > Boxes +   |
| seline | sonar_best.pt | > params, \~5 MB). Classes:  | > scores    |
| de     |               | > debris_net, pipe_cylinder, |             |
| tector |               | > shipwreck_debris.          |             |
|        |               | > imgsz=640.                 |             |
+--------+---------------+------------------------------+-------------+
| Shi    | models/yolo_s | > Fine-tuned on              | > shipwreck |
| pwreck | hipwreck_ai4s | > AI4Shipwrecks (tiles 1024  | > boxes     |
| de     | hipwrecks.pt  | > px, 25% overlap,           |             |
| tector |               | > union-mask YOLO boxes).    |             |
+--------+---------------+------------------------------+-------------+
| A      | src/au        | > 4-layer conv autoencoder;  | > N         |
| nomaly | toencoder.py, | > reconstruction error on    | ovel-object |
| scorer | models/a      | > grid cells YOLO did not    | > boxes     |
|        | utoencoder.pt | > claim; per-image robust    |             |
|        |               | > median/MAD z-score         |             |
|        |               | > threshold.                 |             |
+--------+---------------+------------------------------+-------------+
| Tiling | src/detectio  | > Overlapping 1024 px        | > Unified   |
|        | n_pipeline.py | > windows, remap to source   | > box list  |
|        |               | > coordinates, heuristic     |             |
|        |               | > duplicate merge; clusters  |             |
|        |               | > of strong hits on large    |             |
|        |               | > edge-rich structures       |             |
|        |               | > create shipwreck_candidate |             |
|        |               | > records with               |             |
|        |               | > evidence_count.            |             |
+--------+---------------+------------------------------+-------------+
| Fu     | src/detectio  | > Edge density, aspect ratio | > Scored    |
| sion + | n_pipeline.py | > and local contrast         | >           |
| filter |               | > discount likely            |  detections |
|        |               | > rock/shadow false          |             |
|        |               | > positives; final 0-100%    |             |
|        |               | > score.                     |             |
+--------+---------------+------------------------------+-------------+
| Q      | src/detecti   | > Transparent quality_score  | > Ranked    |
| uality | on_quality.py | > / quality_tier from        | >           |
| layer  |               | > persistence, confidence    |  detections |
|        |               | > stability, spatial         |             |
|        |               | > consistency. Does not      |             |
|        |               | > change model confidence.   |             |
+--------+---------------+------------------------------+-------------+
| Geot   | src/          | > pixel_to_geo: ping index   | > lat/lon   |
| agging | geotagging.py | > gives along-track, pixel   | > per       |
|        |               | > column gives across-track; | > detection |
|        |               | > flat-earth, constant swath |             |
|        |               | > width.                     |             |
|        |               | >                            |             |
|        |               | > Sources: nav CSV, XTF      |             |
|        |               | > headers, or synthetic      |             |
|        |               | > straight track.            |             |
+--------+---------------+------------------------------+-------------+
| Rep    | src/          | > Serializes detections and  | > JSON +    |
| orting | geotagging.py | > quality fields.            | > CSV       |
+--------+---------------+------------------------------+-------------+
| Das    | app.py,       | > Streamlit UI, Folium map,  | >           |
| hboard | src/          | > 3-column HUD layout,       | Interactive |
|        | aura_theme.py | > styled detection cards.    | > review    |
+--------+---------------+------------------------------+-------------+

### Measured results (bundled weights)

  --------------------------------------------------------------------------------------------------------------------------------
  **Component**        **Metric**                                     **Value**       **Evaluated on**
  -------------------- ---------------------------------------------- --------------- --------------------------------------------
  Debris YOLO11-Nano   mAP50 / mAP50-95                               0.993 / 0.840   180 held-out synthetic images, 481 objects

  Debris YOLO11-Nano   Precision / Recall                             0.984 / 0.991   same held-out set

  CNN autoencoder      AUROC (normal vs object)                       1.00            held-out normal patches vs object patches

  Shipwreck YOLO       See reports/ai4shipwrecks_test_m etrics.json   Modest          held-out real sites; improving baseline
  --------------------------------------------------------------------------------------------------------------------------------

These are synthetic-data numbers for the debris detector and should not be read as survey-ready accuracy

**Training and Improvement Workflow**

The debris detector is improved by a repeated \'train until best\' loop (tools/train_until_best.py). Its key safeguard is a fixed held-out set that is never trained on, because the original 0.93 mAP50 was measured on data from the same generation run as training and fell to 0.092 on genuinely held-out data.

![](marine_marine_media/media/marine_media/media/image9.png){width="0.22916666666666666in" height="0.1111111111111111in"}![](marine_marine_media/media/marine_media/media/image9.png){width="0.22916666666666666in" height="0.1111111111111111in"}![](marine_marine_media/media/marine_media/media/image9.png){width="0.22916666666666666in" height="0.1111111111111111in"}

  -------------------------------------------------------------------------------------
  **Run**              **mAP50**            **mAP50-95**   **Precision**   **Recall**
  -------------------- -------------------- -------------- --------------- ------------
  Original weights     0.092                0.032          0.162           0.184

  Round 1              0.904                0.468          0.772           0.832

  Round 2              0.985                0.703          0.970           0.960

  Round 3              0.991                0.794          0.977           0.980

  Round 4 (champion)   0.993                0.840          0.984           0.991

  Round 5              rejected (plateau)   \-             \-              \-
  -------------------------------------------------------------------------------------

### Real-data path (AI4Shipwrecks)

prepare_ai4shipwrecks.py tiles the sonar mosaics and converts binary masks to YOLO boxes using union-mask boxes (avoids fragmented connected-component labels). train_ai4shipwrecks.py then fine-tunes from the debris weights (12 epochs, imgsz 512, backbone partly frozen). The dataset holds shipwreck masks only, so it cannot train a ghost_net class.

### Autoencoder training

train_autoencoder_until_best.py holds out normal patches, computes AUROC of reconstruction error each epoch, keeps the best epoch and early-stops.

**Commands to reproduce**

**Known limitations**

-   **Synthetic training data:** the debris model is a proof of concept and can produce false positives on real sonar texture.

-   **Shipwreck model:** real-data trained, but held-out-site metrics are modest; it needs more sites and threshold calibration.

-   **Autoencoder threshold:** per-image adaptive heuristic (ANOMALY_Z_THRESHOLD); validate on more real surveys.

-   **Geotagging:** flat-earth, constant swath width; production use needs slant-range correction and roll/pitch compensation.

-   **Tiling:** costs CPU time on very long strips, and duplicate merging is heuristic.

-   **Optical mode:** triage aid only; fine-tune on TACO, UAVVaste, DUO or TrashCan for production

**[INNOVATION]{.underline}**

Abyssal Scan's innovation is its **detection-to-recovery workflow**, which converts side-scan-sonar imagery into practical, recovery-ready information.

-   **AI-assisted sonar detection:** Identifies possible nets, traps, ropes and other marine debris in large sonar datasets.

-   **Risk-weighted hotspot mapping:** Combines target location, object type, confidence, ecological risk and recovery accessibility to show where intervention is most urgent.

-   **Persistent object fingerprinting:** Gives every detection a unique record based on its shape, size, acoustic signature, location and survey date, enabling tracking across repeated surveys.

-   **Human-in-the-loop validation:** Allows experts to confirm, reject or correct AI detections, improving reliability in complex sonar environments.

-   **Prioritised recovery list:** Converts raw detections into a ranked list with coordinates and recovery information, helping teams focus on the most harmful and recoverable targets.

-   **Detection-to-recycling connection:** Links confirmed underwater targets with recovery teams and Tamil Nadu's fishnet collection and recycling network.

**Abyssal Scan does not stop at detecting debris; it connects detection, validation, prioritisation, recovery and recycling in one system.**

**[IMPLEMENTATION PLAN]{.underline}**

Abyssal Scan will be implemented in six stages, beginning with data preparation and ending with field validation and recovery integration.

## Phase 1: Data Collection and Preparation

-   Collect side-scan-sonar imagery from available surveys, research partners or public datasets.

-   Gather related metadata, including GPS coordinates, depth, sonar range, survey date and seabed conditions.

-   Define target classes such as nets, traps, ropes, debris and unknown objects.

-   Remove unusable images and standardise the remaining data.

-   Divide the dataset into training, validation and testing sets.

## Phase 2: Image Processing and Annotation

-   Apply noise reduction and contrast enhancement.

-   Separate sonar channels or survey sections where required.

-   Divide large sonar images into smaller analysis tiles.

-   Mark target boundaries using bounding boxes or segmentation masks.

-   Label confirmed targets and difficult non-target objects such as rocks and seabed formations.

## Phase 3: AI Model Development

-   Train or fine-tune an object-detection model using the annotated sonar dataset.

-   Test models such as YOLO or segmentation networks for identifying irregular objects such as nets.

-   Use image augmentation to improve performance across different seabed types and sonar conditions.

-   Generate confidence scores for each predicted detection.

-   Compare the AI results with expert annotations.

## Phase 4: Human Validation and Target Records

-   Develop a review interface showing the original sonar image and AI detections.

-   Allow reviewers to confirm, reject, edit or recategorise each target.

-   Record reviewer corrections for future model improvement.

-   Assign each confirmed object a persistent fingerprint using its shape, size, acoustic pattern and location.

-   Store each target in a structured database.

## 

## Phase 5: Risk Mapping and Recovery Prioritisation

-   Georeference each validated target using GPS and survey metadata.

-   Calculate a priority score using detection confidence, object type, estimated size, ecological risk and recovery accessibility.

-   Generate a risk-weighted debris heatmap.

-   Produce a ranked recovery list with target coordinates, object details and review status.

-   Export target data in suitable formats such as CSV, GeoJSON or shapefile.

## Phase 6: Field Validation and Recovery Integration

-   Share high-priority target coordinates with survey, diving, ROV or recovery teams.

-   Verify selected targets through field inspection or physical recovery.

-   Record whether each target was confirmed, recovered, relocated or unresolved.

-   Measure the quantity of recovered material.

-   Transfer recovered nets to appropriate collection or recycling centres.

-   Conduct repeat surveys to evaluate whether hotspots and target numbers have decreased.

## Evaluation Plan

The prototype will be evaluated using both technical and operational measures:

-   Precision, recall, F1-score and mAP for AI detection.

-   False-positive and missed-detection rates.

-   Time required to review sonar imagery with and without AI support.

-   Accuracy of target coordinates.

-   Agreement between AI-assisted results and expert review.

-   Percentage of prioritised targets confirmed in the field.

-   Number and weight of debris items recovered.

-   Percentage of recovered material sent for recycling.

**Proposed Timeline**

  -----------------------------------------------------------------------------------
  **Stage**          **Main output**
  ------------------ ----------------------------------------------------------------
  **Weeks 1--2**     Data collection, cleaning and target-class definition

  **Weeks 3--4**     Image annotation and preprocessing pipeline

  **Weeks 5--6**     AI model training and initial evaluation

  **Weeks 7--8**     Human-review interface and object database

  **Weeks 9--10**    Risk scoring, heatmap and recovery-list generation

  **Weeks 11--12**   Field validation, performance analysis and final demonstration
  -----------------------------------------------------------------------------------

## Implementation Outcome

The final prototype will provide a complete workflow:

**Sonar data → AI detection → Human validation → Object fingerprint → Risk score → Heatmap → Recovery list → Field verification → Recycling and follow-up monitoring**

The first version will focus on post-survey sonar analysis. Real-time processing, larger-scale integration and automated alerts can be developed in later phases after the model has been validated on local coastal data.

**[EVALUATION METHODOLOGY]{.underline}**

Abyssal Scan will be evaluated at three levels: **AI accuracy, operational efficiency and recovery effectiveness**.

## 1. Dataset and Model Testing

A labelled side-scan-sonar dataset will be divided into training, validation and test sets. The test set will contain unseen imagery and, where possible, data from different locations and seabed conditions.

The model will be assessed using:

-   **Precision:** Correctness of predicted detections.

-   **Recall:** Percentage of real targets detected.

-   **F1-score:** Balance between precision and recall.

-   **IoU:** Overlap between predicted and actual target boundaries.

-   **mAP:** Overall object-detection performance across classes.

These are standard object-detection metrics. [[Ultralyticsdocs.ultralytics]{.underline}](https://docs.ultralytics.com/guides/yolo-performance-metrics)

## 2. Error Analysis

Errors will be classified as:

-   False positives, such as rocks mistaken for debris.

-   False negatives, where real debris is missed.

-   Incorrect target categories.

-   Inaccurate target boundaries or locations.

Performance will be compared across target types, seabed conditions, image quality, object size and survey conditions.

## 3. Human-Review Comparison

AI-assisted review will be compared with manual review by measuring:

-   Total review time.

-   Number of detected targets.

-   Missed detections.

-   False positives.

-   Reviewer agreement.

-   Number of AI predictions accepted or corrected.

The goal is to determine whether AI can reduce review time while maintaining high recall for important debris.

## 4. Risk and Mapping Evaluation

Experts will compare the automated priority rankings with their own assessment of target risk. The system will also be evaluated for:

-   Accuracy of target coordinates.

-   Agreement between automated and expert rankings.

-   Percentage of high-risk targets placed in the top-priority group.

-   Usefulness of heatmaps and recovery lists.

## 5. Field Validation

Selected targets will be verified using repeat sonar surveys, divers, ROVs or recovery teams. Each target will be classified as confirmed debris, non-debris, unresolved or recovered.

The project will record:

-   Targets successfully confirmed.

-   Targets recovered.

-   Weight of debris removed.

-   Percentage sent for recycling.

-   Reduction in high-risk hotspots.

## 6. Success Criteria

Abyssal Scan will be considered successful if it:

-   Detects debris with acceptable precision and recall.

-   Reduces manual review time.

-   Produces accurate target coordinates.

-   Generates useful risk-ranked recovery lists.

-   Reduces false positives through human validation.

-   Supports successful field confirmation and recovery.

Benchmark performance will be reported separately from local field performance because results from external datasets do not automatically represent performance in Indian coastal conditions.

**[BUSINESS AND ADOPTION MODEL]{.underline}**

Abyssal Scan will follow a **B2G/B2B service model**, working with government agencies, conservation organisations and marine-survey companies that already conduct coastal monitoring or recovery operations.

## Target Users and Customers

Potential users include:

-   State fisheries departments.

-   Tamil Nadu Pollution Control Board.

-   Tamil Nadu Green Climate Company.

-   Port and harbour authorities.

-   Marine-conservation NGOs.

-   Hydrographic and marine-survey firms.

-   Research institutions.

-   Fishing cooperatives.

-   Fishnet collection and recycling organisations.

These organisations may need to locate submerged debris, prioritise recovery activities, monitor fishing grounds or measure the results of cleanup programmes.

## Value Offered

Abyssal Scan provides:

-   Faster processing of large sonar datasets.

-   Reduced manual review workload.

-   Georeferenced debris locations.

-   Risk-ranked recovery targets.

-   Hotspot maps for planning.

-   Persistent records for repeat surveys.

-   Reports showing recovery and recycling outcomes.

The primary value is not only detecting debris but helping organisations decide **where to act first**.

## 

## Possible Business Models

## 1. Sonar-analysis service

Survey organisations or government agencies submit sonar data and receive:

-   AI-processed imagery.

-   Validated target records.

-   Risk-weighted maps.

-   Recovery-priority lists.

-   GIS exports.

## 2. Annual monitoring contract

A coastal authority or NGO pays for regular surveys and receives repeat monitoring reports showing:

-   New debris detections.

-   Remaining targets.

-   Recovered objects.

-   Changes in hotspot locations.

-   Cleanup progress.

## 3. Software licensing

Survey companies or research institutions receive access to the Abyssal Scan platform for a subscription or institutional licence.

## 4. Government or NGO pilot

The initial project can be funded through a marine-conservation grant, government innovation programme or institutional pilot. A successful pilot can later support wider deployment across harbours and coastal districts.

## 5. Recovery-planning partnership

Abyssal Scan can partner with fishing-net collection centres and recovery organisations. The platform identifies potential underwater targets, while partners manage physical recovery, collection and recycling.

## 

## 

## Adoption Pathway

1.  **Prototype:** Demonstrate the system using existing or partner sonar datasets.

2.  **Pilot:** Test the system in one harbour or coastal survey area.

3.  **Validation:** Compare AI results with expert review and field verification.

4.  **Partnership:** Obtain support from a fisheries agency, NGO, port or survey company.

5.  **Expansion:** Connect outputs to Tamil Nadu's fishnet collection network.

6.  **Scale-up:** Extend the platform to additional coastal districts and marine-survey projects.

Tamil Nadu has approved discarded-fishnet collection centres across **14 coastal districts** at a total cost of **₹1.75 crore**, creating a relevant pathway for connecting detected gear with collection and recycling operations. [[TNGCCtngcc.tn.gov]{.underline}](https://www.tngcc.tn.gov.in/notifications-circulars/)

## Financial and Policy Support

India's **₹4,077 crore Deep Ocean Mission** demonstrates national investment in ocean technology and sustainable use of marine resources. This creates a supportive environment for marine-monitoring pilots, research partnerships and blue-technology innovation. [[Ministry of Earth Sciencesmoes.gov]{.underline}](https://www.moes.gov.in/static/uploads/2026/06/3ef583815579d5a48f3b11d0d5119333.pdf)

## Key Performance Indicators

Business and adoption can be measured through:

-   Number of pilot partners.

-   Survey area analysed.

-   Number of paying or supporting organisations.

-   Sonar-review time saved.

-   Number of targets detected and verified.

-   Number of recovery operations supported.

-   Kilograms of debris recovered.

-   Percentage of recovered material recycled.

-   Repeat-survey contracts secured.

## Business Model Statement

Abyssal Scan will begin as a sonar-analysis and recovery-planning service for fisheries agencies, ports, NGOs and marine-survey firms. It will use existing sonar data and open-source software to keep initial deployment costs low. After successful pilot validation, the system can scale through annual monitoring contracts, software licensing and partnerships with coastal recovery and recycling networks.

**[EXECUTIVE SUMMARY]{.underline}**

Abyssal Scan is an AI-powered decision-support system designed to detect abandoned, lost, or discarded fishing gear and other underwater debris from side-scan-sonar imagery. Manual interpretation of large sonar surveys is time-consuming, inconsistent, and vulnerable to missed detections, especially when debris is small, partially buried, or visually similar to natural seabed features

The system processes sonar data through image enhancement, noise reduction, and tile-based analysis to improve the detection of small targets. A trained object-detection model identifies known debris types, while an anomaly-detection model flags unfamiliar objects that may not be represented in the training data. Segmentation tools then estimate the boundaries and approximate dimensions of detected objects.

Each detection is converted into a structured, recovery-ready record containing its approximate location, timestamp, debris category, estimated size, confidence score, and verification status. A human-in-the-loop review process allows marine experts to confirm detections, correct false positives, and label unknown objects. These corrections can be used to improve future model performance.

Abyssal Scan further transforms individual detections into a risk-weighted heatmap and ranked recovery queue. Targets can be prioritised according to confidence, debris type, estimated size, ecological risk, depth, and recovery difficulty. This allows fisheries departments, marine survey teams, divers, ROV operators, and environmental organisations to focus their limited resources on the most urgent and recoverable targets.

The project aims to reduce sonar-review time, improve detection consistency, support safer and more targeted recovery operations, and create traceable data for monitoring marine debris over time. By connecting AI-based detection with expert validation, geospatial mapping, and recovery planning, Abyssal Scan moves beyond simple object recognition and provides an operational pathway from **sonar survey to marine-debris recovery**.

## [CONCLUSION]{.underline}

Abyssal Scan addresses the gap between collecting side-scan-sonar data and taking effective marine-debris recovery action. By combining AI-assisted detection, human validation, persistent object records, risk-based prioritisation and geospatial mapping, the system can make large sonar surveys faster and more useful.

The project is technically feasible because it uses established sonar technology, open-source AI tools and a human-in-the-loop workflow. Its viability is supported by potential users such as fisheries departments, ports, NGOs and marine-survey organisations, as well as Tamil Nadu's existing fishnet collection and recycling network.

Abyssal Scan can contribute to marine-life protection, safer fishing grounds and more efficient cleanup operations. Its success should ultimately be measured through local testing, review-time reduction, detection accuracy, field-confirmed targets, kilograms of debris recovered and the amount of material sent for recycling. The project's long-term goal is to create a scalable system that transforms sonar imagery into measurable environmental action.

**[REFERENCES]{.underline}**

-   Food and Agriculture Organization of the United Nations. (2009). *Ghost nets hurting marine environment*.\
    [[https://www.fao.org/newsroom/detail/Ghost-nets-hurting-marine-environment/en]{.underline}](https://www.fao.org/newsroom/detail/Ghost-nets-hurting-marine-environment/en)

-   World Wide Fund for Nature. (2020). *The most deadly form of marine plastic debris: Abandoned, lost and discarded fishing gear*.\
    [[https://wwfint.awsassets.panda.org/downloads/wwfintl_ghost_gear_report_1.pdf]{.underline}](https://wwfint.awsassets.panda.org/downloads/wwfintl_ghost_gear_report_1.pdf)

-   UNEP. (2019). *Underwater ghost-busting to save Indian coral reefs*.\
    [[https://www.unep.org/news-and-stories/story/underwater-ghost-busting-save-indian-coral-reefs]{.underline}](https://www.unep.org/news-and-stories/story/underwater-ghost-busting-save-indian-coral-reefs)

-   Tamil Nadu Pollution Control Board. (2025). *Tamil Nadu Fishnet Initiative*.\
    [[https://tnpcb.gov.in/PDF/About_Us/projects/TN_Fishnet_Initiatives/TNFishnet2025.pdf]{.underline}](https://tnpcb.gov.in/PDF/About_Us/projects/TN_Fishnet_Initiatives/TNFishnet2025.pdf)

-   Tamil Nadu Green Climate Company. (2025). *Tamil Nadu Fishnet Initiative and coastal collection-centre programme*.\
    [[https://tngcc.tn.gov.in/wp-content/uploads/2025/11/envfor_e_122_ms_2025-FIshnet-2025.pdf]{.underline}](https://tngcc.tn.gov.in/wp-content/uploads/2025/11/envfor_e_122_ms_2025-FIshnet-2025.pdf)

-   Ministry of Earth Sciences, Government of India. (2021--2026). *Deep Ocean Mission*.\
    [[https://www.moes.gov.in/schemes/dom]{.underline}](https://www.moes.gov.in/schemes/dom)

-   Microsoft Research and WWF Germany. (2025). *GhostNetZero: AI for detecting marine ghost nets*.\
    [[https://www.microsoft.com/en-us/research/publication/ghostnetzero-ai-for-detecting-marine-ghost-nets/]{.underline}](https://www.microsoft.com/en-us/research/publication/ghostnetzero-ai-for-detecting-marine-ghost-nets/)

-   Ultralytics. (2023). *YOLO performance metrics: Precision, recall, F1-score, IoU and mAP*.\
    [[https://docs.ultralytics.com/guides/yolo-performance-metrics]{.underline}](https://docs.ultralytics.com/guides/yolo-performance-metrics)
