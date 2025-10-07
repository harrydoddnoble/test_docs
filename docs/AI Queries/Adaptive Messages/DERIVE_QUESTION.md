# DERIVE_QUESTION

## Overview

For some assets, there may be specific questions the building managers would want to know in know when raising issues.

These will be captured in a single field on the platform as free text where the managers describe different details they may want to know, for example:

```
If the query relates to toilets, get the cubicle number.

If the problems is to do with a stairwell, identify which corner of the building it is in
```

Both the subject name and the original user input are provided to be used.

The response should either be the question to ask the user or the string `None`

## Query Inputs

| **Input**   | **Description**                                     |
| ----------- | --------------------------------------------------- |
| `userInput` | The user input |
| `subject` | The subject of the current issue being raised |
| `guidance` | Any specific guidance, sourced from Asset record extended metadata* |

_*e.g. interpolation from entity variable in the context_

## Query Outputs

The query should produce one of the following values.

| Output     | **Description**                                     |
| ---------- | --------------------------------------------------- |
| `None` | If there is no question that needs to be asked           |
| Anything else | Question to be asked            |



