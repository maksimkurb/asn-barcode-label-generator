# QR/MicroQR/Code128 barcode Label Generator for ASNs in Paperless-ngx

> [!NOTE]  
> This is a fork of original Tobias L. Maier [QR Code Label Generator](https://github.com/tmaier/asn-qr-code-label-generator).
>
> This version adds support of **STAFF 1156668** template and introduces MicroQR and Code128 barcode support.
>
> Also **Safety zone** setting introduced to ensure that no barcode overflows the label borders if your printer has bad precision.


## About the Project

This project is a web-based QR/MicroQR/Code128 barcode label generator specifically designed for generating Archive Serial Number (ASN) labels in Paperless-ngx. It's a simple and efficient tool aimed at streamlining the process of creating QR/MicroQR/Code128 code labels for document management.

A live version of this application can be accessed at <https://maksimkurb.github.io/asn-barcode-label-generator/>.

### Current Status

This application is currently in an **early alpha stage** and has not been extensively tested.
Users are encouraged to validate the output, especially the positioning of the labels.

### Supported label formats

The application currently supports the following label formats:

- Avery L4731REV-25 (See [UK shop](https://www.avery.co.uk/product/mini-multipurpose-labels-l4731rev-25), [DE shop](https://www.avery-zweckform.com/produkt/universal-etiketten-l4731rev-25))
- STAFF 115666 (189 labels) (See [RU shop](https://www.vseinstrumenti.ru/product/etiketka-samokleyaschayasya-staff-25-4x10mm-189-etiketok-belaya-80g-m2-50-listov-basic-115666-15347920/), [Wildberries](https://www.wildberries.ru/catalog/254336586/detail.aspx))

### Limitations

The application currently has the following limitations:

- The application is currently only available in English.
  This is considered a non-issue, as the application is designed to be self-explanatory.
- The application currently only supports the Avery L4731REV-25 label format.
  Contributions for additional label formats are welcome.
- The application only supports Google Chrome and Chromium-based browsers, such as Microsoft Edge. And partially Firefox.
  This limitation is due to the use of the [CSS `@page` rule](https://developer.mozilla.org/en-US/docs/Web/CSS/@page) for printing.
  Contributions for additional browser support are welcome.

### Key Design Decisions

- **Browser-Based Application**: The application is designed to run entirely on the client side, avoiding the need for server-side logic. This approach simplifies deployment and reduces hosting requirements.

- **Simple Technology Stack**: The application is built using [TailwindCSS](https://tailwindcss.com) and [AlpineJS](https://alpinejs.dev). TailwindCSS provides utility-first CSS classes for styling, while AlpineJS offers reactive and declarative JavaScript for handling interactivity. This combination results in a comparatively lightweight and maintainable codebase.

## Contributions

Contributions to this project are welcome.
If you have ideas for improvements or have found bugs, please feel free to contribute.
You can submit your contributions via GitHub at <https://github.com/maksimkurb/asn-barcode-label-generator>.

## Acknowledgments

This project has been made possible with the support and sponsorship of [BauCloud GmbH](https://www.baucloud.com).

Special thanks to [Marvin Gaube](https://margau.net) for the insightful blog post ["paperless-ngx with qr codes as ASN: My Workflow"](https://margau.net/posts/2023-04-16-paperless-ngx-asn/). His workflow greatly inspired the development of this application.

Additionally, this project drew inspiration from the CLI tool [paperless-asn-qr-codes](https://git.jcg.re/jcgruenhage/paperless-asn-qr-codes) developed by [Jan Christian Grünhage](https://jcg.re). His work follows the same goal of streamlining the process of creating ASN labels for paperless-ng, but uses a different approach.

## License

This project is licensed under the [GNU Affero General Public License v3.0 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0.html).

All rights reserved by [Tobias L. Maier](https://tobiasmaier.info).
Fork by [Maxim Kurbatov](https://kurb.me).
