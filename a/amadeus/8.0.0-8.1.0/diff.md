# Comparing `tmp/amadeus-8.0.0.tar.gz` & `tmp/amadeus-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amadeus-8.0.0.tar", last modified: Mon Jan 30 14:52:40 2023, max compression
+gzip compressed data, was "amadeus-8.1.0.tar", last modified: Thu Jun 22 14:51:33 2023, max compression
```

## Comparing `amadeus-8.0.0.tar` & `amadeus-8.1.0.tar`

### file list

```diff
@@ -1,159 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.772127 amadeus-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    15303 2023-01-30 14:52:02.000000 amadeus-8.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-01-30 14:52:02.000000 amadeus-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-01-30 14:52:02.000000 amadeus-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15370 2023-01-30 14:52:40.772127 amadeus-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14732 2023-01-30 14:52:02.000000 amadeus-8.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.748126 amadeus-8.0.0/amadeus/
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.748126 amadeus-8.0.0/amadeus/airline/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/airline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/airline/_destinations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.748126 amadeus-8.0.0/amadeus/airport/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/airport/_direct_destinations.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/airport/_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.748126 amadeus-8.0.0/amadeus/airport/predictions/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/airport/predictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/airport/predictions/_on_time.py
--rw-r--r--   0 runner    (1001) docker     (122)     3490 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/amadeus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.752126 amadeus-8.0.0/amadeus/analytics/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/analytics/_itinerary_price_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.752126 amadeus-8.0.0/amadeus/booking/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/booking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/booking/_flight_order.py
--rw-r--r--   0 runner    (1001) docker     (122)      926 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/booking/_flight_orders.py
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/booking/_hotel_bookings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.752126 amadeus-8.0.0/amadeus/client/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/access_token.py
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/direction.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/hotel.py
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/location.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/request.py
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/client/response.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.752126 amadeus-8.0.0/amadeus/duty_of_care/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/duty_of_care/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/duty_of_care/_diseases.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.756126 amadeus-8.0.0/amadeus/duty_of_care/diseases/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/duty_of_care/diseases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/duty_of_care/diseases/_covid19_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.756126 amadeus-8.0.0/amadeus/e_reputation/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/e_reputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/e_reputation/_hotel_sentiments.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.756126 amadeus-8.0.0/amadeus/location/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/location/_analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.756126 amadeus-8.0.0/amadeus/location/analytics/
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/location/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/location/analytics/_category_rated_areas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.756126 amadeus-8.0.0/amadeus/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/mixins/encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5586 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/mixins/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/mixins/pagination.py
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/mixins/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/mixins/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.760126 amadeus-8.0.0/amadeus/namespaces/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_airline.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_airport.py
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_booking.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_duty_of_care.py
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_e_reputation.py
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_location.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_reference_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_safety.py
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_schedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_shopping.py
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/_travel.py
--rw-r--r--   0 runner    (1001) docker     (122)     1138 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/namespaces/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.760126 amadeus-8.0.0/amadeus/reference_data/
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      640 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/_airlines.py
--rw-r--r--   0 runner    (1001) docker     (122)      647 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/_location.py
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/_locations.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/_recommended_locations.py
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.760126 amadeus-8.0.0/amadeus/reference_data/locations/
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/_airports.py
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/_cities.py
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/_hotel.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/_hotels.py
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/_point_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/_points_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.764126 amadeus-8.0.0/amadeus/reference_data/locations/hotels/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/hotels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/hotels/_by_city.py
--rw-r--r--   0 runner    (1001) docker     (122)      814 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/hotels/_by_geocode.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/hotels/_by_hotels.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.764126 amadeus-8.0.0/amadeus/reference_data/locations/points_of_interest/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/points_of_interest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/locations/points_of_interest/_by_square.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.764126 amadeus-8.0.0/amadeus/reference_data/urls/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/reference_data/urls/_checkin_links.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.764126 amadeus-8.0.0/amadeus/safety/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/safety/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/safety/_safety_rated_location.py
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/safety/_safety_rated_locations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.764126 amadeus-8.0.0/amadeus/safety/safety_rated_locations/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/safety/safety_rated_locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/safety/safety_rated_locations/_by_square.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.764126 amadeus-8.0.0/amadeus/schedule/
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/schedule/_flights.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.768126 amadeus-8.0.0/amadeus/shopping/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_activities.py
--rw-r--r--   0 runner    (1001) docker     (122)      640 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_activity.py
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_availability.py
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_flight_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_flight_destinations.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_flight_offers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1538 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_flight_offers_search.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_hotel_offer_search.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_hotel_offers_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/_seatmaps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.768126 amadeus-8.0.0/amadeus/shopping/activities/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/activities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/activities/_by_square.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.768126 amadeus-8.0.0/amadeus/shopping/availability/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/availability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/availability/_flight_availabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.768126 amadeus-8.0.0/amadeus/shopping/flight_offers/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/flight_offers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/flight_offers/_prediction.py
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/flight_offers/_pricing.py
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/shopping/flight_offers/_upselling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.768126 amadeus-8.0.0/amadeus/travel/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/_predictions.py
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/_trip_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.768126 amadeus-8.0.0/amadeus/travel/analytics/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/analytics/_air_traffic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.772127 amadeus-8.0.0/amadeus/travel/analytics/air_traffic/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/analytics/air_traffic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/analytics/air_traffic/_booked.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/analytics/air_traffic/_busiest_period.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/analytics/air_traffic/_traveled.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.772127 amadeus-8.0.0/amadeus/travel/predictions/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/predictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/predictions/_flight_delay.py
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/travel/predictions/_trip_purpose.py
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-01-30 14:52:02.000000 amadeus-8.0.0/amadeus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 14:52:40.748126 amadeus-8.0.0/amadeus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15370 2023-01-30 14:52:40.000000 amadeus-8.0.0/amadeus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-01-30 14:52:40.000000 amadeus-8.0.0/amadeus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-30 14:52:40.000000 amadeus-8.0.0/amadeus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-01-30 14:52:40.000000 amadeus-8.0.0/amadeus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-01-30 14:52:40.772127 amadeus-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-01-30 14:52:02.000000 amadeus-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    15939 2023-06-22 14:50:46.000000 amadeus-8.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-06-22 14:50:46.000000 amadeus-8.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-22 14:50:46.000000 amadeus-8.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15655 2023-06-22 14:51:33.081682 amadeus-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    15017 2023-06-22 14:50:46.000000 amadeus-8.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.061682 amadeus-8.1.0/amadeus/
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.065682 amadeus-8.1.0/amadeus/airline/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/airline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/airline/_destinations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.065682 amadeus-8.1.0/amadeus/airport/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/airport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/airport/_direct_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/airport/_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.065682 amadeus-8.1.0/amadeus/airport/predictions/
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/airport/predictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/airport/predictions/_on_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3490 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/amadeus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.065682 amadeus-8.1.0/amadeus/analytics/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/analytics/_itinerary_price_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.065682 amadeus-8.1.0/amadeus/booking/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/booking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/booking/_flight_order.py
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/booking/_flight_orders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/booking/_hotel_bookings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.065682 amadeus-8.1.0/amadeus/client/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/direction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/hotel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/location.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/client/response.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.065682 amadeus-8.1.0/amadeus/duty_of_care/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/duty_of_care/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/duty_of_care/_diseases.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.069682 amadeus-8.1.0/amadeus/duty_of_care/diseases/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/duty_of_care/diseases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/duty_of_care/diseases/_covid19_report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.069682 amadeus-8.1.0/amadeus/e_reputation/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/e_reputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/e_reputation/_hotel_sentiments.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.069682 amadeus-8.1.0/amadeus/location/
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/location/_analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.069682 amadeus-8.1.0/amadeus/location/analytics/
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/location/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/location/analytics/_category_rated_areas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.069682 amadeus-8.1.0/amadeus/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/mixins/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5586 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/mixins/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/mixins/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/mixins/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/mixins/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.073682 amadeus-8.1.0/amadeus/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_airline.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_airport.py
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_booking.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_duty_of_care.py
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_e_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_reference_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_safety.py
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_shopping.py
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/_travel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/namespaces/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.073682 amadeus-8.1.0/amadeus/ordering/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/ordering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/ordering/_transfer_order.py
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/ordering/_transfer_orders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.073682 amadeus-8.1.0/amadeus/ordering/transfer_orders/
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/ordering/transfer_orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/ordering/transfer_orders/_transfers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.073682 amadeus-8.1.0/amadeus/ordering/transfer_orders/transfers/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/ordering/transfer_orders/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/ordering/transfer_orders/transfers/_cancellation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.073682 amadeus-8.1.0/amadeus/reference_data/
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      640 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/_airlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)      647 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/_recommended_locations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.073682 amadeus-8.1.0/amadeus/reference_data/locations/
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/_airports.py
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/_cities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/_hotel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/_hotels.py
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/_point_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/_points_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.077682 amadeus-8.1.0/amadeus/reference_data/locations/hotels/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/hotels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/hotels/_by_city.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/hotels/_by_geocode.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/hotels/_by_hotels.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.077682 amadeus-8.1.0/amadeus/reference_data/locations/points_of_interest/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/points_of_interest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/locations/points_of_interest/_by_square.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.077682 amadeus-8.1.0/amadeus/reference_data/urls/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/reference_data/urls/_checkin_links.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.077682 amadeus-8.1.0/amadeus/safety/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/safety/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/safety/_safety_rated_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/safety/_safety_rated_locations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.077682 amadeus-8.1.0/amadeus/safety/safety_rated_locations/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/safety/safety_rated_locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/safety/safety_rated_locations/_by_square.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.077682 amadeus-8.1.0/amadeus/schedule/
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/schedule/_flights.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/amadeus/shopping/
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_activities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      640 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_activity.py
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_availability.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_flight_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_flight_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_flight_offers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1538 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_flight_offers_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_hotel_offer_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_hotel_offers_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_seatmaps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/_transfer_offers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/amadeus/shopping/activities/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/activities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/activities/_by_square.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/amadeus/shopping/availability/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/availability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/availability/_flight_availabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/amadeus/shopping/flight_offers/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/flight_offers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/flight_offers/_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/flight_offers/_pricing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/shopping/flight_offers/_upselling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/amadeus/travel/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/_trip_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/amadeus/travel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/analytics/_air_traffic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/amadeus/travel/analytics/air_traffic/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/analytics/air_traffic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/analytics/air_traffic/_booked.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/analytics/air_traffic/_busiest_period.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/analytics/air_traffic/_traveled.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.081682 amadeus-8.1.0/amadeus/travel/predictions/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/predictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/predictions/_flight_delay.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/travel/predictions/_trip_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-22 14:50:46.000000 amadeus-8.1.0/amadeus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:33.061682 amadeus-8.1.0/amadeus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15655 2023-06-22 14:51:32.000000 amadeus-8.1.0/amadeus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4860 2023-06-22 14:51:32.000000 amadeus-8.1.0/amadeus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 14:51:32.000000 amadeus-8.1.0/amadeus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-22 14:51:32.000000 amadeus-8.1.0/amadeus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-22 14:51:33.081682 amadeus-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-06-22 14:50:46.000000 amadeus-8.1.0/setup.py
```

### Comparing `amadeus-8.0.0/CHANGELOG.rst` & `amadeus-8.1.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 Changelog
 =========
