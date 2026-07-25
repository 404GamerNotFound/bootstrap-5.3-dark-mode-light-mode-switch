# Bootstrap Dark Mode Switch

[![Stars](https://img.shields.io/github/stars/404GamerNotFound/bootstrap-5.3-dark-mode-light-mode-switch?style=for-the-badge&logo=github&logoColor=white&label=Stars&color=blue)](https://github.com/404GamerNotFound/bootstrap-5.3-dark-mode-light-mode-switch/stargazers)
[![Sponsors](https://img.shields.io/github/sponsors/404GamerNotFound?style=for-the-badge&logo=github&logoColor=white&label=Sponsors&color=blue)](https://github.com/sponsors/404GamerNotFound)
[![PayPal](https://img.shields.io/badge/PayPal-ME-blue?style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/paypalme/TonyBrueser)
[![Revolut](https://img.shields.io/badge/Revolut-ME-blue?style=for-the-badge&logo=revolut&logoColor=white)](https://revolut.me/tony1995)

This repository now contains **two examples**:

1. **Version 1 (Legacy)**: the original dark/light toggle.
2. **Version 2 (Extended)**: dark/light + system mode.

## Description

The original behavior is preserved and a second, more advanced variant is added. Both examples use Bootstrap 5.3.6 and store preferences in localStorage.

## Features

### Version 1 (Legacy)

- Original dark/light switch behavior
- Uses `localStorage` key: `bsTheme`
- Minimal implementation

### Version 2 (Extended)

- Dark/light switch plus `Use system mode` button
- Uses `localStorage` key: `bsThemeMode`
- Supports `dark`, `light`, and `system`
- Reacts to OS preference changes (`prefers-color-scheme`)
- Shows current mode status text

## CDN Version

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.6/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.6/dist/js/bootstrap.bundle.min.js"></script>
```

## Notes

- The legacy example remains available as requested.
- The extended version is added separately, so both can be compared side by side.
- See `index.html` for the full implementation.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Support

If you find this project helpful, you can support it via PayPal: [paypal.me/TonyBrueser](https://www.paypal.com/paypalme/TonyBrueser)
