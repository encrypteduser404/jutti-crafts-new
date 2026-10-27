<img width="1915" height="1078" alt="image" src="https://github.com/user-attachments/assets/e2e5a3ae-e91d-4e92-8ddd-481f89d402b2" />
# JuttiCrafts

A single-page storefront for handcrafted Indian footwear, built with HTML, vanilla JavaScript, and Tailwind CSS via CDN.

## Open the website

Open `index.html` in a modern web browser. The product images are local PNG files in the project directory, so keep them alongside `index.html`:

- `gereen-latkan.png`
- `thar-royal.png`
- `bold-step-tpr-black.png`
- `badami-pink.png`
- `badami-grey.png`
- `lahariya.png`
- `pubjabi-floral.png`

The site loads Tailwind CSS, Google Fonts, and Phosphor icons from external CDNs, so those features require an internet connection.

## Shopping features

- Browse featured designs and the full collection.
- Open a dedicated product page from a product card. Product pages use URL hashes such as `#product-1`; browser Back and the Back to Collection link return to the storefront.
- Select a configured footwear size and quantity before adding a product or using Buy Now.
- Add products to the cart, update quantities, and remove items. Separate sizes of the same product are kept as separate cart lines.
- Continue through the existing checkout, payment-method selection, order confirmation, and printable invoice flow.
- Cart contents are saved in browser `localStorage` under the `jutti_cart` key.

## Product data

The catalogue and its descriptions are defined in the `products` array inside `index.html`. Each product includes its image path, price, category, descriptions, highlights, styling guidance, and `sizeOptions`.

The size options are configurable examples; the project does not include an inventory or size-availability system. Update each product's `sizeOptions` to match the sizes actually offered. The interface does not claim that a size is in stock.

## Notes

- Shipping and GST values are defined in `index.html` and shown during checkout.
- This project is a static front-end demonstration. The checkout simulates order processing in the browser; it is not connected to a payment provider, order service, or fulfilment system.
- Tailwind's CDN script is convenient for local use, but Tailwind recommends a build-based setup for production deployments.
