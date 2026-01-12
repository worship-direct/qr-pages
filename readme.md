# QR Code Generator for Worship Direct

qr.worship.direct/###

## Dynamic QR Code Generation

This repository provides a dynamic QR code generator that creates QR codes linking to `worship.direct/###` where `###` can be any alphanumeric code (0-9, A-Z).

## Usage

### Using URL Parameters (Recommended)
Access the QR code generator using:
```
index.html?page=CODE
```

Examples:
- `index.html?page=000` - Generates QR code for worship.direct/000
- `index.html?page=AAA` - Generates QR code for worship.direct/AAA
- `index.html?page=ZZZ` - Generates QR code for worship.direct/ZZZ
- `index.html?page=123` - Generates QR code for worship.direct/123

### Using Direct HTML Files (Backward Compatibility)
For backward compatibility with existing URLs, you can create individual HTML files (e.g., `000.html`, `AAA.html`) that redirect to the main index page with the appropriate parameter. This is only needed if you want to support legacy URLs. See `000.html` as an example.

## Features

- **Dynamic Generation**: Only one page (`index.html`) needs to be maintained
- **Client-Side QR Generation**: Uses qrcodejs library for generating QR codes directly in the browser
- **Automatic URL Encoding**: Correctly encodes URLs for QR code generation
- **Responsive Design**: Clean, centered layout that works on all devices
- **High Error Correction**: QR codes use high error correction level for better scanning reliability

## Technical Details

The QR codes link to `https://worship.direct/###` for church pages.

QR code generation is powered by [qrcodejs](https://github.com/davidshimjs/qrcodejs), a JavaScript library for creating QR codes.