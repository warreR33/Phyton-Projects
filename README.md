# Python Utilities Collection

## Overview

This repository contains two simple Python scripts:

1. **BMI Calculator** — Calculates a user's Body Mass Index and classifies their weight category.
2. **Automatic File Sorter** — Organizes files in a directory into folders based on file type.

---

## 1. BMI Calculator

### Description

This script prompts the user to enter their name, weight (kg), and height (meters). It calculates BMI using the formula:

[
BMI = \frac{weight}{height^2}
]

It then prints the BMI value and a classification message.

### Categories Used

| BMI Range | Classification    |
| --------- | ----------------- |
| 16–18.5   | Moderate Thinness |
| 18.5–25   | Normal            |
| 25–30     | Overweight        |
| 30–35     | Obese Class I     |
| 35–40     | Obese Class II    |
| >40       | Obese Class III   |

If input is invalid or outside expected range, it displays an error message.

### How to Run

```bash
python bmi_calculator.py
```

---

## 2. Automatic File Sorter

### Description

This script scans a directory and automatically sorts files into folders depending on their extension.

### Supported File Types

* `.csv` → **csv files/**
* `.png` → **image files/**
* `.txt` → **text files/**

If the folders do not exist, the script creates them automatically.

### Configuration

Edit this line in the script to match your directory path:

```python
path = r"F:/DATA P/DataSets/Imports/"
```

### How to Run

```bash
python automatic_file_sorter.py
```

---

## Requirements

* Python 3.x
* Standard libraries only:

  * `os`
  * `shutil`

(No external packages required.)

---

## Notes

* The file sorter will **move files**, not copy them.
* It ignores files already placed in their correct folder.
* Only specified file types are handled. Others remain untouched.

---

## Possible Improvements

* Add support for more file formats.
* Use command-line arguments instead of hardcoded paths.
* Add logging.
* Add GUI interface.
* Improve error handling and validation.

---

## License

This project is free to use and modify for educational or personal purposes.
