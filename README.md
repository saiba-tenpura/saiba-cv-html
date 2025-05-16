# Saiba CV - HTML

Repo for storing my personal HTML based curriculum vitae templates.

Sidebar Version | Header Version
:--------------:|:------------------:
![CV with Sidebar](https://github.com/saiba-tenpura/saiba-cv-html/blob/main/saiba-cv-sidebar.jpg?raw=true) | ![CV with Header](https://github.com/saiba-tenpura/saiba-cv-html/blob/main/saiba-cv-header.jpg?raw=true)

## Generating Files
The easiest way to create the PDFs is using Firefox together with a local Python webserver.
```bash
python -m http.server -d .
```

Visit localhost:8000 in Firefox, Ctrl + P and "Save to PDF".

Use magick to generate the example JPG images from the PDF files.
```bash
magick -verbose -density 300 saiba-cv-sidebar.pdf -quality 90 -flatten -sharpen 0x1.0 saiba-cv-sidebar.jpg
magick -verbose -density 300 saiba-cv-header.pdf -quality 90 -flatten -sharpen 0x1.0 saiba-cv-header.jpg
```

## License
[MIT](./LICENSE)

## Author
This project was created in 2025 by Saiba Tenpura.
