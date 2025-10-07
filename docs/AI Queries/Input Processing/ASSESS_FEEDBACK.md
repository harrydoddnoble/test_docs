# ASSESS_FEEDBACK

## Overview

The query aims to assess whether the user provided feedback is:
* Praise - positive feedback
* Complaint - explicit complaint or negative feedback
* Suggestion - suggestion for improvement

## Query Inputs

| **Input**   | **Description**                                     |
| ----------- | --------------------------------------------------- |
| `userInput` | The user input provided earlier in the conversation |


## Query Outputs

The query should produce one of the following values.

| Output     | **Description**                                     |
| ---------- | --------------------------------------------------- |
| `Praise`   | Positive feedback, praise               |
| `Complaint` | Complaint of negative feedback          |
| `Suggestion` | Suggestion for improvement           |
| `Unknown` | Unclear           |



