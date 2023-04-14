# Launchtracker.co

A tool to discover and track high growing startups before they take off. 

## Front End

### V1

- Set up the frontend using Vite and Tailwind CSS
- Display a grid of startups (name, description, domain, added date) with their respective website traffic data (past 3 months) displayed in a chart. Charts are done using the Recharts library
- Sort startups by growth rate (e.g. greater than 50%) within the last x months (another input field)
- /me page with basic account creation and auth

### V2

- Add more company filtering/sorting (e.g. by keywords and absolute traffic amount)
- Limit the results for “free” users
- Allow users to subscribe to a Pro plan that unlocks all companies via their /me page, and a /pro page

### V3

- Polish UI, mobile responsiveness, transactional emails etc.
- Create a /details page for each company with more information (e.g. similar companies, full description, etc.)
- Allow users to save companies to their “Tracklist”

## Back End

### V1

- Admin page, that lets me add new domains manually
- Once added, company information (name, description, and traffic information for the past 3 months) will be fetched via the the SimilarWeb API
- Store the companies with respective information in MongoDB
- Create an aggregation script, that allows the filtering and sorting (by traffic) in the frontend
- Create an “update all” function, that automatically updates all companies on a monthly basis with new website traffic information via the SimilarWeb API (using bottleneck etc. for rate limiting on the API)

### V2

- Create scraping scripts, that automatically scrape target sources on a daily basis for newly launched companies
- Automatically funnel scraped companies through SimilarWeb API to retrieve traffic information
- User Auth, Protected Routes via Access & Refresh Token (via Cookies)
- Set up transactional Emails (via SendGrid) for Password reset etc.
- Hook up payment workflows via the Stripe API and allow users to create and manage a “Pro Subscription”

### V3

- Identify and hook up more APIs that allow me to retrieve more useful information about each company (e.g. similar companies etc.)
- Build save to tracklist functionality
