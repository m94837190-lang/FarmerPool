# FarmerPool

**Tagline:** Grow together. Sell smarter.

FarmerPool is a mobile-friendly hackathon prototype for a farmer-to-buyer crop-listing marketplace. Farmers can add produce details and buyers can browse listings by crop or village.

## Problem statement
Small and marginal farmers may struggle to reach multiple buyers, compare prices, and coordinate transportation. Buyers may have to contact many individual farmers to source a desired quantity. These issues can contribute to information gaps, high transaction effort, and avoidable logistics costs.

## Proposed solution
FarmerPool provides one shared marketplace for crop listings. A farmer can list crop type, available quantity, expected price per quintal, location, and availability. Buyers can browse and search listings. A future version can add verified buyer requests, pooled orders, reliable price feeds, and transport coordination.

## Run the prototype
1. Download or clone this repository.
2. Open `index.html` in a modern browser. No build step or dependencies are required.
3. On GitHub, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save. Wait for the published URL to appear.
4. Test the published page on a phone.

## Implemented in this prototype
- Responsive layout for phone and desktop
- Sample crop listings (illustrative data)
- Search by crop, farmer, or village
- Crop filter
- Form validation for new listings
- Local browser storage for listings created on the same device
- Clear demo message for non-functional production services

## Not implemented (be honest in the submission)
- No backend or shared database; listings added by one user do not appear for other users
- No real user authentication, buyer/seller verification, bidding, confirmed orders, payments, transport booking, live mandi prices, or SMS delivery
- “I'm interested” is a demo interaction only
- Sample prices are not live market rates and must not be used for trading

## Suggested next development steps
1. Choose a backend (for example, Firebase or Supabase) and define farmer, listing, buyer inquiry, and order data models.
2. Add authentication and role-based access controls.
3. Store listings on a server with input validation and ownership checks.
4. Connect verified mandi price data only through a permitted, documented data source; show the source and timestamp.
5. Add buyer inquiry and order confirmation with cancellation policies and dispute handling.
6. Add transport partners with availability confirmation, transparent quotes, backup options, and no promise of service until confirmed.
7. Add Telugu and other regional languages, accessible forms, low-bandwidth design, and optional SMS alerts through a compliant provider.
8. Test with farmers and buyers, document feedback, and improve security and reliability.

## Repository structure
```text
FarmerPool/
├── index.html
├── README.md
├── docs/
│   └── research-and-submission.md
└── .gitignore
```

## Team contributions
Update this section with real team members and the work they actually completed. Make separate commits for meaningful contributions; do not fabricate contribution history.

## License
For a hackathon demo, choose a license your team agrees to use. No license is included by default.
