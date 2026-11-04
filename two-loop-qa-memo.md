

# IMPLEMENTATION MEMO: LOOP 1/LOOP 2 SYNTHESIS & ACTION ITEMS
**Scope:** Ad Evidence Gallery, Site Navigation, Inline Sourcing, QA Protocol  
**Status:** Implementation-Ready | **Performance Data:** None Inferred

---

## 1. ASSET MANAGEMENT: KEEP / ADD / REMOVE
### ✅ KEEP (7 Primary Gallery Assets)
*These are the only individual-ad crops to retain in the primary gallery.*
1. `google_4allfamily_ad_card_01.png`
2. `google_4allfamily_ad_card_02.png`
3. `google_4allfamily_ad_card_03.png`
4. `breezypacks_google_ad_3.webp`
5. `meta_4allfamily_ad_card_kate_hall_harnden.png`
6. `meta_4allfamily_ad_card_bainybt1d.png`
7. `meta_4allfamily_ad_card_direct_response.png`

### ➕ ADD (3 Supplemental/Verification Assets)
1. Fresh crop of `google_4allfamily_ad_card_04.png` *(verify readability before embedding)*
2. Meta “52h/72h” claim crop
3. Type1sami “storing insulin saves money” video crop

### 🗑️ REMOVE (From Primary Gallery)
- **All generic/full-page screenshots** and landing-page captures. Retain only as internal audit artifacts.
- **Page-level ad counts** (e.g., “Google: 27, Meta ~35”). Move to appendix/metadata only; visibility ≠ creative strategy.
- **Unqualified compliance claims** (“TSA-Approved,” “Medical-Grade,” “Guaranteed 48h”). Replace with auditable, test-condition language.

---

## 2. GALLERY STRUCTURE & PLATFORM GAPS
| Section | Content | Annotation Requirement |
|---------|---------|------------------------|
| **1. Google Ads** | 4–5 assets | `Source: Google Ad Library, [Date]` |
| **2. Meta Ads** | 4–5 assets | `Source: Meta Ad Library, [Date]` |
| **3. Platform Gaps** | TikTok note only | *“TikTok query returned blank/JS-only interface. This indicates platform accessibility limitation, not absence of ads. No ad-level evidence is available for verification.”* |

---

## 3. NAVIGATION & ANCHOR CORRECTIONS
All 8 required anchors exist in the outline but require explicit HTML/Markdown implementation and duplicate cleanup.

| Anchor | Status | Action Required |
|--------|--------|-----------------|
| `#decision` | Present | Implement `<a id="decision">` at Section 1 header |
| `#market` | Present | Implement `<a id="market">` at Section 2 header |
| `#competitors` | Present | Implement `<a id="competitors">` at Section 3 header |
| `#ads` | Present | Implement `<a id="ads">` at Section 4 header |
| `#paid-growth` | Present | **Remove duplicate** in Section 7; retain only in Section 6 |
| `#audiences` | Present | Implement `<a id="audiences">` at Section 5 header |
| `#roadmap` | Present | Implement `<a id="roadmap">` at Section 8 header |
| `#references` | Present | Implement `<a id="references">` at Section 11 header |

**Rule:** All anchors must be lowercase, hyphenated, unique, and clickable. Sticky nav links must use `<a href="#...">` syntax matching target sections.

---

## 4. INLINE SOURCE LINK IMPLEMENTATION
**Missing:** ~8 inline citations near factual claims in Sections 2–6.  
**Placement Rule:** Inline links must appear within 1–2 sentences of the claim they support. Use `[n]` markers mapping to Section 11 References.

| Claim Category | Required Inline Link Format |
|----------------|-----------------------------|
| Competitor ad counts | `[Source: Google Ad Library, 4AllFamily domain; Ref [40], [41], [9]]` |
| Hooks/Claims (“TSA-Ready,” “No Ice,” “52h/72h”) | `[Source: Ad Library crops, e.g., google_4allfamily_ad_card_02.png]` |
| Creator Ads (“Myles Above T1D”) | `[Source: Meta Library ID / Saved Page Text, Ref [9]]` |
| Platform Gaps (TikTok) | `[Source: TikTok Public Query URL, Ref [28]]` |
| Thermal/Battery Claims | `[Source: FDA Insulin Storage Guidance; FAA Battery Regulation (14 CFR § 175.10)]` |

---

## 5. LINK-QA & COMPLIANCE CHECKLIST
- [ ] All 8 anchors resolve correctly to target sections; no duplicate IDs exist.
- [ ] All `[n]` citations match active, non-redirecting URLs in Section 11.
- [ ] External library links (Google/Meta/TikTok/FDA/FAA) open without login walls, 404s, or JS-only skeletons.
- [ ] All external links include `rel="noopener noreferrer"`.
- [ ] Anchor text is descriptive and matches target heading.
- [ ] Inline source links are placed within 1–2 sentences of claims.
- [ ] Gallery contains only card-level creative evidence; page-level counts moved to appendix.
- [ ] **Zero performance metrics** (CPC, ROAS, CAC, spend, reach, effectiveness) present in copy, captions, or metadata.
- [ ] TikTok gap explicitly documented as accessibility limitation, not strategic absence.

---

## NEXT STEPS
1. **Loop 1:** Swap gallery assets, restructure sections, inject TikTok gap note, move counts to appendix.
2. **Loop 2:** Inject 8 inline source links, verify `<a id>` implementation, remove duplicate `#paid-growth`.
3. **QA:** Run checklist against rendered HTML/Markdown. Confirm all anchors resolve, links open cleanly, and no inferred metrics remain.

**Deliverable:** Sourced, navigable, and auditable ad intelligence brief ready for publication.