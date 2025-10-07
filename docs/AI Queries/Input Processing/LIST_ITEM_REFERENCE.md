# LIST_ITEM_REFERENCE

## Overview

This query aims to identify if an item in a provided list of strings is mentioned in a users input.
This is a fairly basic function, think string match rather than a more 'clever' inference.

## Query Inputs

| **Input**   | **Description**                                     |
| ----------- | --------------------------------------------------- |
| `userInput` | The user input provided earlier in the conversation |
| `list`      | An array of items                                   |



## Query Outputs

The query should produce one of the following values.

| Output     | **Description**                                        |
| ---------- | -------------------------------------------------------|
| `<string>`   | The verbatim string value of the identified list item|
| `None` | No items in the list were matched                          |



