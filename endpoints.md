# Endpoints

## 1) api/owners/:owner_id - GET

Business owners can see their own details.

## 2) api/owners - POST

Business details posted to database by owner.

## 2.5) api/owners/:owner_id - PATCH

Business owner can update their information.

## 3) api/owners/:owner_id - POST

New deal is posted by the owner and sent out to app users.

## 4) api/offers - GET

Shows list of most recent/active offers.

## 5) api/offers/:owner_id - GET

User gets venue details and most recent offers when clicking on offer.

## 6) api/owners/:owner_id/:offer_id - PATCH

When timer on deal runs out, PATCH request sent to change deal from: active: true to active: false.

## 7) api/owners/:owner_id - DELETE

Owner can delete themselves from the site.

## 8) api/owners/:owner_id/offers - GET

Owner can view a list of all their offers ordered by most recent.

---Maybe---

6. Unique coupons generated -> Deal posted -> copupons generated -> called equentially -> when used PATCH coupon from active: true to active: false -> when deal reached zero returns "Deal sold out"
7. Create a CRON Lambda that posts inactive deals to inactive deals table for archiving and deletes data from active/live table
