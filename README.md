# Accuknox Django Trainee Assignment

This repository contains solutions for the Django Trainee Assignment provided by Accuknox.

## Topic: Django Signals

### Question 1: Are Django Signals Synchronous or Asynchronous by Default?

**Answer:** Django signals are executed synchronously by default. The implementation demonstrates that the caller waits until the signal handler completes execution.

**Location:** `Answer1/`

**Run:**

```bash
python manage.py test_sync_signal
```

---

### Question 2: Do Django Signals Run in the Same Thread as the Caller?

**Answer:** By default, Django signals execute in the same thread as the caller. The implementation compares thread identifiers of the caller and signal handler to verify this behavior.

**Location:** `Answer2/`

**Run:**

```bash
python manage.py test_thread_signal
```

---

### Question 3: Do Django Signals Run in the Same Database Transaction as the Caller?

**Answer:** By default, Django signals participate in the same database transaction as the caller. The implementation demonstrates that when a transaction is rolled back, changes made inside the signal handler are also rolled back.

**Location:** `Answer3/`

**Run:**

```bash
python manage.py test_transaction_signal
```

---

## Topic: Custom Classes in Python

### Rectangle Class

Implemented a custom `Rectangle` class that:

* Requires `length: int` and `width: int` during initialization.
* Supports iteration using the `__iter__()` method.
* Returns:

  ```python
  {'length': <VALUE_OF_LENGTH>}
  ```

  followed by

  ```python
  {'width': <VALUE_OF_WIDTH>}
  ```

**Location:** `Class/code2.py`

---

## Project Structure

```text
Accuknox Assignment
│
├── Answer1
│
├── Answer2
│
├── Answer3
│
├── Class
│   └── code2.py
│
└── README.md
```

---

## Technologies Used

* Python 3.x
* Django
* SQLite
* Django Signals
* Object-Oriented Programming (OOP)

## Submitted by

Tanveer Kalluru
