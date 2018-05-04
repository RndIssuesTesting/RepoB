---
name: Archer_issues_template
about: Describe this issue template's purpose here.

---

# Choose your own adventure - IVD style

Directions:

1. Pick what issue you have
    - General Issue / Bug
    - New or Improved Feature / Design
    - Failing Verification or Validation
    - Sprint Open
    - Sprint Close
    
2. Remove the other issue templates and this header section
3. Fill out the requested information

------------------------------------

## General Issue / Bug

#### Description of the Issue

1. The problem
1. Impact on the IVD 
    - What is the risk of this issue
    - List designs and requirements affected 
1. Data to replicate the issue
    - This MUST be turned into a failing regression test FIRST then fix it 
1. Time line for resolution

#### Definition of Done

 - [ ] The fix is consistent with all affected requirements and designs.
 - [ ] When affected documentation is updated to reflect any changes to design.
 - [ ] All traceability tags are in place and valid.
 - [ ] When the new regression test is passing.
 - [ ] When all other verification for affected designs and requirements is passing.

<Assign github labels for the severity of the issue and the software block that is affected>
------------------------------------

## New Feature / Design 

#### Description of the Feature
1. Overview of the feature 
1. List design and requirement numbers 

#### Definition of Done

 - [ ] The implementation is consistent with design requirements.
 - [ ] All documentation is updated including the Low Level Design.
 - [ ] All traceability tags are in place and valid.
 - [ ] When all other verification for affected designs and requirements is passing.
 - [ ] <Replace this with how the developer will know this feature is complete.  This can be test sets, links to design numbers or a concrete description>

<Assign github labels for the severity of the issue and the software block that is affected>
------------------------------------

## Failing Verification or Validation

#### Description of the Failure
1. Link to the failing test.
1. Version used in the failure.
1. List the design and requirement numbers the test affects.

#### Definition of Done

 - [ ] When all other verification for affected designs and requirements is passing.
 - [ ] When affected documentation is update to reflect any changes to design.

------------------------------------

## Sprint Open

> This checklist comes from http://bldr-ivd-docs01/archerdxinc/ivd-base/dev/docs/development-plan.rst and should be kept up to date

  - [ ] Sprint completion checklist issue created and assigned to sprint, :ref:`Sprint Completion Checklist`.
  - [ ] Backlog items that are chosen for this sprint should be added to the
  sprint milestone.
  - [ ] Additional backlog items are created and assigned to this sprint.
  - [ ] Each backlog item has a definition of DONE.
  - [ ] Each backlog has a list of expected documents to be updated.
  - [ ] Sync the dev branch with last configuration baseline (e.g. pull master onto dev)
  - [ ] Update the version in `config.py`
  - [ ] confirm the DRAFT setting in `config.py` is True
  
------------------------------------

## Sprint Close

> This checklist comes from http://bldr-ivd-docs01/archerdxinc/ivd-base/dev/docs/development-plan.rst and should be kept up to date

  - [ ] All milestone issues are either completed, put back into the backlog or be added to the next sprint.
  - [ ] Each issue opened or closed during the sprint is properly :ref:`traced <traceability>`
    to the appropriate :term:`design element`.
  - [ ] Each issue/pull request that recorded a review is properly tagged and
    traced
  - [ ] Each :term:`design element` that was created or updated has
    accurate and coherent :ref:`traces <traceability>` 
  - [ ] Final versions of all documents for the :term:`DHR` are created in preparation for approval.
  - [ ] Verify tests are passing.
    - [ ] Open tickets for failing verifications
  - [ ] Decide which blocks need to remain in `dev`
  - [ ] Build new baseline
    - [ ] Merge approved `dev` blocks into `master`
    - [ ] Summarize approved changes for Sprint Review document
    - [ ] Tag new baseline
        - [ ] repo tag
   - [ ] Generate PDF version of the baseline documents
   - [ ] Submit Sprint Review document for project owner approval and submission to QS
