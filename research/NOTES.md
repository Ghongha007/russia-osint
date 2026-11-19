# Research notes (checked 2026-11-19, from a non-Russian IP, via curl)

167 entries: 103 ok, 53 unreachable, 11 changed.

**Access from outside Russia.** Most federal .gov.ru and .ru state sites (Rosstat, zakupki, Fedresurs, Rosreestr/NSPD, SOZD, pravo.gov.ru, mil.ru, CEC) timed out from our checker: the connection is dropped, not refused, which is consistent with geo-blocking of foreign IPs. Several private Russian aggregators (Rusprofile, List-org, Checko) returned 403. Expect to need a Russian connection for many of them. Separately, Cloudflare bot checks blocked our script (not geography) on ISW, Proekt, ACF, Verstka, TGStat and GEM wiki. Unreachable entries were kept only where the URL was confirmed by a Wayback Machine capture or other sources; the capture date is in each note.

## (a) Moved or died

- **War & Sanctions:** sanctions.nazk.gov.ua timed out (last Wayback capture October 2024); the same portal loads at war-sanctions.gur.gov.ua, run by Ukraine's Defence Intelligence (HUR).
- **Minjust registers:** the foreign agents (documents/7755) and undesirable organisations (documents/7756) links return 404. Replaced with the current /ru/pages/ addresses.
- **Other moves:** bo.nalog.ru to bo.nalog.gov.ru; sbis.ru to saby.ru (rebrand); data.ovdinfo.org to data.ovd.info; rivreg.ru to rfclass.ru (Russian Classification Society); soar.earth to soaratlas.com; globalforestwatch.org to globalnaturewatch.org; yandex.ru home now goes to dzen.ru, search at ya.ru; bis.gov/entity-list redirects into the regulations; pkk.rosreestr.ru replaced by nspd.gov.ru/map (confirmed by regional government notices).
- **service.nalog.ru** address-check tool (addrfind.do) now redirects to pb.nalog.ru; dropped as a separate entry.
- **Dead, dropped:** warfare.be (domain for sale); loadmap.net (parked); reestr.rublacklist.net (Roskomsvoboda block register, HTTP 500, last capture 2022); ach.gov.ru/opendata (404); duma.mos.ru (no capture since 2014).

## (b) Unsure

- **Blocked and only weakly confirmed:** sozd.duma.gov.ru and budget.gov.ru (last Wayback capture 2022), izbirkom.ru (no recent capture), cikrf.ru (2023), customs.gov.ru/statistic (2022), morflot.gov.ru (2022), reformagkh.ru (2023). These are long-standing official addresses, but we could not see the current pages.
- **torgi.gov.ru/new/public** and **zakupki.gov.ru** never loaded; confirmed by a 2025 Rosimushchestvo document and a May 2026 Wayback capture respectively.
- **Customs statistics:** FTS publishes headline trade totals again (reported in 2025 to 2026 news) but detailed data remains restricted; exact page contents not seen.
- **2GIS** redirected our script to a splash page; it loads as 2GIS but search was not tested. **Sokr.ru** and **OCCRP Aleph** are JavaScript apps; shell loaded, content not machine-verified.
- **Access values** are from prior knowledge plus page loads, not from running every search form. Captcha frequency on EGRUL and kad.arbitr.ru varies.
- "Declared undesirable" and "foreign agent" labels were checked against news reports of each designation on 2026-11-19 (undesirable status is set by the Prosecutor General and entered on the Ministry of Justice register; extremist and terrorist labels come from court rulings and the Rosfinmonitoring list). Designations change often; check the registers before relying on them. The old transparency.org.ru domain now hosts an unrelated loan site; the entry points to TI Russia in exile.
- Dropped KSE "Russia Will Pay" (it documents war damage in Ukraine, off scope). Trimmed 26 weaker entries (for example Japan and Australia sanctions lists, Garant, HUDOC, VesselFinder) to stay under 170; they all loaded except DFAT and the World Bank.

## (c) Prior art on GitHub

| Repo | Last push | Size |
|---|---|---|
| [paulpogoda/OSINT-Tools-Russia](https://github.com/paulpogoda/OSINT-Tools-Russia) | 2026-10-13 | 96 stars, ~56 links in README |
| [lorien/ru-osint-infosec-map](https://github.com/lorien/ru-osint-infosec-map) | 2023-08-07 | 45 stars; graph of Russian-language OSINT and infosec resources (nodes.json, 47 KB) |
| [nixintel/sansosintsummit2024](https://github.com/nixintel/sansosintsummit2024) | 2024-02-29 | 11 stars, ~25 links (talk "OSINT On The Russian Internet") |
| [OSINT-mindset/osint-cases-ru](https://github.com/OSINT-mindset/osint-cases-ru) | 2024-04-26 | 29 stars; case write-ups, not a link list |

There is no OSINT-for-countries Russia repo (unlike India). Many other GitHub hits for "Russia OSINT" are live war dashboards (e.g. NoblerWorks-HQ/IRONSIGHT) or people-search and username tools.

## Deliberately excluded

People-search services, phone, passport, SNILS and vehicle-owner lookups, Telegram "probiv" bots, leaked or breached databases (such as leaked delivery-service or food-delivery data), and tools that de-anonymise private individuals. Aleph and ICIJ Offshore Leaks are included because they are curated by newsrooms and focus on companies and public figures; their notes flag the leaked origin of some data.
