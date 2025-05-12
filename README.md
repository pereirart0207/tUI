tUI – Lightweight Web UI Utility Module
tUI is a self-invoking JavaScript module that provides essential UI helpers for modern web interfaces: loading spinners, toast notifications, and custom modals. It is lightweight, dependency-free, and designed for easy integration.

🚀 Features
✅ Customizable loading spinner (color, size, message, background)

✅ Toast notifications with support for different types (success, error, warning, info, dark) and duration control

✅ Dynamic modals for displaying HTML content

✅ Automatically prevents multiple instances from loading

✅ Exposes a clean global API via window.tUI

📦 Installation
Include the script in your HTML file, preferably before the closing </body> tag:

html
Copiar
Editar
<script src="tui.js"></script>
🧩 Usage
Show a Spinner
js
Copiar
Editar
tUI.showSpinner({
  message: "Processing...",
  color: "#007bff",
  size: 60,
  background: "#f0f0f0"
});
Hide the Spinner
js
Copiar
Editar
tUI.hideSpinner();
Show a Notification
js
Copiar
Editar
tUI.showNotification({
  message: "Operation completed successfully",
  type: "success", // success | error | warning | info | dark
  duration: 5000,  // in milliseconds
  fontSize: "15px"
});
Show a Modal
js
Copiar
Editar
tUI.showModal("<h2>Hello World</h2><p>This is a custom modal.</p>");
Close the Modal Manually
js
Copiar
Editar
tUI.closeModal();
🎨 Customization
You can override the default styles by injecting your own CSS or by modifying the <style> block dynamically added to the document's <head>.

🧠 Notes
The module dynamically appends necessary HTML elements to the body.

It prevents duplicate initialization if already loaded.

All functionality is accessible via the global tUI object.

📄 License
MIT

