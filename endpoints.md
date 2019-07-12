### Endpoints

1) Venue/Business details are POSTed to DB by Business
2) Deals are appended (PATCH/PUT) to profile as a secondary index
3) Live deals are pulled (GET) by user/customer (where active = true)
4) User/Customer clicks on paper/deal and GETs venue info
5) When timer on deal runs out, PATCH request sent to change deal from: active: true to active: false

5) Unique coupons generated -> Deal posted -> copupons generated -> called equentially -> when used PATCH coupon from active: true to active: false -> when deal reached zero returns "Deal sold out"
6) Create a CRON Lambda that posts inactive deals to inactive deals table for archiving and deletes data from active/live table