+8.1.0 - 2023-06-22
+--------------------
+Add support for the `Transfer Search API <https://developers.amadeus.com/self-service/category/cars-and-transfers/api-doc/transfer-search/api-reference>`_
+
+Add support for the `Transfer Booking API <https://developers.amadeus.com/self-service/category/cars-and-transfers/api-doc/transfer-booking/api-reference>`_
+
+Add support for the `Transfer Management API <https://developers.amadeus.com/self-service/category/cars-and-transfers/api-doc/transfer-management/api-reference>`_
+
+Big thanks to `Siddhartha Dutta <https://github.com/siddydutta>`_ for his contribution to the above implementations!
+
 8.0.0 - 2023-01-30
 --------------------
 Decommissioned Travel Restrictions API v1
 
 Decommissioned Hotel Search API v2
 
 Upgraded Python v3.8+ support and old dependencies
```

### Comparing `amadeus-8.0.0/LICENSE` & `amadeus-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/PKG-INFO` & `amadeus-8.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amadeus
-Version: 8.0.0
+Version: 8.1.0
 Summary: Python module for the Amadeus travel APIs
 Home-page: https://github.com/amadeus4dev/amadeus-python
 Author: Amadeus
 Author-email: developers@amadeus.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -365,14 +365,23 @@
 
     # Travel Restrictions v2
     amadeus.duty_of_care.diseases.covid19_report.get(countryCode='US')
 
     # Airline Routes
     amadeus.airline.destinations.get(airlineCode='BA')
 
