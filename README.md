# DVplan_reviewer
Experimenting with DVplan reviews.

The purpose of this repo is to enable experimentation for methods to review
[DV Plans](https://github.com/openhwgroup/core-v-verif/tree/master/docs/VerifPlans#verification-plans)
used by [CORE-V-VERIF](https://github.com/openhwgroup/core-v-core).
The current DV Plans use Excel Spreadsheets which is a good format for writing them, but a poor format for distributed reviews.

## Proposed Review Flow
1. Capture DV Plan using MS Excel, LibreOffice Calc, etc.
2. Write out a CSV file.
3. Translate to yaml using csv2yml.
4. Reviewers provide feedback as pull-requests against the yaml file.
5. Review is complete when all issues and pull-requests against the yaml are closed/merged.
6. Translate to csv and xlsx (script TBD).

## Contents:

**CV32E40S_UserMode.xlsx** : example DV plan.
**CV32E40S_UserMode.csv**  : verison of DV plan in CSV format (somewhat modified from the original).
**csv2yml** : prototype conversion script for step 3.
