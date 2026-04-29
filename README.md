# PHP Validation Class

A simple and lightweight PHP validation class for handling form validation rules easily.

---

## 🚀 Features

- Required field validation
- Email validation
- Numeric validation
- String validation
- Min / Max length validation
- Easy rule-based syntax
- Static usage (no instantiation needed)

---

## 📦 Usage

```php
use core\validation\Validation;

Validation::make([
    "email" => "required|email",
    "name"  => "required|string|min:3|max:50",
    "age"   => "required|number"
]);
