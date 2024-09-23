**README for YouTube Video to PDF Converter**

## Project Overview

This repository contains a Jupyter Notebook that allows you to convert YouTube video URLs to PDF documents. The converter leverages the `pdfkit` library to generate PDF files from HTML.

## Features

* Convert YouTube video URLs to PDF documents
* Flexible conversion options, including page size and orientation
* Option to include table of contents and page numbers
* Easy-to-use interface with customizable parameters

## Installation

* Install the `pdfkit` library using `pip install pdfkit`
* Download or clone this repository

## Usage

1. Open the `youtubeVideoToPdf.ipynb` notebook in Jupyter Lab or Jupyter Notebook.
2. Paste the YouTube video URL in the `video_url` variable.
3. (Optional) Customize the conversion parameters as desired.
4. Run all cells in the notebook.

**Note:** Ensure that `wkhtmltopdf` is installed and added to your system path (e.g., `/usr/local/bin/wkhtmltopdf`).

## Output

The output PDF file will be saved in the same directory as the notebook. The filename will be based on the video title.

## Example Usage

To convert the YouTube video "How to Use Jupyter Notebooks" to a PDF with custom page size:

```
import pdfkit

video_url = "https://www.youtube.com/watch?v=i0drVsIC1Lc"

# Set custom page size and orientation
options = {
    "page-size": "A4",
    "orientation": "Landscape",
}

# Generate the PDF
pdfkit.from_url(video_url, "youtubetutorial.pdf", options=options)

# Print success message
print("Successfully converted YouTube video to PDF.")
```

## Contributing

Contributions are welcome! Please feel free to:

* Report bugs or suggest improvements
* Add new features or functionality
* Improve documentation or code quality

## License

This project is licensed under the MIT License. See the LICENSE file for details.