# USER_INPUT_FILTER

## Overview

The query aims to pre-filter a user's input utterance before classification to detect whether they are:

- Greeting the assistant (so they have misunderstood the previous message in the conversation!)
- Providing a complete enough utterance to have a strong chance of classification
- Provide a fragment, e.g. mentioning just a room
- Including multiple separate issues in a single utterance

This will allow the conversation to only proceed with classification with good utterances and to take appropriate steps with the user for anything else.

## Query Inputs

| **Input**   | **Description**                                     |
| ----------- | --------------------------------------------------- |
| `userInput` | The user input provided earlier in the conversation |



## Query Outputs

The query should produce one of the following values.

| Output     | **Description**                                     |
| ---------- | --------------------------------------------------- |
| `Single`   | The input is a complete enough phrase               |
| `Fragment` | The input is a fragment or partial phrase           |
| `Multiple` | The input contains multiple issues                  |
| `Greeting` | The input is a standalone greeting to the assistant |



