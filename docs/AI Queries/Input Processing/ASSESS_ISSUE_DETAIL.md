# ASSESS_ISSUE_DETAIL

## Overview

The query aims to assess whether the user input of an issue is sufficiently detailed to raise a task for.

The subject of the issue report is included (from previous classification) to help inform

## Query Inputs

| **Input**   | **Description**                                     |
| ----------- | --------------------------------------------------- |
| `userInput` | The user input provided earlier in the conversation |
| `subject` | The subject of the issue report |



## Query Outputs

The query should produce one of the following values.

| Output     | **Description**                                     |
| ---------- | --------------------------------------------------- |
| `Yes`   | The input is a complete enough phrase               |
| `No` | Further details are needed           |
| `Unknown` | It is unclear whether the phrase is complete enough           |



