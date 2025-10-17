# Hello World + CSV Viewer

## Overview
This is a minimal, static web app that:
- Displays the text “Hello World”.
- Loads and displays the contents of sample.csv as a table on the home page.
- Includes a graceful fallback: if the browser blocks loading local files (e.g., when opened via file://), the page shows a bundled preview of sample.csv so data is still visible.

## Setup
1. Ensure the following files are in the project root:
   - index.html
   - sample.csv (provided)

2. Serve the folder with any static web server (recommended to avoid browser restrictions on local file access):
   - Python 3: python3 -m http.server 8000
   - Node.js (serve): npx serve .
   - VS Code: Use the “Live Server” extension and open index.html

3. Open http://localhost:8000 (or your server’s URL) in your browser.

Note: Opening index.html directly via file:// may prevent fetch() from reading sample.csv due to browser security. The page will then show the bundled preview automatically.

## Usage
- Navigate to the app in your browser; you will see:
  - “Hello World” header.
  - A table rendering the contents of sample.csv.
- Use the “Download CSV” button to download or inspect sample.csv directly.
- To display different data, replace sample.csv with your own CSV file using the same filename and refresh the page.

## License
MIT License

Copyright (c) 2025 Your Name

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.