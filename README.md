# Bootstrap Dark Mode Switch

A simple and reusable dark mode toggle switch using Bootstrap 5 for your website.

## Description

This project integrates a dark mode switch into your website, allowing users to toggle between dark and light themes. It uses Bootstrap 5 for styling and JavaScript for functionality, with the state of the theme being persisted in local storage so that the user's preference is maintained across sessions.

## Features

- Easy to integrate with existing Bootstrap projects
- Uses local storage to remember the user's theme preference
- Automatically applies the user's preferred theme on page load

## How to Use

To use this switch in your project, follow these steps:

1. Make sure Bootstrap 5 is included in your project:

```html
<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Bootstrap Bundle JS (includes Popper) -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>

```

2. Include the HTML for the switch in your webpage:

```html
<!-- Bootstrap 5 switch -->
<div class="form-check form-switch">
    <input class="form-check-input" type="checkbox" id="darkModeSwitch" checked>
    <label class="form-check-label" for="darkModeSwitch">Dark Mode</label>
</div>
```

3. Add the JavaScript code to handle the switch behavior:

```js
document.addEventListener('DOMContentLoaded', (event) => {
    const htmlElement = document.documentElement;
    const switchElement = document.getElementById('darkModeSwitch');

    // Set the default theme to dark if no setting is found in local storage
    const currentTheme = localStorage.getItem('bsTheme') || 'dark';
    htmlElement.setAttribute('data-bs-theme', currentTheme);
    switchElement.checked = currentTheme === 'dark';

    switchElement.addEventListener('change', function () {
        if (this.checked) {
            htmlElement.setAttribute('data-bs-theme', 'dark');
            localStorage.setItem('bsTheme', 'dark');
        } else {
            htmlElement.setAttribute('data-bs-theme', 'light');
            localStorage.setItem('bsTheme', 'light');
        }
    });
});
```

4. (Optional) Customize the switch's appearance using Bootstrap's form-check classes or your own CSS.

## Customization

You can easily customize the look and feel of the dark mode switch to match your website's branding. Use Bootstrap's utility classes or your own CSS to create a unique user experience.

## Contribution

Feel free to fork the project and submit pull requests. You can improve the script, add new features, or propose improvements to the documentation.

## License

This project is open-source and available under the [MIT License](LICENSE).
