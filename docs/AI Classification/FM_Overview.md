# FM Classification Overview

## Classification

For FM classifications, up to three levels of classification are used.

**Request Type** categorises the kind of request a user is raising (e.g. issue, task follow-up etc.) use the `FM_L1` taxonomy.

Depending on the request type selected, the classification may then proceed to categorise the **subject** of the request (e.g. leaking tap, replace filter etc.) using the `FM_L2_IssueRequest` taxonomy.

Depending on the subject identified, a further sub-subject may be categorised using a specific taxonomy for that subject (of the form `FM_L3_xxx`).

## Composed Subject

To aid processing, subject and sub-subject (also referred to as primary and secondary) are merged into a single value of `subjectComposed` that can be used within the DDF to apply conditional logic. The following rules are followed when composing:
* If there is not sub-subject taxonomy for that subject, use that value
* Elif the sub-subject successfully matched, use that value
* Else suffix the subject with `Other` and use that value

A full list of possible values can be found on the corresponding page (TODO - add link once fixed)