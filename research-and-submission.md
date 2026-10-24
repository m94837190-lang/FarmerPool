# FarmerPool — Research and Hackathon Submission

## 1. Project overview
**Project:** FarmerPool  
**Category:** Software / Agriculture / Digital marketplace  
**Stage:** Front-end demonstration prototype  
**Core idea:** Help farmers present available produce to a wider set of potential buyers and help buyers discover supply by crop and location.

## 2. Problem statement
Farmers can face difficulty finding buyers beyond their existing local network, comparing offers, and arranging transport for small or fragmented quantities. Buyers may need to contact multiple farmers to assemble a larger order. A digital listing and discovery tool may reduce search effort, but it cannot by itself guarantee a fair price, a buyer, or transport.

## 3. Target users
- Farmers and farmer producer organisations (FPOs) listing produce
- Wholesalers, retailers, processors, and other crop buyers
- Potential future transport partners and marketplace administrators

## 4. Proposed solution
FarmerPool offers a shared digital interface to publish crop listings with quantity, expected price, village/town, and availability. Buyers can browse, filter, and search listings. Future releases could support verified inquiries, group purchasing, order commitments, and transport coordination.

## 5. Main workflow
1. Farmer opens the app and enters listing details.
2. The app validates required fields.
3. The listing appears in the browser's marketplace.
4. A buyer searches by crop or location and compares available listings.
5. In a production system, the buyer would send an inquiry and the farmer would explicitly accept or reject it.
6. Only after quantity, price, pickup/delivery terms, and payment/cancellation rules are confirmed should an order be treated as committed.
7. Transport should be assigned only after a provider confirms availability, price, pickup point, and delivery plan.

**Current prototype boundary:** Steps 1–4 are demonstrated locally. Buyer contact and real orders are not implemented.

## 6. Features implemented
- Mobile-responsive HTML/CSS interface
- Sample marketplace cards
- Search by crop, village, or farmer
- Crop-category filter
- Form for new crop listing
- Browser local storage for locally created listings
- Input validation and demo notices

## 7. Technical design
- **Frontend:** HTML5, CSS3, vanilla JavaScript
- **Storage:** Browser localStorage for demonstration only
- **Dependencies:** None
- **Deployment option:** GitHub Pages for static hosting
- **Production architecture (planned):** Frontend + authenticated API/backend + database + optional messaging and transport integrations

## 8. Data and accuracy
The sample listings and prices included in the prototype are fictional/illustrative demonstration data. They are not current mandi prices. A production implementation must use a lawful, reliable source for market rates, retain the source and update time, and avoid claiming coverage of every mandi unless that coverage has been verified.

## 9. Risks and mitigations
- **Buyer cancels after commitment:** Use explicit order acceptance, written terms, cancellation deadlines, and a documented dispute process.
- **Farmer cannot supply the crop:** Require availability reconfirmation before order acceptance and allow prompt cancellation/refund processes where applicable.
- **No transport available:** Do not promise delivery until a carrier confirms; offer pickup, alternate providers, rescheduling, or cancellation terms.
- **Poor roads or remote villages:** Capture pickup location and vehicle/access constraints early; do not assume every vehicle can reach every farm.
- **Incorrect listings or fraud:** Add verified profiles, report/block tools, moderation, audit records, and safe contact practices.
- **Privacy/security:** Do not publish phone numbers by default; use authentication, authorization, data minimization, secure communication, and retention policies.
- **Low connectivity/language barriers:** Keep pages lightweight and add regional-language and low-bandwidth support; offline/SMS features are future work, not implemented in this prototype.

## 10. Testing checklist
- Open the app on Android Chrome and desktop browser.
- Navigate through Home, Marketplace, List a crop, and About.
- Search for a sample crop and a village.
- Filter by crop.
- Submit a valid listing and confirm it appears on the same browser/device.
- Try blank required fields and invalid numeric values.
- Refresh the page and confirm local listing persists.
- Clear browser site data and note that local demo listings can be removed.
- Check that sample prices are labelled as illustrative and no real order/payment claim is made.

## 11. Future roadmap
**Phase 1:** Backend database, authentication, user roles, and shared listings.  
**Phase 2:** Buyer inquiries, confirmed orders, cancellation terms, and audit trail.  
**Phase 3:** Verified market-price source and timestamps, plus price comparison.  
**Phase 4:** Transport partner directory, availability confirmation, quote comparison, and contingency handling.  
**Phase 5:** Regional languages, accessibility, low-bandwidth improvements, and optional SMS notifications.

## 12. Hackathon demonstration script
1. Explain the problem in 20–30 seconds.
2. Open the Home page and describe the farmer-first concept.
3. Search for rice or a sample village in Marketplace.
4. Open List a crop and add a demonstration listing with non-sensitive sample information.
5. Show that the listing appears in the marketplace on that device.
6. Clearly explain that this is a front-end prototype: listings are local, prices are sample data, and authentication, live prices, actual buyer contact, orders, payment, and transport booking are future work.
7. Describe the next technical milestone and how the team will validate the idea with real users.

## 13. Submission honesty
Only claim features that work in the submitted code. Add the actual team name/member contributions, screenshots, test evidence, and commits from work genuinely completed. Do not include passwords, API keys, private phone numbers, or other secrets in the repository.
