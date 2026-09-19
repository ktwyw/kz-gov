# Government and public services of Kazakhstan

A one-page directory of the official sites of Kazakhstan's state bodies and
the online services people actually use — eGov, tax and customs, courts,
pensions, licences, procurement, the National Bank — plus the emergency and
help-line numbers. 59 entries in six groups, with a search box.

Plain HTML, CSS and JavaScript; no build step, no dependencies.

Live: https://ktwyw.github.io/kz-gov/

Companion to [kz-universities](https://github.com/ktwyw/kz-universities),
[kz-companies](https://github.com/ktwyw/kz-companies) and
[kz-media](https://github.com/ktwyw/kz-media).

## What's in it

- **President, Kurultai and Government** — Akorda, the new unicameral
  Kurultai, the Prime Minister's site, the gov.kz portal, the election commission
- **Ministries** — all 21, linked to their pages on gov.kz using the slugs
  from the Prime Minister's official list of state bodies
- **Agencies and oversight** — financial regulator, financial monitoring,
  anti-corruption, civil service, KNB, Supreme Audit Chamber, statistics,
  Ombudsman
- **Courts and justice** — Constitutional Court, Supreme Court, prosecutors,
  the Adilet legal database, police
- **Everyday services** — eGov, e-Otinish, service centres, digital
  signature, tax cabinet, e-invoices, e-licence, labour exchange, pension
  fund, health insurance, procurement, university testing, Bolashak
- **Finance and open data** — National Bank, AIFC, Kazakh Invest, open data,
  open budgets, open legal acts

## Why gov.kz links

Since 2020 every ministry, agency and regional administration has its page
on the single portal gov.kz at `gov.kz/memleket/entities/<slug>`. Old
standalone domains mostly redirect there, and the slugs survive renamings
better than domains do, so those are the links used here.

## How to add or correct an entry

All data lives in one array near the top of the script in `index.html`:

```js
["Name", "https://site", "Group", "one-line note"],
```

`G + "slug"` is shorthand for a gov.kz entity page. Add a line in the right
group and open a pull request.

## Notes

- Verified in September 2026 against primeminister.kz (state bodies list),
  gov.kz entity pages and the services' own sites.
- The 2026 Constitution took effect on 1 July 2026: the bicameral Parliament
  became the unicameral Kurultai (quryltai.kz), a vice-presidency was created,
  and Constitution Day moved to 15 March. Ministries are reorganised from time
  to time; the AI and Digital Development ministry dates from September 2025.
- Not legal advice. For anything with a deadline or a fee, confirm on the
  service's own site or by calling 1414.

## Ideas for next steps

- Add the 20 regional and city akimats (all on gov.kz)
- Add embassies and consulates abroad
- Kazakh and Russian interface
