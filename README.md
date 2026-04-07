# Bootstrap Dark Mode Switch

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
