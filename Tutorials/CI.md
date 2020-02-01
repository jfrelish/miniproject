# CI

## Continuous Integration

Continuous integration is a process software development teams use to collaborate, stay agile, and minimize bugs. 
CI was inspired by the XP methodology of Kent Beck, documented by [Martin Fowler in 2006](https://martinfowler.com/articles/continuousIntegration.html) and has enabled the agile process in that time.

#### Main Points of CI:
* Developers integrate with the main line of development early and often.
* Create unit tests that can confirm the code is not broken.
* Create an environment in which the tests can be run for each checkin.

#### Example Daily Workflow
* Merge copy of main line into local dev branch
* Work on local dev to complete ticket (feature or bug)
* Run unit tests locally
* If tests pass, push from local to remote
* If tests pass on CI server, create pull request
* Have a code review of the branch
* If all is well, merge from the dev branch to main line
   