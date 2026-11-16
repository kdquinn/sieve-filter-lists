# Sieve filter lists

These are the content-blocker lists bundled with **Sieve**, a Safari ad, tracker and annoyance blocker for iPhone.

They're published here because most of them are adaptations of lists licensed under
[CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/), which asks that adapted versions be shared under the same license.
The Sieve app itself is a separate project; its code isn't part of this repository.

## What's in this repository

| Path | What it is |
|---|---|
| `Rules/catalog.json` | Every filter Sieve offers: its name, description, source and rule count |
| `Rules/<filter>.txt` | One filter, converted to [Safari content-blocker JSON](https://developer.apple.com/documentation/safariservices/creating-a-content-blocker) |
| `FILTER-LICENSES.md` | The source list and license for every file |

Each `Rules/<filter>.txt` file has exactly three lines, and each line is a JSON array of Safari rules:
1. Block and hide rules
2. Exceptions (`ignore-previous-rules`)
3. Important rules, which take priority over exceptions

## Where the lists come from

| Source | License | Website |
|---|---|---|
| EasyList, EasyPrivacy and the EasyList Cookie, Newsletter, Annoyances, AI, Notifications and Chat lists | CC BY-SA 3.0 (dual-licensed with GPL-3.0; used here under CC BY-SA) | https://easylist.to |
| Fanboy's Social Blocking List | CC BY-SA 3.0 | https://easylist.to |
| EasyList Germany | CC BY-SA 3.0 | https://easylist.to |
| RU AdList | CC BY 3.0 | https://github.com/easylist/ruadlist |
| malware-filter: URLhaus, Phishing and PUP lists | CC0 1.0 | https://gitlab.com/malware-filter/malware-filter |
| NoCoin adblock list | MIT | https://github.com/hoshsadiq/adblock-nocoin-list |
| Lists written for Sieve: company blockers, focus mode, data saver, site-specific ad rules and others | CC BY-SA 3.0 | — |

Thank you to the maintainers of these lists. They do the hard work of tracking ads and trackers across the web.

## Changes from the original lists

The original lists use adblock filter syntax. For Sieve they were:
- **Converted** to Safari's content-blocker JSON format.
- **Trimmed** of rules Safari can't run, such as scriptlets, redirects and procedural selectors.
- **Supplemented**, in a few files, with rules written for Sieve. These are noted in `FILTER-LICENSES.md`.

No other changes were made to what the lists block.

## License

Each file keeps the license of the list it was adapted from, as listed in `FILTER-LICENSES.md`. See `LICENSE.md` for details.
