# CHECK_PHOTO_HELPFUL

## Overview

The query aims to assess whether an issue being reported would benefit from a photo (or video) being supplied.

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
| `Yes`   | A photo or video would be relevant for the issue               |
| `No` | A photo or video is unlikely to be helpful           |
| `Unknown` | It is unknown whether a photo or video would be helpful           |



