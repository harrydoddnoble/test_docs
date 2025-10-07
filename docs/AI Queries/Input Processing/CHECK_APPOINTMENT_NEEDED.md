# CHECK_APPOINTMENT_NEEDED

## Overview

The query aims to assess whether an issue being reported is something for which an appointment is likely to be required as it is a future piece of work, e.g. request to paint a wall, hang a picture, escort a visitor or move between offices

The subject of the issue report is included (from previous classification) to help inform AI.

## Query Inputs

| **Input**   | **Description**                                     |
| ----------- | --------------------------------------------------- |
| `userInput` | The user input provided earlier in the conversation |
| `subject` | The subject of the issue report |



## Query Outputs

The query should produce one of the following values.

| Output     | **Description**                                     |
| ---------- | --------------------------------------------------- |
| `Yes`   | An appointment would be relevant for the issue               |
| `No` | An appointment is unlikely to be needed           |
| `Unknown` | It is unknown whether an appointment would be needed           |



