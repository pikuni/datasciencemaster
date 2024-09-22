---
description: >-
  Pytest is a testing framework based on python. It is mainly used to write API
  test cases.
---

# PyTest

## Summary of pytest&#x20;

* Installing pytest&#x20;
  * Install latest version using `pip install pytest`&#x20;
  * Confirm the installation using `pytest -h`
* Identifying test files and test functions.
  * Running pytest without mentioning a filename will run all files of format **test\_\*.py** or **\*\_test.py** in the current directory and subdirectories.
  * Pytest requires the test function names to start with **test**. Function names which are not of format **test\*** are not considered as test functions by pytest.
* Executing all test files using `pytest –v`.
* Executing specific file using `pytest <filename> -v`.
* Execute tests by substring matching `pytest -k <substring> -v`.
* Execute tests based on markers `pytest -m <marker_name> -v`.
* Creating fixtures using `@pytest.fixture`.
* `conftest.py` allows accessing fixtures from multiple files.
* Parametrizing tests using `@pytest.mark.parametrize`.
* Xfailing tests using `@pytest.mark.xfail`.
* Skipping tests using `@pytest.mark.skip`.
* Stop test execution on n failures using `pytest --maxfail = <num>`.
* Running tests in parallel using `pytest -n <num>`.
* Generating results xml using `pytest -v --junitxml = "result.xml"`.



Ref: [https://www.tutorialspoint.com/pytest/pytest\_environment\_setup.htm](https://www.tutorialspoint.com/pytest/pytest\_environment\_setup.htm)