+    # Transfer Search
+    amadeus.shopping.transfer_offers.post(body)
+
+    # Transfer Booking
+    amadeus.ordering.transfer_orders.post(body, offerId='1000000000')
+
+    # Transfer Management
+    amadeus.ordering.transfer_order('ABC').transfers.cancellation.post(body, confirmNbr=123)
+
 Development & Contributing
 --------------------------
 
 Want to contribute? Read our `Contributors
 Guide <.github/CONTRIBUTING.md>`__ for guidance on installing and
 running this code in a development environment.
```

### Comparing `amadeus-8.0.0/README.rst` & `amadeus-8.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -346,14 +346,23 @@
 
     # Travel Restrictions v2
     amadeus.duty_of_care.diseases.covid19_report.get(countryCode='US')
 
     # Airline Routes
     amadeus.airline.destinations.get(airlineCode='BA')
 
+    # Transfer Search
+    amadeus.shopping.transfer_offers.post(body)
+
+    # Transfer Booking
+    amadeus.ordering.transfer_orders.post(body, offerId='1000000000')
+
+    # Transfer Management
+    amadeus.ordering.transfer_order('ABC').transfers.cancellation.post(body, confirmNbr=123)
+
 Development & Contributing
 --------------------------
 
 Want to contribute? Read our `Contributors
 Guide <.github/CONTRIBUTING.md>`__ for guidance on installing and
 running this code in a development environment.
