# Analytics Plan

## Event Taxonomy (v1)
- `app_open`
- `search_performed` {query, location, radius_km}
- `listing_viewed` {venue_id}
- `slot_selected` {venue_id, slot_id, price}
- `payment_initiated` {method}
- `payment_succeeded` {amount}
- `booking_confirmed` {booking_id}
- `booking_cancelled` {reason}
- `review_submitted` {rating}
- `referral_sent` {channel}

## Core Funnels
1. Search → Listing → Slot → Pay Success
2. Listing → Review → Booking
3. Onboarding: Venue Created → Photos Uploaded → Slots Configured → First Booking

## Quality & Alerting
- Monitor pay success rate; alert if < 95% for 15 mins.
- Anomaly detection on cancellations/refunds.
- Weekly cohort retention & repeat booking dashboards.
