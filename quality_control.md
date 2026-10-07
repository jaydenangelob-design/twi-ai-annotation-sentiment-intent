# Annotation Quality Control

## 1. Purpose

Quality control helps ensure that annotations are accurate, consistent, complete, and reproducible.

This project uses a simple review process to identify labeling errors, ambiguous examples, and inconsistencies.

## 2. Quality Checks

Each dataset review checks:

- Correct sentiment label
- Correct intent label
- Consistent use of annotation definitions
- Correct ambiguity flag
- Clear annotation notes
- Complete dataset fields
- Duplicate or unnecessary examples

## 3. Annotation Consistency

Annotations should follow the definitions in `annotation_guidelines.md`.

Similar messages should receive the same label when their meaning and context are substantially similar.

When two possible labels appear reasonable, the primary intent should be selected based on the main purpose of the message.

## 4. Ambiguous Examples

Ambiguous examples receive additional attention during review.

The reviewer should:

1. Read the complete text.
2. Identify the most likely interpretation.
3. Compare the example against the annotation guidelines.
4. Check whether the ambiguity flag is appropriate.
5. Confirm that the annotation note explains the decision.

## 5. Error Review

Potential annotation errors include:

- Incorrect sentiment classification
- Incorrect intent classification
- Missing ambiguity flags
- Unsupported assumptions
- Inconsistent labeling
- Missing or malformed fields

Errors should be corrected before the dataset is considered complete.

## 6. Sampling Review

A quality-control review can examine a sample of dataset rows rather than relying only on the original annotation pass.

The review should focus especially on:

- Ambiguous examples
- Examples with multiple possible intents
- Examples containing code-switching
- Examples with mixed sentiment
- Examples that were difficult to classify

## 7. Quality-Control Checklist

Before finalizing the dataset:

- [ ] Every row has an ID.
- [ ] Every row contains text.
- [ ] Every row has a sentiment label.
- [ ] Every row has an intent label.
- [ ] Ambiguous examples are identified.
- [ ] Annotation notes are clear where needed.
- [ ] Labels follow the annotation guidelines.
- [ ] No private or personally identifying information is included.
- [ ] The dataset is clearly identified as portfolio/synthetic data.

## 8. Review Outcome

The objective of quality control is not simply to increase the number of labeled examples.

The objective is to produce annotations that are:

- Accurate
- Consistent
- Explainable
- Reproducible
- Suitable for demonstrating an AI data annotation workflow

## 9. Portfolio Scope

This repository is a small portfolio demonstration rather than a production dataset.

The quality-control process is included to demonstrate an understanding of how annotation accuracy and consistency can be evaluated before data is used in an AI workflow.
