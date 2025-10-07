# DERIVE_MESSAGE

## Overview

For some assets, there may be specific information the building managers wish to relay.

These will be captured in a single field on the platform as free text where the managers describe different details they may want to supply, for example:

```
If the query relates to loss of internet connectivity let the user know that we aware of an issue with the ISP.

If the query relates to Legionella testing, let the user know to contact Maria on x6789
```

Both the subject name and the original user input are provided to be used.

The response should either be a single message to send to the user or the string `None`

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
| `None` | If there is no message to be relayed           |
| Anything else | Message to be played to the user            |



