## Captcha Solver Frontend (Client-side only)

This is a simple client-side application designed to demonstrate a basic captcha solving interface. It's built with HTML, Tailwind CSS, and vanilla JavaScript.

### Features:
- Displays a captcha image (`sample.png` by default).
- Allows users to input text from the captcha.
- Provides immediate feedback on whether the input is correct (for the default image).
- Supports dynamic captcha images via URL parameters (though validation for dynamic images is not implemented client-side).

### How to Use:
1.  **Open `index.html` in your browser.**
2.  You will see a captcha image (by default, `sample.png`).
3.  Type the text you see in the image into the input field.
4.  Click "Submit" or press Enter.
5.  Receive feedback on your attempt.

### Default Captcha:
- The default `sample.png` contains the text: `ADORS`
- The client-side validation specifically checks for `ADORS` (case-insensitive due to `.toUpperCase()` in JS).

### Dynamic Captcha (Client-side display only):
- You can specify a custom image URL by adding a `?url=` parameter to the `index.html` URL.
- **Example:** `index.html?url=https://example.com/your-captcha-image.png`
- **Note:** Client-side validation is *only* for the `sample.png` image. If you provide a dynamic URL, the app will display the image but will inform you that validation requires a backend service.

### Project Structure:
- `index.html`: The main application file containing HTML, Tailwind CSS setup, and JavaScript logic.
- `sample.png`: The default captcha image.

### Technologies Used:
- HTML5
- Tailwind CSS (via CDN)
- Vanilla JavaScript
