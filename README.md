# Label Studio 2.3.3

Label Studio prepares marketplace and carrier shipping labels for printing on thermal or standard printers. It can capture visible labels or import PDF files. Label processing happens locally in the extension.

## Install in Chrome

1. Download `label-studio-2.3.3.zip` from **Assets** below and extract it to a folder you’ll keep.
2. In Chrome, open `chrome://extensions`.
3. Turn on **Developer mode**.
4. Click **Load unpacked** and select the extracted folder containing `manifest.json`.
5. Pin Label Studio from Chrome’s Extensions menu if you want quick access.

Keep the extracted folder in place while using the extension. To update, download and extract the new release, then load its folder from `chrome://extensions`.

## Use

Click the Label Studio toolbar icon on a supported page to capture a visible label, or choose a PDF from your device in the editor. Review the crop and every barcode before printing. You can save a prepared PDF or open Chrome’s print preview.

In Chrome’s print dialog, select the matching paper size and printer. Check the scaling, margins, and headers before printing.

## Notes

- PDF imports work offline. Processing stays on your device.
- Capturing labels from websites may require site access and depends on the page layout. Downloading the label as a PDF and importing it is a useful fallback.
- Automatic crops and quality warnings are aids; inspect the output before use.
- Physical printer output and live authenticated marketplace workflows have not been verified for this release.

See the project README and changelog for more details.
