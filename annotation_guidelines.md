# Twi Annotation Guidelines

## 1. Purpose

These guidelines define a consistent process for labeling Twi text for sentiment and intent classification.

The goal is to produce clear, consistent, and reproducible annotations that can support AI training and evaluation workflows.

## 2. General Annotation Principles

Annotators should:

- Read the complete text before assigning labels.
- Consider the meaning and context of the entire message.
- Avoid relying on individual words alone.
- Select the label that best represents the primary meaning.
- Avoid making assumptions that are not supported by the text.
- Mark uncertain or ambiguous examples for review.
- Apply the same criteria consistently across the dataset.

## 3. Sentiment Annotation

### Positive

Use **Positive** when the text clearly expresses satisfaction, happiness, approval, appreciation, or another favorable attitude.

### Negative

Use **Negative** when the text expresses dissatisfaction, frustration, anger, disappointment, criticism, or another unfavorable attitude.

### Neutral

Use **Neutral** when the text mainly provides information, asks a question, gives an instruction, or does not clearly express positive or negative emotion.

## 4. Intent Annotation

Assign the intent that best represents the primary purpose of the message.

### Pricing

The user is asking about a product or service price, cost, discount, or payment amount.

### Purchase

The user expresses an intention to buy, order, or obtain a product or service.

### Delivery

The user is asking about delivery, shipping, arrival time, or delivery status.

### Complaint

The user reports a problem, dissatisfaction, failed service, damaged product, or other negative experience requiring attention.

### Information Request

The user is requesting general information about a product, service, process, or organization.

### Feedback

The user provides an opinion, comment, review, suggestion, or evaluation.

### Cancellation

The user wants to cancel an order, booking, subscription, or service.

### Other

Use this label when the primary intent does not reasonably fit the defined categories.

## 5. Ambiguity Handling

Some messages may support more than one interpretation.

When a message is ambiguous:

1. Read the complete message.
2. Identify the most likely intended meaning.
3. Choose the strongest supported label.
4. Record the ambiguity in the annotation notes.
5. Escalate the example for review when the correct label cannot be determined reliably.

Annotators should not invent context that is not present in the text.

## 6. Code-Switching

Twi messages may contain English words or phrases.

Code-switching should not automatically change the language classification of the message.

The annotation should
