# HTML File with CSS `:user-invalid` Implementation

This HTML file demonstrates the use of the CSS `:user-invalid` pseudo-class to style form fields that contain invalid input.

## Table of Contents

* [Introduction](#introduction)
* [HTML Structure](#html-structure)
* [CSS Styles](#css-styles)

## Introduction

The `:user-invalid` pseudo-class is a CSS selector that targets form fields that contain invalid input. This pseudo-class is useful for providing visual feedback to users when they enter incorrect data.

## HTML Structure

The HTML file consists of a simple form with a text input field and a submit button:
```html
  <form>
        <div class="form__field">
            <input type="text" placeholder="Name" class="form__input" required>
            <span class="icon"></span>
        </div>
        <div class="form__field">
            <input type="email" placeholder="Email" class="form__input" required>
            <span class="icon"></span>
        </div>
        <div class="form__field">
            <input type="password" placeholder="Password" class="form__input" pattern=".{6,}" required>
            <span class="icon"></span>
        </div>
    </form>
```
## CSS Styles

The Css consists of:
```Css
        .form__input:user-invalid {
            border-color: firebrick;
        }

        .form__input:user-invalid+.icon::after {
            content: '❌';
        }
```
![ezgif-2-780d8c4791](https://github.com/user-attachments/assets/ac0c269d-eedf-46ee-99f4-d4e845939c75)
