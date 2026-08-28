# bulk-document-scanner-web

Web demos for bulk document scanning.

* [document-scanner-via-twain.html](https://tony-xlh.github.io/bulk-document-scanner-web/document-scanner-via-twain.html). Use [Dynamic Web TWAIN](https://www.dynamsoft.com/web-twain/overview/) (`dwt@19.4.3`) to access document scanners via TWAIN.
* [document-scanner-via-camera.html](https://tony-xlh.github.io/bulk-document-scanner-web/document-scanner-via-camera.html). Use [Dynamsoft Capture Vision Bundle](https://www.npmjs.com/package/dynamsoft-capture-vision-bundle) (`dynamsoft-capture-vision-bundle@3.6.3000`, replaces the deprecated standalone Document Normalizer) for document border detection and [Dynamsoft Document Viewer](https://www.dynamsoft.com/document-viewer/docs/introduction/index.html) (`dynamsoft-document-viewer@5.0.0`) to control the workflow. The DDV `documentBoundariesDetect` processing handler bridges DDV camera frames to `CaptureVisionRouter.capture(DSImage, 'DetectDocumentBoundaries_Default')`.

Camera demo video:

https://github.com/xulihang/bulk-document-scanner-web/assets/5462205/7e839b2a-bb93-4cf9-8f2c-36494e4e5cc4

## Run

Open the HTML files over `http://localhost` or HTTPS (camera and the DWT service require a secure context), e.g. `python -m http.server`. Each demo loads the SDK from the jsDelivr/unpkg CDN and uses a public one-day trial key; replace it with [your own](https://www.dynamsoft.com/customer/license/trialLicense/?product=dcv&package=cross-platform) for production.

