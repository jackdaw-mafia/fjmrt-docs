# Endpoints

\* denotes completed endpoints as shown on the api route.

## 1) api - GET \*

Shows all available endpoints.

## 2) api/owners/:id - GET

Business owners can see their own details.

## 3) api/owners - POST \*

Business details posted to database by the owner.

## 4) api/owners/:id - PATCH \*

Business owner can update their information.

## 5) api/offers - POST \*

New deal is posted by the owner and sent out to app users.

## 6) api/offers - GET \*

Shows list of most recent/active offers.

## 7) api/offers/:id - GET

User gets venue details and most recent offers when clicking on offer.

## 8) api/owners/:owner_id/:offer_id - PATCH

When timer on deal runs out, PATCH request sent to change deal from: active: true to active: false.

## 9) api/owners/:id - DELETE \*

Owner can delete themselves from the site.

## 10) api/owners/:owner_id/offers - GET

Owner can view a list of all their offers ordered by most recent.

---Maybe---

Unique coupons generated -> Deal posted -> copupons generated -> called equentially -> when used PATCH coupon from active: true to active: false -> when deal reached zero returns "Deal sold out"
Create a CRON Lambda that posts inactive deals to inactive deals table for archiving and deletes data from active/live table
