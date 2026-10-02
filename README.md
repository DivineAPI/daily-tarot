# Daily Tarot API (moved)

This repository is archived. The maintained DivineAPI docs and examples for the Daily Tarot API are in
**[DivineAPI/tarot-api](https://github.com/DivineAPI/tarot-api)**.

The old `divineapi.com/api/1.0/...php` URLs shown in earlier versions of this repo are not the current API.
The current endpoint returns a daily tarot card (upright or reversed) with career, love and finance readings and two card image URLs.

## Current endpoint

`POST https://astroapi-5.divineapi.com/api/v2/daily-tarot`

Auth: your auth token as an `Authorization: Bearer` header and your API key as the `api_key` form field
(never in the URL). `lan` sets the response language (default `en`).

```bash
curl -X POST "https://astroapi-5.divineapi.com/api/v2/daily-tarot" \
  -H "Authorization: Bearer YOUR_AUTH_TOKEN" \
  -F "api_key=YOUR_API_KEY" \
  -F "lan=en"
```

Real response (2 Oct 2026, trimmed with `...`):

```json
{
  "success": 1,
  "data": {
    "card": "KNIGHT OF WANDS",
    "category": "Upright",
    "career": "The card indicates that this is a good time to join a business and compliment people for t...",
    "love": "Someone new is going to be coming in your life and you are going to find yourself having a...",
    "finance": "The card indicates that money is going to be coming your way, especially because of the ha...",
    "image": "https://divineapi.com/admin/uploads/daily_tarot/27_2.jpg",
    "image2": "https://divineapi.com/admin/uploads/daily_tarot/27.jpg"
  }
}
```

## Links

- API reference: https://developers.divineapi.com/horoscope-and-tarot-api/daily-tarot
- Maintained repo: https://github.com/DivineAPI/tarot-api
- Get an API key: start the 14-day free trial (credit card required to activate the trial) at https://divineapi.com/start-trial
