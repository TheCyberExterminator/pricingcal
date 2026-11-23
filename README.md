# Pestable Price Check

A one-page pricing calculator for technicians: `index.html`. There's no build step and no server. It's made for iPhone 13 Pro Max to 16 Pro Max, works offline once loaded, and has a dark mode for night.

It matches the Price check page in the Pest CRM (same prices, postcode lookup and diesel maths) and adds the extras below.

## How a tech uses it
1. **Where:** type the postcode, tap **📍 I'm at the job** (GPS), or tap a recent suburb. All 1,335 suburbs in Sydney, the Central Coast and the Illawarra are built in.
2. **Pest:** big tiles with icons, tap all that apply.
3. **Property:** sets the general pest range.
4. **Price:** drag the slider left to right through **Low** (amber), **Medium** (green) and **High** (blue). It moves in $5 steps and the price and band show big. You can also tap Low / Medium / High, nudge with **−5 / +5**, or type a price. It warns below the lowest or above the top.
5. **Quote:** the range, the lowest to go, km, drive time (normal and peak), diesel, the travel add-on, the total and what's left after diesel. **Copy / Text / WhatsApp** sends it to the customer.

The total stays pinned at the bottom of the screen the whole time.

## Settings (top of the `<script>` in index.html)
- `SERVICES`, `PROPERTY`: prices.
- `VEHICLE_DEFAULTS`: diesel $2.38/L, 11 L/100 km (the quote also shows the cost at 10–12 L), return trip.
- Drive time: the first 10 km at 35 km/h, then 65 km/h, and +50% in peak hour.
- Techs can change diesel, fuel use and "drive from" (Potts Hill or their GPS location) on the phone.

## Publish with GitHub Pages
Go to Settings → Pages → Deploy from a branch, pick the branch and `/ (root)`, then save. The link will be `https://thecyberexterminator.github.io/pricingcal/`. GPS needs that https link. On the iPhone, use Safari → Share → **Add to Home Screen** so it opens like an app.

Suburb locations come from the matthewproctor/australianpostcodes list.
