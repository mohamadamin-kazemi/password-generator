# Password Generator 🔐

A Python project for generating secure and memorable passwords using different strategies such as:

- Numeric PIN codes
- Random secure passwords
- Memorable word-based passwords

Built with clean, object-oriented Python design.

---

## Features

- Generate numeric PINs
- Generate secure random passwords
- Generate memorable passwords using English words
- Configurable password length and settings
- Optional symbols and numbers
- Optional random capitalization
- Uses abstract base classes (OOP)
- Clean and Pythonic code structure

---

## Project Structure

```text
PASSWORD-GENERATOR/
│
├── src/
│   └── main.py
│
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/mohamadamin-kazemi/password-generator.git
```

### 2. Navigate into the project directory

```bash
cd password-generator
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Download NLTK words dataset

Run Python:

```python
import nltk
nltk.download("words")
```

---

## Usage

Run the program:

```bash
python src/main.py
```

Example output:

```text
Generated PIN: 482193
Generated Random Password: p@9Ks!2LmQ#x
Generated Memorable Password: APPLE-river-HOUSE-cloud
```

---

## Password Generators

### 1. PIN Generator

Generates numeric PIN codes.

```python
pin_generator = PinGenerator(length=6)
print(pin_generator.generate())
```

---

### 2. Random Password Generator

Generates secure random passwords using letters, numbers, and symbols.

```python
random_password_generator = RandomPasswordGenerator(
    length=12,
    include_numbers=True,
    include_symbols=True,
)

print(random_password_generator.generate())
```

---

### 3. Memorable Password Generator

Generates readable passwords using random English words.

```python
memorable_password_generator = MemorablePasswordGenerator(
    number_of_words=4,
    separator="-",
    capitalization=True,
)

print(memorable_password_generator.generate())
```

---

## Requirements

- Python 3.10+
- nltk

---

## Technologies Used

- Python
- Object-Oriented Programming (OOP)
- Abstract Base Classes (`abc`)
- NLTK

---

## License

This project is licensed under the MIT License.

---

## Author

**Mohamadamin Kazemi**

---