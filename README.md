# Pestable Price Check

A one-page pricing calculator for technicians: `index.html`. There's no build step and no server, and it works on any phone.

## What it does
1. Tap the service(s). You can pick more than one.
2. Tap the property: Unit, Granny flat, Single storey or Double storey. This sets the General pest range.
3. Tap **Lowest / Usual / Highest**, or type a price. It warns if the price is below the floor or above the top.
4. Type the suburb or postcode, or the km. It shows the distance from Potts Hill, the diesel cost and the travel add-on (Fuel / +$20 / +$30).

## Prices
These are at the top of the `<script>` in `index.html` (`SERVICES`, `PROPERTIES`).
- General pest by property: Unit $120–189, Granny $150–200, Single $180–289, Double $250–300.
- Other services come from 173 CRM bookings. Jobs at $100 or under are left out.

## Publish with GitHub Pages
Go to Settings → Pages → Deploy from a branch, pick the branch and `/ (root)`, then save.
The link will be `https://<user>.github.io/pricingcal/`.