```

### Comparing `amadeus-8.0.0/amadeus/__init__.py` & `amadeus-8.1.0/amadeus/__init__.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/airline/_destinations.py` & `amadeus-8.1.0/amadeus/airline/_destinations.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/airport/_direct_destinations.py` & `amadeus-8.1.0/amadeus/airport/_direct_destinations.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/airport/predictions/_on_time.py` & `amadeus-8.1.0/amadeus/airport/predictions/_on_time.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/amadeus.py` & `amadeus-8.1.0/amadeus/amadeus.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/analytics/_itinerary_price_metrics.py` & `amadeus-8.1.0/amadeus/analytics/_itinerary_price_metrics.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/booking/_flight_order.py` & `amadeus-8.1.0/amadeus/booking/_flight_order.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/booking/_flight_orders.py` & `amadeus-8.1.0/amadeus/booking/_flight_orders.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/booking/_hotel_bookings.py` & `amadeus-8.1.0/amadeus/booking/_hotel_bookings.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/client/access_token.py` & `amadeus-8.1.0/amadeus/client/access_token.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/client/errors.py` & `amadeus-8.1.0/amadeus/client/errors.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/client/request.py` & `amadeus-8.1.0/amadeus/client/request.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/client/response.py` & `amadeus-8.1.0/amadeus/client/response.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/duty_of_care/diseases/_covid19_report.py` & `amadeus-8.1.0/amadeus/duty_of_care/diseases/_covid19_report.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/e_reputation/_hotel_sentiments.py` & `amadeus-8.1.0/amadeus/e_reputation/_hotel_sentiments.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/location/analytics/_category_rated_areas.py` & `amadeus-8.1.0/amadeus/location/analytics/_category_rated_areas.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/mixins/http.py` & `amadeus-8.1.0/amadeus/mixins/http.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/mixins/pagination.py` & `amadeus-8.1.0/amadeus/mixins/pagination.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/mixins/parser.py` & `amadeus-8.1.0/amadeus/mixins/parser.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/mixins/validator.py` & `amadeus-8.1.0/amadeus/mixins/validator.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/namespaces/_booking.py` & `amadeus-8.1.0/amadeus/namespaces/_booking.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/namespaces/_reference_data.py` & `amadeus-8.1.0/amadeus/namespaces/_reference_data.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/namespaces/_shopping.py` & `amadeus-8.1.0/amadeus/namespaces/_shopping.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 from amadeus.shopping._flight_offers_search import FlightOffersSearch
 from amadeus.shopping._seatmaps import Seatmaps
 from amadeus.shopping._activities import Activities
 from amadeus.shopping._activity import Activity
 from amadeus.shopping._availability import Availability
 from amadeus.shopping._hotel_offer_search import HotelOfferSearch
 from amadeus.shopping._hotel_offers_search import HotelOffersSearch
