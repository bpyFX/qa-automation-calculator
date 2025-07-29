# ✅ QA Portfolio Project Plan: Calculator Test Suite + CI/CD

This portfolio project is designed to showcase your ability to write automated tests, use modern testing tools (`pytest`), and integrate a basic CI/CD pipeline using GitHub Actions. It aligns directly with the QA Engineer role you're targeting.

---

## 📦 Project Overview

**Project Name:** `qa-automation-calculator`  
**Goal:** Build a simple calculator module in Python and test it with `pytest`, integrated with GitHub Actions.  
**Tech Stack:** Python, pytest, GitHub Actions, Markdown  

---

## 📁 File Structure

```bash
qa-automation-calculator/
├── app/
│   └── calculator.py
├── tests/
│   └── test_calculator.py
├── .github/
│   └── workflows/
│       └── python-app.yml
├── README.md
```

---

## 🧩 Step-by-Step Plan

### ✅ Step 1: Build the Calculator Module

**File:** `app/calculator.py`  
Functions to implement:
- `add(a, b)`
- `subtract(a, b)`
- `multiply(a, b)`
- `divide(a, b)` → Handle divide-by-zero with `ValueError`

---

### ✅ Step 2: Write Unit Tests with Pytest

**File:** `tests/test_calculator.py`  
Write at least 5 test functions:
- Basic test for each math function
- One failure case (e.g. divide-by-zero)

Example:
```python
def test_divide_by_zero():
    with pytest.raises(ValueError):
        divide(5, 0)
```

---

### ✅ Step 3: Setup GitHub Actions CI Workflow

**File:** `.github/workflows/python-app.yml`  
Configure the pipeline to:
- Use Python 3.10
- Install pytest
- Run all tests under `tests/`

Example:
```yaml
- name: Run tests
  run: pytest tests/
```

---

### ✅ Step 4: Write the README

**File:** `README.md`  
Include:
- ✅ Project description
- ✅ How to run tests locally
- ✅ GitHub Actions badge (after first push)
- ✅ Tools used

---

### ✅ Step 5: Push to GitHub

**Repo Name Suggestion:** `qa-automation-calculator`  
1. Initialize with Git  
2. Create `.gitignore` and commit your files  
3. Push to GitHub  
4. Ensure GitHub Actions runs automatically

---

### ✅ Step 6: Polish & Share

- Check that test coverage looks good  
- Clean and readable code with comments  
- Optional: Add test coverage badge with `pytest-cov`  
- Share the repo link in your resume and on LinkedIn

---

## 🧠 Bonus Ideas

- Add more edge cases (e.g., negative numbers, floats)
- Write tests using `@pytest.mark.parametrize`
- Add `pytest-cov` for test coverage
- Expand calculator into a Flask API and test endpoints

---

## 📌 Outcome

By finishing this project, you'll have:
- Demonstrated ability to write and run test suites
- Shown familiarity with DevOps practices (CI pipelines)
- Created a polished, real-world portfolio project

Perfect for showcasing your transition from manual QA to test automation engineer.
