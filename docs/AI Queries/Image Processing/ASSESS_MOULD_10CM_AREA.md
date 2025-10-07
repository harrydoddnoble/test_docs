# ASSESS_MOULD_10CM_AREA

## Overview

The query aims to assess a user provided image for:
- Does the image depict an area of mould larger or smaller than 10cm across.

## Query Inputs

| **Input**   | **Description**                                     |
| ----------- | --------------------------------------------------- |
| `userInput` | The user image reference provided earlier in the conversation |


The query should produce one of the following values.

| Output     | **Description**                                     |
| ---------- | --------------------------------------------------- |
| `Larger`   | The affected area appears to be larger than 10cm     |
| `Smaller`  | The affected area appears to be smaller than 10cm    |
| `Unknown`  | The model is unable to determine the appropriate answer |