+from amadeus.shopping._transfer_offers import TransferOffers
 
 
 class Shopping(Decorator, object):
     def __init__(self, client):
         Decorator.__init__(self, client)
         self.flight_dates = FlightDates(client)
         self.flight_destinations = FlightDestinations(client)
         self.flight_offers = FlightOffers(client)
         self.flight_offers_search = FlightOffersSearch(client)
         self.seatmaps = Seatmaps(client)
         self.activities = Activities(client)
         self.availability = Availability(client)
         self.hotel_offers_search = HotelOffersSearch(client)
+        self.transfer_offers = TransferOffers(client)
 
     def hotel_offer_search(self, offer_id):
         return HotelOfferSearch(self.client, offer_id)
 
     def activity(self, activity_id):
         return Activity(self.client, activity_id)
```

### Comparing `amadeus-8.0.0/amadeus/namespaces/_travel.py` & `amadeus-8.1.0/amadeus/namespaces/_travel.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/namespaces/core.py` & `amadeus-8.1.0/amadeus/namespaces/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from amadeus.namespaces._booking import Booking
 from amadeus.namespaces._safety import Safety
 from amadeus.namespaces._schedule import Schedule
 from amadeus.namespaces._analytics import Analytics
 from amadeus.namespaces._location import Location
 from amadeus.namespaces._duty_of_care import DutyOfCare
 from amadeus.namespaces._airline import Airline
+from amadeus.namespaces._ordering import Ordering
 
 
 class Core(object):
     def __init__(self):
         self.reference_data = ReferenceData(self)
         self.travel = Travel(self)
         self.shopping = Shopping(self)
@@ -22,7 +23,8 @@
         self.booking = Booking(self)
         self.safety = Safety(self)
         self.schedule = Schedule(self)
         self.analytics = Analytics(self)
         self.location = Location(self)
         self.duty_of_care = DutyOfCare(self)
         self.airline = Airline(self)
