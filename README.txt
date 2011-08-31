This module lets you show a preview of PDF files uploaded through FileField.
This module uses ImageMagick to extract the first page of a PDF file to a JPEG
image which is used as PDF preview link to the file. If imagecache module is
available, you can select any imagecache preset for the PDF preview image link.
Instead of convert pdf files onto a set of images like PDF to ImageField does,
and lost any connection to the PDF file, PDFPreview extract only the first page
and uses it as link to PDF file. The images are stored on a configurable folder
inside your files folder, so it's fully compatible with multisite installations.
If the image is missing at display moment it will be created.

- Usage:
Install like any other module and enable it. Go to 'Display fields' page of your
content type and select 'PDFPreview' as formatter. If you have imagecache
enabled, you will have one 'PDFPreview: presetname image' option for each
imagecache preset you have. You can also use it as a field formatter on a Views
view.

 - Requisites:
ImageAPI module with ImageMagick toolkit enabled and configured. Is not
necessary to be set as default toolkit. FileField module and a content type
which uses it. Imagecache module if you want to use other image sizes or add
efects to thumbnails.
