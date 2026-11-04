# VialCool Ad Intelligence Evidence Pack — Loop 1 Refresh

## Capture quality rule
Loop 1 replaces generic full-page screenshots in the primary gallery with readable crops of individual competitor ad cards. Each image below is a crop from a public transparency/ad-library page and is paired with the underlying public page URL. It documents visible creative and copy, not spend or performance.

## Google Ads Transparency Center — individual ad cards

Public advertiser page: https://adstransparency.google.com/?region=US&domain=4allfamily.com

The U.S. domain page showed 27 ads for 4AllFamily. The individual card crops are:

- `/home/ubuntu/vialcool_ad_assets/google_4allfamily_ad_card_01.png` — “Medication Cooler Travel Case - Travel…” with product image and portability/safety copy.
- `/home/ubuntu/vialcool_ad_assets/google_4allfamily_ad_card_02.png` — “Travel Cooler For Medication - Best Medication Cooler Case” with insulin/GLP-1 and all-day cooling copy.
- `/home/ubuntu/vialcool_ad_assets/google_4allfamily_ad_card_03.png` — “4AllFamily Travel Cooler - TSA Approved Medication Cooler” with multi-vial/pen fit and USB insulin-cooler links.
- `/home/ubuntu/vialcool_ad_assets/google_4allfamily_ad_card_04.png` — “TSA Approved - Medication Cooler Travel Case” with lightweight/durable/travel copy and product image.

Individual creative detail route inspected: https://adstransparency.google.com/advertiser/AR08568207486320902145/creative/CR18151391825737285633?region=US. Google exposed ad-level metadata including advertiser, U.S. visibility, last shown date, and text format, while the detail creative area was not reliably rendered as a readable standalone image in the browser. The card crops are therefore the primary visual assets.

Public BreezyPacks domain page: https://adstransparency.google.com/?region=US&domain=breezypacks.com

The U.S. domain page showed 8 ads under verified advertiser Innolou inc. The readable individual card crop remains `/home/ubuntu/vialcool_ad_assets/breezypacks_google_ad_3.webp`, with “Worldwide Shipping - Cooling Case” and cooling/travel copy. The page also exposed “No Electricity Needed - TSA-Approved” and “No Ice Packs Needed” themes. A fresh crop should be treated as a card-level capture only when its text is readable; the full page screenshot is retained as a source audit artifact, not as the primary gallery image.

## Meta Ad Library — individual advertiser cards

Public advertiser page: https://www.facebook.com/ads/library/?id=1264674129085890

The 4AllFamily advertiser page showed approximately 35 active ads. Fresh card-level crops from the visible U.S. advertiser page are:

- `/home/ubuntu/vialcool_ad_assets/meta_4allfamily_ad_card_kate_hall_harnden.png` — creator ad; “First time flying with my two babies,” diabetic supplies, Nomad Pro, temperature display, and TSA-friendly framing. Library ID 961068976477148; started Oct. 7, 2026.
- `/home/ubuntu/vialcool_ad_assets/meta_4allfamily_ad_card_bainybt1d.png` — creator ad; “Traveling with insulin,” T1D family context, Pioneer cooler, reliable temperature, less worry. Library ID 1423527386422665; started Oct. 8, 2026; #AD.
- `/home/ubuntu/vialcool_ad_assets/meta_4allfamily_ad_card_direct_response.png` — direct-response ad; built for travel/real life, Nomad/Voyager/Chiller, free delivery/free returns. Library ID 1328441539368670; active.

The same public page exposed additional individual records: Myles Above T1D vacation/heat creative, a direct-response “52 hours refrigerated / 72 hours below 79°F” creative, and a Type1sami “storing insulin saves money” short video. These are supported by the saved page text at `/home/ubuntu/page_texts/www.facebook.com_ads_library__active_status_active_ad_type_all_country_US_id_1264674129085890_is_tar.md`.

## TikTok — direct individual evidence attempt

Public ad-library query: https://library.tiktok.com/ads?region=US&search_term=insulin%20cooler

The public query returned a blank/JavaScript-only page in the browser session. The public hashtag page https://www.tiktok.com/tag/insulcool also returned a login/skeleton view with no readable individual video cards. No TikTok ad screenshot is included because a blank or login skeleton would be misleading. This is an explicit platform evidence gap, not an inferred absence of advertising.

## Loop 1 model input

The open-weight ensemble should rank the individual card captures by readability and strategic usefulness; separate card-level evidence from page-level counts; identify which claims are repeated across Google and Meta; and recommend which exact assets belong in the primary site gallery. It should not infer spend, impressions, CPC, CAC, ROAS, or performance from library presence.