+        self.ordering = Ordering(self)
```

### Comparing `amadeus-8.0.0/amadeus/reference_data/_airlines.py` & `amadeus-8.1.0/amadeus/reference_data/_airlines.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/_location.py` & `amadeus-8.1.0/amadeus/reference_data/_location.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/_locations.py` & `amadeus-8.1.0/amadeus/reference_data/_locations.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/_recommended_locations.py` & `amadeus-8.1.0/amadeus/reference_data/_recommended_locations.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/_airports.py` & `amadeus-8.1.0/amadeus/reference_data/locations/_airports.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/_cities.py` & `amadeus-8.1.0/amadeus/reference_data/locations/_cities.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/_hotel.py` & `amadeus-8.1.0/amadeus/reference_data/locations/_hotel.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/_point_of_interest.py` & `amadeus-8.1.0/amadeus/reference_data/locations/_point_of_interest.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/_points_of_interest.py` & `amadeus-8.1.0/amadeus/reference_data/locations/_points_of_interest.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/hotels/_by_city.py` & `amadeus-8.1.0/amadeus/reference_data/locations/hotels/_by_city.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/hotels/_by_geocode.py` & `amadeus-8.1.0/amadeus/reference_data/locations/hotels/_by_geocode.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/hotels/_by_hotels.py` & `amadeus-8.1.0/amadeus/reference_data/locations/hotels/_by_hotels.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/locations/points_of_interest/_by_square.py` & `amadeus-8.1.0/amadeus/reference_data/locations/points_of_interest/_by_square.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/reference_data/urls/_checkin_links.py` & `amadeus-8.1.0/amadeus/reference_data/urls/_checkin_links.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/safety/_safety_rated_location.py` & `amadeus-8.1.0/amadeus/safety/_safety_rated_location.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/safety/_safety_rated_locations.py` & `amadeus-8.1.0/amadeus/safety/_safety_rated_locations.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/safety/safety_rated_locations/_by_square.py` & `amadeus-8.1.0/amadeus/safety/safety_rated_locations/_by_square.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/schedule/_flights.py` & `amadeus-8.1.0/amadeus/schedule/_flights.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_activities.py` & `amadeus-8.1.0/amadeus/shopping/_activities.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_activity.py` & `amadeus-8.1.0/amadeus/shopping/_activity.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_flight_dates.py` & `amadeus-8.1.0/amadeus/shopping/_flight_dates.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_flight_destinations.py` & `amadeus-8.1.0/amadeus/shopping/_flight_destinations.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_flight_offers.py` & `amadeus-8.1.0/amadeus/shopping/_flight_offers.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_flight_offers_search.py` & `amadeus-8.1.0/amadeus/shopping/_flight_offers_search.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_hotel_offer_search.py` & `amadeus-8.1.0/amadeus/shopping/_hotel_offer_search.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_hotel_offers_search.py` & `amadeus-8.1.0/amadeus/shopping/_hotel_offers_search.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/_seatmaps.py` & `amadeus-8.1.0/amadeus/shopping/_seatmaps.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/activities/_by_square.py` & `amadeus-8.1.0/amadeus/shopping/activities/_by_square.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/availability/_flight_availabilities.py` & `amadeus-8.1.0/amadeus/shopping/availability/_flight_availabilities.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/flight_offers/_prediction.py` & `amadeus-8.1.0/amadeus/shopping/flight_offers/_prediction.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/flight_offers/_pricing.py` & `amadeus-8.1.0/amadeus/shopping/flight_offers/_pricing.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/shopping/flight_offers/_upselling.py` & `amadeus-8.1.0/amadeus/shopping/flight_offers/_upselling.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/travel/_trip_parser.py` & `amadeus-8.1.0/amadeus/travel/_trip_parser.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/travel/analytics/air_traffic/_booked.py` & `amadeus-8.1.0/amadeus/travel/analytics/air_traffic/_booked.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/travel/analytics/air_traffic/_busiest_period.py` & `amadeus-8.1.0/amadeus/travel/analytics/air_traffic/_busiest_period.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/travel/analytics/air_traffic/_traveled.py` & `amadeus-8.1.0/amadeus/travel/analytics/air_traffic/_traveled.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/travel/predictions/_flight_delay.py` & `amadeus-8.1.0/amadeus/travel/predictions/_flight_delay.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus/travel/predictions/_trip_purpose.py` & `amadeus-8.1.0/amadeus/travel/predictions/_trip_purpose.py`

 * *Files identical despite different names*

### Comparing `amadeus-8.0.0/amadeus.egg-info/PKG-INFO` & `amadeus-8.1.0/amadeus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amadeus
-Version: 8.0.0
+Version: 8.1.0
 Summary: Python module for the Amadeus travel APIs
 Home-page: https://github.com/amadeus4dev/amadeus-python
 Author: Amadeus
 Author-email: developers@amadeus.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -365,14 +365,23 @@
 
     # Travel Restrictions v2
     amadeus.duty_of_care.diseases.covid19_report.get(countryCode='US')
 
     # Airline Routes
     amadeus.airline.destinations.get(airlineCode='BA')
 
