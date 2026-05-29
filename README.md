Pre-FC & Surplus Funds Map
A field-ready door knocking tool built for surplus funds recovery operators, foreclosure investors, and real estate professionals working distressed property markets.

What This Is
This app turns raw foreclosure and surplus funds data into an interactive map you can use in the field. Upload your CSV lists, see color-coded pins across Miami-Dade and Broward County, build an optimized door knocking route from wherever you are, and track every interaction — all from your phone or laptop.
Built for solo operators and small teams working surplus funds recovery, pre-foreclosure outreach, and auction-adjacent door knocking. Designed to maximize doors knocked per hour of drive time.

Core Features
Interactive Map

Color-coded pins by category: gold for high-value surplus anchors, green for surplus funds, yellow for upcoming auctions, red for foreclosures and lis pendens
Tier 1 anchor pins ($100K+ surplus) are larger and gold — they stand out immediately
Dark map theme optimized for outdoor readability on a phone screen
Draw a circle or rectangle on the map to isolate a target zone

Smart Data Upload

Upload three separate CSV files: surplus funds, upcoming auctions, foreclosures/lis pendens
Automatic duplicate detection by case number — merged into single pins when a property appears across multiple lists
Expired auction filter — flags past sale dates on upload and lets you hide them in one tap
Surplus lead age indicator — color-coded badge showing how many days since auction (fresh/mid/stale)

Dual Address Intelligence

For surplus properties, the app distinguishes between the property address (where the foreclosure is) and the mailing address (where the owner actually lives)
Out-of-state owners are automatically flagged — phone and email outreach recommended over a door knock
Two separate navigation buttons in each popup: Navigate to Owner and Navigate to Property
Geocode validation using ZIP code centroids to prevent pins from landing in the wrong city

Advanced Filters

Surplus amount range (min/max) — focus only on six-figure claims
Date range filter for auctions — preset buttons for next 7, 14, 21, 30 days
Street name, city, ZIP code, and county filters
Surplus lead age cutoff — hide anything older than X days
Adjustable Tier 1 anchor threshold — default $100K, change anytime

Location-Based Route Optimization

Tap Optimize from Location — the app reads your GPS and sorts all stops using a nearest-neighbor algorithm starting from where you physically are
Tier 1 anchor stops are prioritized first, with fill-in stops (smaller surplus, auctions, FC) inserted near the anchors they're closest to
Works whether you're leaving home or already in the field mid-shift
Fallback to zip-code area sort when GPS is unavailable

Google Maps 10-Stop Limit Workaround

Routes with more than 10 stops are automatically split into chunks of 10
Each chunk opens in Google Maps as a complete optimized route with turn-by-turn navigation
Chunk buttons show which ones contain Tier 1 anchors
Work through chunks sequentially — finish one, tap the next

Zone Outlier Detection

After drawing a zone, the app detects properties whose ZIP code doesn't match the majority of selected pins
Outliers are flagged in orange and can be removed from the route in one tap before opening Maps

Field Canvassing Tracker

Five door knock statuses per property: Answered, Not Home, Not Interested, Call Back, Signed
Tap a status and the map pin immediately changes color to reflect the outcome
Notes field per property — owner said call back at 6pm, gate locked, left package in mailbox, whatever
All field data saves automatically and persists between sessions

Full Contact Information

Up to 5 phone numbers per owner with type (Mobile, Residential) and DNC flags
Up to 5 email addresses
Up to 5 relatives with their own phones and emails — accessible when the owner doesn't answer
Tap-to-call and tap-to-email on mobile

KPI Dashboard

Doors knocked, contact rate, signed count, total surplus pool value
Outcome breakdown by status
Top zip codes by canvassing activity
Export canvass results as CSV for CRM import or record keeping

Persistent Storage

API key, CSV data, geocode cache, field notes, and filter settings all save to browser local storage
Upload once on your laptop — data is there when you reopen the file
Each device (laptop, iPhone, Android) maintains its own saved state
Clear data anytime from the Data tab — field notes are preserved separately


Data Sources
The app accepts CSV uploads from any of these sources:
CategorySourceSurplus FundsCounty Clerk of Court (Miami-Dade, Broward)Upcoming AuctionsRealForeclosure.comForeclosures / Lis PendensATTOM Data, PropertyRadar, or manual clerk exportSkip TracingBatchSkipTracing, BeenVerified, or similar

CSV Column Requirements
Surplus Funds
Surplus Amount, Closing Bid, Opening Bid, Date Sold, Case Number, Parcel Number, Type of foreclosure, First Name, Last Name, Mailing Street, Mailing City, Mailing State, Mailing ZIP Code, Property Street, Property City, Property State, Property ZIP Code, County, Source, Age, Deceased, Phone 1–5 (with Type and DNC columns), Email 1–5, Relative 1–5 (with phones and emails)
Upcoming Auctions
Sale Date, Case Number, Address, City, Zip, County, Final Judgment, Assessed Value, Status, Plaintiff Max Bid, Type of foreclosure
Foreclosures / Lis Pendens
Address, City, Zip, County, Owner Name, Default Amount, Case Number — flexible column name matching

Setup

Get a free Google Maps API key at console.cloud.google.com
Enable Maps JavaScript API and Geocoding API
Open the app, paste your API key, and click Load Map
Your key is saved — you only enter it once per device
Upload your CSV files from the Data tab

To use on mobile: host this file on GitHub Pages or Netlify, open the URL in Safari or Chrome, and add it to your home screen.

Operational Strategy
This tool is designed around a tiered door knocking approach:
Tier 1 anchors (gold pins) are your primary targets — six-figure surplus claims where your commission is largest. These anchor your route.
Fill-in stops (green, yellow, red pins) are smaller surplus claims, upcoming auctions, and active foreclosures that happen to be near your anchor stops. Hit these in between to maximize every trip.
Out-of-state owners are your best remote closes — they cannot physically claim the funds themselves and are often unaware of the surplus. Phone and email outreach first.
Absentee/mailing address — the app navigates you to where the owner lives, not just where the foreclosure is. A different knock address means a real person at a different location, not a vacant house.

Built By
Surplus Prosperity / IDEA Prosperity Group
South Florida Surplus Funds Recovery Operation
Miami-Dade & Broward County

This tool is for internal operational use. Data sourced from public county records.
