# Prompt 2: In-App & Post-Purchase Prompts

## Purpose
Generate micro-copy for review/rating requests inside products and at purchase moments. Covers SaaS modal dialogs, e-commerce order confirmations, and mobile app push notifications.

---

## The Prompt

```
You are a UX copywriter specializing in customer feedback and social proof collection. Generate in-product review prompts for a business.

BUSINESS INFO:
- Business name: [BUSINESS NAME]
- Business type: [SaaS web app / E-commerce / Mobile app (iOS/Android) / Local service / Other]
- Product/service: [BRIEF DESCRIPTION]
- Target review platform: [Google / App Store / G2 / Trustpilot / Amazon / Internal NPS only]
- Review link: [URL OR APP STORE LINK]
- Trigger moment: [When does this appear? E.g., "after user completes their 5th project", "after delivery confirmation", "after 30 days of active use", "after support ticket resolved"]
- Brand voice: [Formal / Friendly / Playful / Minimal]

GENERATE ALL OF THE FOLLOWING:

---

SECTION 1: MODAL DIALOG (for web/desktop apps)
Format:
- Headline (under 10 words)
- Body text (1-2 sentences, under 30 words)
- Primary CTA button: "Leave a Review"
- Secondary option: "Maybe Later" | "I'll skip this" | "Give private feedback instead"
- Dismiss sentiment: what text shows if they click "Maybe Later" (brief, no guilt)

Create 3 variants (A/B/C test options):
- Variant A: Outcome-focused (references what they've accomplished)
- Variant B: Community-focused (helping others like them find the tool)
- Variant C: Gratitude-focused (simple thank-you framing)

---

SECTION 2: POST-PURCHASE / ORDER CONFIRMATION PAGE INSERT
A box or section to add to the order confirmation email or thank-you page.
Format:
- Section headline
- 1-2 sentence ask
- CTA link text
Keep under 50 words total. Must not distract from order details.

---

SECTION 3: MOBILE PUSH NOTIFICATIONS (3 variants)
For mobile apps requesting App Store / Google Play ratings.
Each push notification:
- Title: under 6 words
- Body: under 20 words
- Timing note: when to send this variant

Variant 1: After first meaningful success moment
Variant 2: After 7 days of active use
Variant 3: After customer support resolution (if applicable)

---

REQUIREMENTS:
- Never use the word "please" more than once
- No dark patterns (no pre-selected stars, no guilt trips)
- Apple App Store review prompt must comply with SKStoreReviewRequest guidelines (no custom star UI, just native prompt trigger context)
- All copy should feel earned — user must have had a real win before seeing this
```

---

## How to Use

1. Fill in all bracketed fields
2. Run in Claude — get all 3 sections in one response
3. A/B test the 3 modal variants (run each for 2 weeks, pick highest click-through)
4. Implement push notifications via OneSignal, Braze, or your mobile push provider

---

## Trigger Timing Best Practices

| Business Type | Best Trigger Moment | Avoid |
|--------------|--------------------|----|
| SaaS | After 3rd login OR after completing first core workflow | At signup, after free trial ends |
| E-commerce | 7-10 days post-delivery | Day of purchase, before item arrives |
| Mobile app | After first meaningful use OR 7-day streak | First launch, during onboarding |
| Local service | Within 2 hours of service completion | Weeks later |
| Marketplace | After buyer confirms receipt | Before transaction completes |
