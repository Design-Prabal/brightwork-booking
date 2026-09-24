# Brightwork — booking prototype

An interactive prototype of a customer-facing booking experience for a home-repair business.
Static build, no backend — all data is mocked in the browser.

## What you can do

1. Browse services by category, or search
2. Tap one and give a zip code (any 6 digits works)
3. Pick an option and any extras
4. Choose a professional, then a time
5. Repeat for as many services as you like — each gets its own professional and slot
6. Check out with contact details and a card (nothing is charged)

Not sure what you need? Use **Request a home visit** instead — that path takes a description and
photos rather than booking a slot.

## Variations

The same pill opens a **Variations** section:

- **How the zip is asked** — a modal over the storefront (default), or a dedicated
  map screen where you enter a zip, watch the map redraw, drop a pin and confirm.
- **Service imagery** — on, or off for businesses that publish no photos. With it off
  the whole catalogue falls back to a text-only layout.

The storefront also has a card/list switcher next to the category chips.

## Previewing edge states

The dark pill in the bottom-left corner forces states that are otherwise hard to reach: no
services published, zip not serviceable, partial coverage, no availability, slot taken at payment,
payment declined, request submission failure, slow network.

## Notes

- Fictional business, services, staff, prices and reviews
- Card details are never sent anywhere; any 16 digits pass validation
- Rebuild with `npm run build` from the source project and copy `dist/` here
