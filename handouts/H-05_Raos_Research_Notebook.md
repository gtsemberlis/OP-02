---
id: H-05
title: Rao's Research Notebook
author: Dr. Ananya Rao
document_type: Research Notebook
audience: Player
related_artifact: A-05
related_scene:
  - Scene 3
appendix: C
status: Canonical
---

Here are the pages of H05



# H-05 — Rao's Research Notebook



## Page 1 of 10



**Research Notebook 4**



A. Rao



Alexandria Aviation Systems



January 2025



---



### Project



Runway Obstruction Detection Validation



Phase III Operational Verification



---



**January 21**



Run 181



Objective:



Verify synchronization stability across all production sensor inputs following deployment update 4.2.



Configuration unchanged from Run 180.



---



Primary Radar



✓ Pass



---



Surface LIDAR



✓ Pass



---



Electro-Optical



✓ Pass



---



Infrared



✓ Pass



---



ADS-B Correlation



✓ Pass



---



Environmental Inputs



✓ Pass



---



Synchronization Drift



0.0038 sec



Within tolerance.



---



Confidence Distribution



Nominal.



No unexpected classifications.



---



Notes



No meaningful deviation from previous operational baseline.



Engineering recommendation remains unchanged.



Continue scheduled verification.



---



**January 23**



Repeat Run 181 using archived environmental conditions.



Results reproduced within expected statistical variance.



---



Reminder:



Request Kevin review timestamp normalization before Phase IV.



No concerns expected.



---



Margin Note



Need cleaner visualization for confidence decay.



Current graphs encourage over-interpretation.



Observation ≠ explanation.



Keep those separate.



---



Bottom of Page



Meeting Friday:



* Kevin

* Ethan

* QA Review



Bring calibration plots.



Do not include speculative commentary.



# H-05 — Rao's Research Notebook



## Page 2 of 10



**February 3**



Run 184



Objective:



Post-deployment validation using live operational capture from ORD.



Routine verification only.



---



### Sensor Status



Primary Radar



✓ Pass







Surface LIDAR



✓ Pass



Electro-Optical



⚠ Review Required



Infrared



✓ Pass



ADS-B



✓ Pass



Environmental



✓ Pass



---



### Observation



Unexpected confidence spike during final approach.



Duration:



2.8 seconds



Automatic classification discarded after post-processing.



---



### Initial Assessment



Most likely causes:



□ Camera synchronization



□ Lens contamination



□ Compression artifact



□ Timestamp offset



□ Environmental reflection



---



Repeat using raw optical feed.



Do **not** review processed visualization first.



Avoid confirmation bias.



---



**February 4**



Repeated using archived raw imagery.



No evidence of:



* compression error

* dropped frames

* timestamp drift



Camera calibration verified.



Optical confidence remains elevated.



---



Margin Calculation



Correlation coefficient remains unusually high.



Need independent verification before discussing with anyone outside Engineering.



---



Question



Why does only optical disagree?



Investigate wavelength filtering before continuing.



Assume instrumentation error until proven otherwise.



---



Bottom of Page



Reminder:



Ask Kevin whether calibration changed after maintenance window.



Check maintenance logs before opening QA ticket.



---



Margin Note (written later)



Maintenance confirmed.



No changes.



Strike calibration hypothesis.



→ Return to raw data.





# H-05 — Rao's Research Notebook



## Page 3 of 10



**February 7**



Run 187



Objective:



Determine source of elevated optical confidence.



Repeat using independent validation sequence.



No changes to production model.



---



### Hypothesis Log



**H-01 — Camera Calibration**



**Rejected**



Calibration confirmed by Engineering.



Independent test within specification.



---



**H-02 — Lens Contamination**



**Rejected**



Manual inspection completed.



No optical defects identified.



---



**H-03 — Image Compression Artifact**



**Rejected**



Raw sensor feed reproduces identical observation.



---



**H-04 — Environmental Reflection**



**Rejected**



Unable to reproduce under simulated lighting conditions.



---



**H-05 — Software Regression**



**Rejected**



Previous production build produces identical result.



---



### Observation



None of the rejected hypotheses explain the observed confidence value.



Continue assuming measurement error.



Unknown source.



---



### Independent Review



Requested second analysis from Kevin.



Do not discuss current working assumptions.



Only provide datasets.



---



Margin Note



Blind review preferable.



Need independent interpretation before continuing.



---



**February 8**



Kevin reproduced confidence values.



No discussion beforehand.



Agreement within expected tolerance.



---



Question



If independent analysis reproduces the same observation...



...what exactly is being reproduced?



---



Margin Calculation



Correlation remains statistically significant.



Still insufficient to conclude anything beyond repeatability.



---



Bottom of Page



Reminder to self:



Do **not** become attached to the anomaly.



Become attached to the process.


