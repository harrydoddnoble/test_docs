# ASSESS_ISSUE_PRIORITY

## Overview

The query aims to get AI's view of the priority of an issue according to the descriptions in the table below.

Additional guidance may optionally be provided that may inform the prioritisation, for example, that glass cleaning issues should be treated as urgent.

## Query Inputs

| **Input**   | **Description**                                     |
| ----------- | --------------------------------------------------- |
| `userInput` | The user input provided earlier in the conversation |
| `guidance` | [ optional ] Any specific guidance to inform the decision |



## Query Outputs

The query should produce one of the following values.

| Output     | **Description**                                     |
| ---------- | --------------------------------------------------- |
| `Urgent`   | The issue relates to loss of critical services in a building or poses a severe safety or security risk that must be resolved as soon as possible               |
| `High` | The issue relates to the loss or impairment of important services within a building           |
| `Medium` | The issue impacts some services within a building and is causing a moderate level of inconvenience to its occupants                   |
| `Low` | The issue is minor or nice to have |
| `Unknown` | It's not been possible to asset the priority |



