# Campaign Calendar Structure & Automation Flow

## 1. Core Cadence & Weekly Rhythm
To maintain consistency without overwhelming the audience, the automated calendar will follow a 4-post-per-week structure across primary platforms (Facebook, Instagram, Nextdoor). 

**Weekly Thematic Structure:**
*   **Tuesday: The Transformation (Proof of Work)**
    *   *Content:* High-contrast Before/After photos or time-lapse Reels.
    *   *Objective:* Build trust and showcase quality.
*   **Thursday: The Expert Tip (Value Add)**
    *   *Content:* Short text or infographic (e.g., "Watering schedule for July", "How to spot grub damage").
    *   *Objective:* Establish authority and reciprocity.
*   **Friday: The Weekend Saver (Direct Response)**
    *   *Content:* Promotional post emphasizing time-saving. "Don't spend your Saturday sweating. Book our weekend prep package."
    *   *Objective:* Lead generation and immediate bookings.
*   **Sunday: Community/Behind-the-Scenes (Brand Affinity)**
    *   *Content:* Crew highlights, community involvement, or a beautiful local landscape shot.
    *   *Objective:* Humanize the brand and build local affinity.

## 2. Monthly Campaign Themes
The calendar will rotate through seasonal themes to ensure relevance:
*   **March/April:** Spring Cleanup & Pre-emergent Weed Control.
*   **May/June:** Growth Management & Fertilization.
*   **July/August:** Drought Defense & Irrigation Optimization.
*   **September/October:** Aeration, Overseeding, & Fall Cleanup.

## 3. Automation Flow & Data Schema
The campaign will be driven by a `campaign_calendar.json` file. The automation engine will read this file daily and execute posts.

**JSON Schema Structure:**
```json
{
  "campaign_name": "Spring Growth 2026",
  "posts": [
    {
      "platform": "instagram",
      "post_type": "image",
      "scheduled_date": "2026-04-14",
      "scheduled_time": "08:00",
      "text": "Transform your yard from an eyesore to an oasis. Swipe to see this week's cleanup in [Neighborhood]! #LawnCare #TransformationTuesday",
      "image": "before_after_spring.png",
      "hashtags": "#[City]LawnCare #[City]Landscaping #CurbAppeal",
      "cta_url": "https://example.com/quote"
    }
  ]
}
```

## 4. Email Nurture Sequence (Automated)
For leads captured via the website who do not immediately book:
*   **Day 1:** Welcome & Instant Quote Delivery.
*   **Day 3:** The "Why Us" (Reviews & Guarantees).
*   **Day 7:** Educational Value (Top 3 Lawn Mistakes in [City]).
*   **Day 14:** Scarcity/Offer (10% off first month if booked by Friday).