# H-05 — Rao's Research Notebook

## Page 4 of 10

**February 12**

Objective:

Review archived operational detections using current validation pipeline.

Question:

Is ORD unique?

---

Archive Query

Parameters:

* Confidence ≥ 0.90
* Runway environment
* Multi-modal agreement
* No confirmed obstruction

---

Results

Returned more records than expected.

---

### Initial Review

Chicago (ORD)

Confirmed.

---

Alaska

Similar profile.

Weather substantially different.

---

Atlantic Crossing

Brief detection.

Insufficient duration.

Requires review.

---

Military Airfield

Access restricted.

Metadata only.

Confidence comparable.

---

Second Military Airfield

Similar.

Unable to access raw sensor package.

---

Third Military Airfield

Incomplete archive.

Possible match.

---

Margin Note

These are not duplicates.

Different airports.

Different equipment.

Different weather.

Different personnel.

---

Question

Common failure mode?

---

Review

Software versions differ.

Sensor manufacturers differ.

Environmental conditions differ.

Geographic locations differ.

Operational procedures differ.

---

Nothing obvious shared.

---

**February 13**

Repeated archive search using previous production model.

Same events returned.

---

Repeated using current validation build.

Same events returned.

---

Repeated using manually reconstructed confidence calculations.

Same events returned.

---

Margin Note (boxed)

If independent systems,

independent software,

independent locations,

and independent personnel

produce the same observation...

what exactly is independent?

---

Bottom of Page

Do not discuss outside Engineering until archive review is complete.

Need more evidence.

Not fewer questions.

# H-05 — Rao's Research Notebook

## Page 5 of 10

**February 18**

Working Principle

Current observations remain internally consistent.

Consistency is **not** explanation.

Need experiment capable of falsifying present assumptions.

---

### Objective

Design a test that should **fail** if the current interpretation is incorrect.

If the interpretation survives, confidence may increase.

If it fails, return to baseline assumptions.

Either result is acceptable.

---

### Candidate Experiments

□ Artificial sensor noise

Expected Result:

Confidence should decrease.

---

□ Randomized timestamp offsets

Expected Result:

Correlation should collapse.

---

□ Independent processing pipeline

Expected Result:

Different implementation should produce different classifications.

---

□ Blind engineering review

Expected Result:

Independent analyst reaches different conclusion.

---

□ Archived data reconstruction

Expected Result:

Unable to reproduce historical observations.

---

### Results

Artificial sensor noise

✓ Expected

Confidence decreased.

---

Timestamp offsets

✓ Expected

Correlation failed.

---

Independent processing pipeline

Unexpected.

Independent implementation reproduced identical detections.

Repeat.

---

Blind engineering review

Unexpected.

Kevin identified the same archive events without prior discussion.

Repeat.

---

Archive reconstruction

Unexpected.

Historical detections reproduced.

Repeat.

---

Margin Note

Unexpected results require repetition.

Not interpretation.

---

Question

How many independent reproductions are sufficient before the burden of proof changes?

---

Later Entry (different pen)

Dangerous question.

Burden of proof never changes.

Only the evidence changes.

---

Bottom of Page

Continue assuming error.

Simply identify a different error.

If one exists.

# H-05 — Rao's Research Notebook

## Page 6 of 10

**February 24**

Archive review complete.

Engineering review complete.

Quality Assurance review complete.

No procedural deficiencies identified.

---

### Current Position

The observations remain reproducible.

The observations remain measurable.

The observations remain unexplained.

Those are three separate statements.

Do not combine them.

---

### Working Assumptions

Assumption:

The system is detecting an object that does not exist.

Status:

Unsupported.

---

Assumption:

The object exists exactly as represented.

Status:

Unsupported.

---

Assumption:

The observations correspond to a measurable external phenomenon.

Status:

Consistent with current evidence.

Requires additional testing.

---

Margin Note

Need to stop asking:

> *"What is being detected?"*

Better question:

> *"What do the observations actually establish?"*

---

### Established Observations

Independent sensors agree.

Observations are repeatable.

Historical examples exist.

Environmental conditions vary.

No common hardware failure identified.

No common software failure identified.

No common operator error identified.

---

### Observations Not Established

Nature of observed phenomenon.

Mechanism.

Duration.

Behavior.

Origin.

Relationship to visual perception.

---

Bottom Margin

Evidence is becoming more precise.

My language should become more precise as well.

---

**February 25**

Removed "object" from working documentation.

Replacing with:

**phenomenon**

Reason:

The former implies an interpretation.

The latter describes an observation.

---

Margin Note (circled)

Words matter.

Do not let vocabulary become evidence.


# H-05 — Rao's Research Notebook

## Page 7 of 10

**March 1**

No experiments today.

Reviewed previous notebook entries.

Read from beginning.

---

Observation:

