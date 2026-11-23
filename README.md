# Pestable Price Check

A one-page pricing calculator for technicians: `index.html`. There's no build step and no server, and it works on any phone.

It matches the Price check page in the Pest CRM (the same prices, postcode lookup and diesel maths) and adds a few extras.

## What it does
1. Type the postcode on the number pad, or start typing the suburb. Every suburb in Sydney, the Central Coast and the Illawarra is built in (1,335 of them) and it works offline.
2. Tap the service(s). You can pick more than one.
3. Tap the property: Unit, Granny flat, Single storey or Double storey. This sets the General pest range.
4. Tap **Lowest / Usual / Highest**, or type a price. It warns if the price is below the lowest or above the top.
5. Read the quote: the range, the lowest to go, the distance from Potts Hill, the diesel cost, a travel add-on (Fuel / +$20 / +$30, marked "suggested" past 30 km), the total, and what's left after diesel.
6. **Copy**, **Text** or **WhatsApp** the quote to the customer.

## Prices
These are at the top of the `<script>` in `index.html` (`SERVICES`, `PROPERTY`, `VEHICLE_DEFAULTS`).
- General pest by property: Unit $120–189, Granny $150–200, Single $180–289, Double $250–300.
- Other services come from 173 CRM bookings. Jobs at $100 or under are left out.

## Publish with GitHub Pages
Go to Settings → Pages → Deploy from a branch, pick the branch and `/ (root)`, then save.
The link will be `https://<user>.github.io/pricingcal/`.

Suburb locations come from the matthewproctor/australianpostcodes list.
