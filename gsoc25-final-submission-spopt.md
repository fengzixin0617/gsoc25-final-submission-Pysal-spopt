# GSOC25-final-submission - Flow Refuelling Location Model 

## Summary
1. Fork the repo (pysal-spopt) and create a dev branch [add-frlm-feature](https://github.com/fengzixin0617/spopt/tree/add-frlm-feature)
2. [Pull request](https://github.com/pysal/spopt/pull/487)
3. Create a set of [Flow Refuelling Location Models](https://github.com/fengzixin0617/spopt/blob/add-frlm-feature/spopt/locate/flow.py)
4. Create a corresponding [notebook for the models](https://github.com/fengzixin0617/spopt/blob/add-frlm-feature/notebooks/flow.ipynb)
5. Create code [test](https://github.com/fengzixin0617/spopt/blob/add-frlm-feature/spopt/tests/test_locate/test_flow.py)
6. Document the learning process with [blogs](https://fengzixin0617.github.io/gsoc2025/) 

## Task 0.
Before starting the project, I reviewed academic papers on Flow Refuelling Location Models (FRLM), as these models are closely related to my PhD research. At that time, I was new to software engineering practices, including object-oriented programming (OOP) and collaborative workflows such as GitHub’s push/pull/fork process. My initial tasks therefore focused on becoming familiar with these tools and practices.

## Initial draft of the basic FRLM model. 
I began by developing an initial draft of the basic Flow Refuelling Location Model (FRLM). I then extended this draft by incorporating the threshold-based version of the model, followed by the capacitated version. After I gained a better understanding of OOP, I refactored the code into an object-oriented structure.

Each of the three models can be solved using either Exact solver or Greedy solver. 

## Code review and revision. 

I then submitted my first [Pull Request](https://github.com/pysal/spopt/pull/487), which went through rounds of code review by my mentors. 

## Notebook. 

After two rounds of code review and revisions, I created a notebook with real-world examples demonstrating the models included in the package. It documents the details of the three optimisation models, ways to prepare the input data, and the API for solving an optimisation problem. The notebook also shows how to retrieve relevant statistics and results.

## Test. 

The next step was to develop a [test](https://github.com/fengzixin0617/spopt/blob/add-frlm-feature/spopt/tests/test_locate/test_flow.py) file for the newly implemented module.

## Pre-commit 

Finally, I set up pre-commit checks for all the new files. At first, I used the 'black'configuration, but then realised I needed to align with the pre-commit settings already used in the rest of the package. After making the adjustments, the latest version of the files successfully passed all pre-commit checks.
 
