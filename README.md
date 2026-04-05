# 📅 clsDate Library

## 📌 Overview

`clsDate` is a complete C++ date handling class that provides functionality similar to modern date libraries.

It allows creating, validating, manipulating, and comparing dates.

---

## 🚀 Features

### 📆 Date Creation

* Current system date
* From string (dd/mm/yyyy)
* From day order in year
* Custom (day, month, year)

---

### 🔍 Date Validation

* Check if date is valid
* Leap year detection

---

### ➕ Date Operations

* Add / subtract:

  * Days
  * Weeks
  * Months
  * Years
  * Decades / Centuries

---

### 📊 Date Analysis

* Day of week
* Days in month/year
* Remaining days in:

  * Week
  * Month
  * Year

---

### 📈 Date Comparison

* Before / After / Equal
* Difference in days

---

### 📅 Calendar

* Print monthly calendar
* Print yearly calendar

---

## 🛠️ Usage

```cpp
#include "clsDate.h"

int main() {
    clsDate d1(1, 1, 2024);
    clsDate d2("10/1/2024");

    cout << clsDate::GetDifferenceInDays(d1, d2) << endl;

    d1.AddDays(10);
    d1.Print();

    return 0;
}
```

---

## 🧠 Design Notes

* Combines:

  * Procedural functions (static)
  * Object-oriented design

* Uses custom algorithms instead of external libraries

---

## ⚠️ Limitations

* Does not use `std::chrono`
* Performance can degrade with large date differences
* Limited error handling for invalid input strings

---

## 📌 Future Improvements

* Use modern C++ (`chrono`)
* Optimize date difference calculations
* Add timezone support
