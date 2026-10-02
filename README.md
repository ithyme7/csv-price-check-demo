# CSV Price Check — fixed-data demo

A free interactive preview of CSV Price Check, using **ten fixed fictional comparison items**. Review price-change flags, approve eligible sample changes individually and inspect the resulting CSV text preview. Nothing is approved automatically.

[Try the demo on the product page](https://ithyme7.itch.io/csv-price-check). The full downloadable tool has a **$19 USD one-time listed minimum price**; itch.io shows checkout terms and any applicable taxes.

The browser embed observed on the product page on 2 October 2026 is [this hosted demo](https://html-classic.itch.zone/html/19522805/index.html?v=1790959193). The product-page link is the stable place to find the current demo and paid release.

## Try the sample

1. Use the hosted demo, or download this repository and keep its three files together.
2. For a local copy, open `index.html` in a desktop browser with JavaScript enabled. **Direct `file://` opening has not been verified.** The recorded browser checks used Chromium through local HTTP and the hosted itch.io embed. Other browsers, mobile use and an anonymous hosted session remain unverified.
3. Inspect the rows. For example, SKU `000102` keeps its leading zero and shows a proposed price of `8.90`; the zero-price example requires individual approval.
4. Select an eligible changed row to see it in the CSV text panel. Duplicate, missing, new, absent, invalid and unchanged items cannot be approved.
5. Change the review threshold or display currency to clear approvals. Currency changes formatting only; it does not convert prices. **Reset sample** restores the original examples.

## Demo limits

This copy accepts no uploaded or local CSV files and has no own-file import, downloadable exports or saved sessions. Its output is a **text preview of the fixed sample only**. It has no shop connection and does not change live prices.

All demo code and styles are embedded in `index.html`. Once loaded, the demo runs locally in the browser without external runtime assets, automatic network requests or runtime AI. Its Content Security Policy blocks connections. Following a product-page link is a user-initiated visit to itch.io and needs a network connection.

The original application code was developed with generative AI assistance and reviewed/tested by AI agents. AI is not used to process the sample. The existing packaged-demo checks and recorded browser checks were performed before this repository was prepared; this repository adds no new functionality or browser-compatibility claim.

## What the full paid tool adds

The [full CSV Price Check download](https://ithyme7.itch.io/csv-price-check) lets you load your own current and intended new **selling-price** CSVs, map columns, compare exact SKUs, approve individual existing-product price changes, download approved updates and download a full audit CSV. It includes example CSVs, a quick-start guide, editable source and a separate licence for your own commercial business.

The documented input limits are UTF-8 CSVs with comma, semicolon or tab delimiters and dot or comma decimals, up to **5 MiB, 25,000 records and 250 columns per file**. Both files must use the same currency and tax basis. The tool does not calculate margins, markup, tax or currency conversion.

The update format uses `SKU` and `Regular price` for the documented WooCommerce mapping. It is not a live store connector, Shopify importer, product-creation tool or full import validator. Actual WooCommerce import remains unverified. Keep a backup and test a small batch on staging before using a live store. CSV Price Check is independent of WooCommerce and itch.io. Buying the full tool does not promise shop compatibility or business results.

## Licence

`LICENSE.txt` contains the **unchanged custom demo licence**, followed by the **unchanged Papa Parse MIT notice**. The demo licence refers to the original archive's `PAPAPARSE-LICENSE.txt`; its complete notice is preserved in this repository's combined `LICENSE.txt`.

The MIT notice applies to **Papa Parse only**, not to the original CSV Price Check application code. The custom demo licence permits evaluation and sharing of the complete unmodified demo archive with its README and licence notices intact. It does not permit resale, rebranding or extraction of the application's code to redistribute a general CSV tool. The paid product has its own licence.