Every experiment has assumed the instrumentation requires explanation.

None have examined the observer.

---

Question

When did I decide the sensors were unusual?

---

Review

Radar reports measurable return.

LIDAR reports measurable return.

Infrared reports measurable return.

Optical reports measurable return.

Independent systems agree.

---

Question

Why is visual observation considered the baseline?

---

Margin Note

Habit is not evidence.

---

Halfway Down the Page

Current assumptions:

✓ The sensors agree.

✓ The observations repeat.

✓ Historical examples exist.

✓ Conventional explanations remain unsupported.

---

Current assumptions **not** supported:

□ The sensors are incorrect.

□ Human perception is complete.

□ Absence of visual confirmation disproves observation.

---

Large Blank Space

(Several inches of empty paper.)

---

Near Bottom of Page

Perhaps the question has always been backwards.

We continue asking:

> *Why do the sensors detect something?*

Perhaps we should ask:

> *Why don't we?*

---

Final Entry

No experiment proposed.

Need to think before designing the next one.

# H-05 — Rao's Research Notebook

## Page 8 of 10

**March 4**

Working Hypothesis

The observations are not increasing.

Our ability to detect them may be.

---

Immediate objections:

How?

No mechanism identified.

No supporting literature.

No predictive model.

No biological explanation.

No experimental verification.

---

Conclusion

Hypothesis remains speculative.

Do not incorporate into working documentation.

---

Margin Note

A useful hypothesis is not the same as a correct hypothesis.

---

### Thought Experiment

Assume, for the moment, that the observations are accurate.

Question:

Would the existing evidence appear different?

---

Review

Historical detections

Still consistent.

---

Independent engineering review

Still consistent.

---

Sensor agreement

Still consistent.

---

Witness timelines

Still consistent.

---

Question

Interesting.

Nothing changes.

---

Margin Note

The hypothesis explains the observations.

That does **not** make it true.

---

Lower Half of Page

Need an experiment capable of distinguishing between:

A.

Instrumentation is producing false observations.

or

B.

Instrumentation is extending observation beyond ordinary human perception.

Current evidence does not discriminate.

---

Bottom of Page

No publication.

No presentation.

Need decisive experiment.

Everything else is philosophy.

# H-05 — Rao's Research Notebook

## Page 9 of 10

**March 7**

Current Position

The evidence now supports continued investigation.

The evidence does **not** support public conclusions.

Maintain that distinction.

---

### Before Any Publication

The following must occur:

□ Independent replication outside Alexandria

□ External engineering review

□ Controlled experimental observation

□ Statistical review

□ Methodology audit

□ Ethical review

---

If any item fails:

Return to baseline.

---

Question

Who should evaluate work that challenges the assumptions of the evaluator?

No answer.

---

### Risk Assessment

Risk of publication before sufficient evidence:

High.

---

Risk of suppressing reproducible observations:

Also high.

---

Neither outcome is acceptable.

Need better evidence.

---

Margin Note

The responsible decision is rarely the comfortable one.

---

Lower Half of Page

Reminder:

Engineering establishes observations.

Society decides what to do with them.

Those are different responsibilities.

---

Meeting Notes

Discuss with Ethan.

Discuss with Kevin.

Do **not** seek agreement.

Seek criticism.

---

Bottom Margin

If every reviewer agrees immediately,

I have probably explained it poorly—

or tested it insufficiently.

# H-05 — Rao's Research Notebook

## Page 10 of 10

**March 9**

Final Review Before Presentation

Read notebook in full.

No corrections to methodology.

Several corrections to language.

Evidence remains stronger than interpretation.

Maintain that order.

---

### Established

Independent observations agree.

The observations are reproducible.

Historical examples exist.

Conventional engineering explanations remain unsupported.

Current instrumentation appears to be functioning as designed.

These statements are supported by evidence.

---

### Not Established

Nature of the phenomenon.

Mechanism.

Origin.

Intent.

Biological significance.

Long-term implications.

These statements require evidence that does not yet exist.

Do not imply otherwise.

---

### Recommendation

Present observations.

Present methodology.

Present uncertainty.

Do not present conclusions that cannot yet survive independent review.

---

Margin Note

There is a temptation to make the evidence more exciting.

Resist it.

The evidence is sufficient.

---

Lower Half of Page

Question

If these observations survive independent review...

they cease to belong to Alexandria.

They become part of humanity's understanding of the world.

That carries responsibilities beyond engineering.

---

Final Entry

The data deserve publication.

The conclusions do not.

Not yet.

---

Signed,

**A. Rao**

**March 9**

---

Inside Back Cover (written in pencil)

If someone else is reading this notebook,

begin where I began.

Assume I am mistaken.

Repeat everything.

Trust only what you can reproduce.

If, after that,

you arrive here as well—

we should continue the work together.



