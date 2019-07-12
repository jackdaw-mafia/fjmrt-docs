# Endpoints

## 1) api/owners/:owner_id - POST

Business details posted to database by owner.

## 2) api/owners/:owner_id - PUT

Deals are appended to profile as a secondary index and sent out to app users.

## 3) api/offers - GET

Shows list of most recent/active offers.

## 4) api/offers/:owner_id GET

User gets venue details when clicking on offer.

## 5) api/owners/:owner_id PATCH

When timer on deal runs out, PATCH request sent to change deal from: active: true to active: false.

## 6) api/owners/:owner_id DELETE

Owner can delete themselves from the site.

---Maybe---

6. Unique coupons generated -> Deal posted -> copupons generated -> called equentially -> when used PATCH coupon from active: true to active: false -> when deal reached zero returns "Deal sold out"
7. Create a CRON Lambda that posts inactive deals to inactive deals table for archiving and deletes data from active/live table
