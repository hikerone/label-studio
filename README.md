# Label Studio for Chrome

Prepare shipping labels for thermal printers or US Letter sheets. Import a PDF, check the crop, add optional artwork, then save a PDF or open Chrome’s print preview. Processing happens locally in the extension.

## Features

- **Label sizes:** 4 × 6, 4 × 8, 6 × 4, A6, 100 × 150 mm, and custom sizes.
- **4 × 8 options:** Print a full 4 × 8 shipping label, or keep a 4 × 6 label at full size with a separate two-inch area above it.
- **Personalization:** Add a logo, image, or text. Choose from 12 text styles and see a live sample.
- **Automatic placement:** Look for a clear top area or a divided bottom footer on each label. Artwork is skipped with a warning when no suitable space is found.
- **Sheet layouts:** Print one, two, or four labels on US Letter paper. Artwork stays inside each individual label.
- **Batch editing:** Select, reorder, crop, rotate, and inspect pages before output.

## Install

1. Download and extract the latest release ZIP.
2. Open `chrome://extensions` in Chrome.
3. Turn on **Developer mode**.
4. Select **Load unpacked** and choose the extracted folder containing `manifest.json`.
5. Pin **Label Studio — Shipping Labels** from Chrome’s Extensions menu if you want quick access.

Keep the extracted folder in place while the extension is installed.

## Prepare a label

1. Open Label Studio and choose a shipping-label PDF. You can also drop PDFs into the editor.
2. Check the crop on every page. Keep the full address, service markings, and barcodes visible.
3. Choose the label size, printer profile, and sheet layout.
4. Optionally add text or an image. For a 4 × 6 label on 4 × 8 paper, select the mode with the separate top area.
5. Check the label and sheet previews, then save the PDF or open print preview.

In Chrome’s print dialog, choose the matching paper size, **100% or actual size**, no margins, and no headers or footers. Four-label US Letter output reduces label size; confirm that your carrier accepts the result.

## Placement and print checks

Automatic artwork placement avoids gaps between address, postage, and tracking sections. It may leave a label undecorated when it cannot find a suitable area. Inspect every preview before printing, especially the delivery address and all barcodes.

The editor checks for some crop, image-quality, and barcode problems, but a passed check does not certify a physical print or guarantee a carrier scan.

## Privacy

PDF editing and image processing happen locally. Imported files are not uploaded by the extension. Capturing a label from a website may require permission to access that site. Printer settings and text choices are stored locally; an uploaded logo or image stays in the current editor tab.

## Limits

- 25 MB per input PDF
- 50 MB per batch
- 100 pages per batch
- Password-protected PDFs are not supported

## Development

There is no build step; the extension folder can be loaded unpacked in Chrome.

```bash
npm test
npm run release
```

`npm run release` runs checks and creates a ZIP in `release/`.

Label Studio is an independent tool and is not affiliated with USPS, Vinted, Amazon, or other carriers and marketplaces.
