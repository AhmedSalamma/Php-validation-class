# Php-validation-class
The Validation class is a PHP utility for validating form input data. It offers a set of static methods to validate fields against common rules such as required fields, email format, numeric values, and string length constraints. Designed for ease of use, it is a valuable addition to any PHP project requiring form validation.

use core\validation\Validation;

Validation::make([
    'username' => 'required|string|min:3|max:20',
    'email' => 'required|email',
    'age' => 'required|number|min:1|max:3'
]);

if (!empty(Validation::$errors)) {
    echo Validation::any(); // Prints all error messages
} else {
    // Process the form data
}