+    # Transfer Search
+    amadeus.shopping.transfer_offers.post(body)
+
+    # Transfer Booking
+    amadeus.ordering.transfer_orders.post(body, offerId='1000000000')
+
+    # Transfer Management
+    amadeus.ordering.transfer_order('ABC').transfers.cancellation.post(body, confirmNbr=123)
+
 Development & Contributing
 --------------------------
 
 Want to contribute? Read our `Contributors
 Guide <.github/CONTRIBUTING.md>`__ for guidance on installing and
 running this code in a development environment.
```

### Comparing `amadeus-8.0.0/amadeus.egg-info/SOURCES.txt` & `amadeus-8.1.0/amadeus.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -53,20 +53,28 @@
 amadeus/namespaces/_airline.py
 amadeus/namespaces/_airport.py
 amadeus/namespaces/_analytics.py
 amadeus/namespaces/_booking.py
 amadeus/namespaces/_duty_of_care.py
 amadeus/namespaces/_e_reputation.py
 amadeus/namespaces/_location.py
+amadeus/namespaces/_ordering.py
 amadeus/namespaces/_reference_data.py
 amadeus/namespaces/_safety.py
 amadeus/namespaces/_schedule.py
 amadeus/namespaces/_shopping.py
 amadeus/namespaces/_travel.py
 amadeus/namespaces/core.py
+amadeus/ordering/__init__.py
+amadeus/ordering/_transfer_order.py
+amadeus/ordering/_transfer_orders.py
+amadeus/ordering/transfer_orders/__init__.py
+amadeus/ordering/transfer_orders/_transfers.py
+amadeus/ordering/transfer_orders/transfers/__init__.py
+amadeus/ordering/transfer_orders/transfers/_cancellation.py
 amadeus/reference_data/__init__.py
 amadeus/reference_data/_airlines.py
 amadeus/reference_data/_location.py
 amadeus/reference_data/_locations.py
 amadeus/reference_data/_recommended_locations.py
 amadeus/reference_data/_urls.py
 amadeus/reference_data/locations/__init__.py
@@ -98,14 +106,15 @@
 amadeus/shopping/_flight_dates.py
 amadeus/shopping/_flight_destinations.py
 amadeus/shopping/_flight_offers.py
 amadeus/shopping/_flight_offers_search.py
 amadeus/shopping/_hotel_offer_search.py
 amadeus/shopping/_hotel_offers_search.py
 amadeus/shopping/_seatmaps.py
+amadeus/shopping/_transfer_offers.py
 amadeus/shopping/activities/__init__.py
 amadeus/shopping/activities/_by_square.py
 amadeus/shopping/availability/__init__.py
 amadeus/shopping/availability/_flight_availabilities.py
 amadeus/shopping/flight_offers/__init__.py
 amadeus/shopping/flight_offers/_prediction.py
 amadeus/shopping/flight_offers/_pricing.py
```

### Comparing `amadeus-8.0.0/setup.py` & `amadeus-8.1.0/setup.py`

 * *Files identical despite different names*

