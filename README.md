# Interview Project for Python Backend Developer

Create a private git repo and implement the following project.

## Goal
### Coding
1. Create a Django project (use https://pipenv.pypa.io/en/latest/)
2. Use Postgres as DB (in Docker container)
3. Add tables:
    - Person (name, email, age, phone, address, created datetime, modified datetime)
    - Employee (person_id Foreign Key, department, role, line_manager person_id Foreign Key, created datetime, modified datetime)
        - `person_id` refers to `id` of a person from the `Person` table
4. Django Admin views
    1. one for Person and Employee models
    2. relevant fields should be separately displayed in columns
    3. add filters for all fields (see: [https://docs.djangoproject.com/en/4.0/ref/contrib/admin/](https://docs.djangoproject.com/en/4.0/ref/contrib/admin/))
    4. sortable
6. REST APIs to add, delete, modify single or multiple
    - Person(s)
    - Employees(s) 
7. REST APIs to bulk query Persons or Employees over any combinations of the fields of the two models
8. Postman file demonstrating the REST APIs (see [https://apitransform.com/how-to-export-all-collections-from-postman/](https://apitransform.com/how-to-export-all-collections-from-postman/))
9. Tests
    1. Pytest ([https://pytest-django.readthedocs.io/en/latest/](https://pytest-django.readthedocs.io/en/latest/)) using Django APIClient
    2. One test.py for each view
    3. One integration test
    4. No model access in test except for verification if not possible with only APIs
11. [https://pylint.org/](https://pylint.org/) your code
12. [https://coverage.readthedocs.io/en/6.2/](https://coverage.readthedocs.io/en/6.2/) code coverage (exclude all 3rd party libraries)
13. Document code with https://docs.python.org/3/library/pydoc.html
14. Run tests and lint with Github Actions (https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-nodejs-or-python?langId=py)

### Deliverables (pushed to private repo)
_**include this README and check if completed or explain why it isn't done**_
- [ ] Source code
- [ ] Development setup instructions including commands for running lint and tests with coverage
<br>_example template_
> ### Development Setup
> ```
> 1. git clone <your repo url here>
> 2. docker run postgres ...
> 3. python manage.py makemigrations
> ...
> 4. pylint ...
> 5. pytest ... --cov=...
> ```
- [ ] PyLint run report (expected no errors or warnings)
- [ ] Coverage report (expected 100% code coverage)
- [ ] Postman json
- [ ] GitHub Action run in your private repo



### Selection Criteria
1. Make sure that checklist above is complete
2. In case any point on the checklist is failed to be accomplished please provide all attempt information and reason for failure in details
3. Incomplete submissions without proper explanation or documentation will be rejected

## Code Evaluation
Provide `walter-weinmann`, `c-bik` and `janmenjoyroy` with **read** access to your repository.

## Interview Demo
An interviewee will demonstrate the project in action and perform certain operations as requested. Questions will be asked about your different coding choices in the project and on any part of the repository.
