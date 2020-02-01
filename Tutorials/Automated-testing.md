# Automated Testing

Software can be full of mistakes. Devs can misinterpret specs, or not implement them yet, or provide an incorrect implementation. Testing tries to provide a safety net that catches these problems and brings them to everyones attention.

* Fowler calls for unit tests that run in 10 minutes or less. The quicker they are, the more frequently they can be run without interrupting normal work flow.

* Different levels of test:
    1. Unit test
    2. Integration test
    3. End-to-end test

It can be a good idea to run tests in this order, if a unit test fails, then the devs will know not to trust later tests that depend on the individual components.

The tests can live in the codebase alongside the code they are testing. When source code is changed, a corresponding change is made to the component's unit test. Both changes can be checked in together.

