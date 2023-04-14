Front End :computer:
V1 :rocket:
Set up the front-end using Vite and Tailwind CSS :sparkles:
Display a grid of startups (name, description, domain, added date) with their respective website traffic data (past 3 months) displayed in a chart. Charts are done using the Recharts library :bar_chart:
Sort startups by growth rate (e.g. greater than 50%) within the last x months (another input field) :chart_with_upwards_trend:
/me page with basic account creation and auth :bust_in_silhouette:
V2 :rocket:
Add more company filtering/sorting (e.g. by keywords and absolute traffic amount) :mag_right:
Limit the results for "free" users :lock:
Allow users to subscribe to a Pro plan that unlocks all companies via their /me page, and a /pro page :money_with_wings:
V3 :rocket:
Polishing UI, mobile responsiveness, transactional emails, etc. :nail_care:
Create a /details page for each company with more information (e.g. similar companies, full description, etc.) :page_facing_up:
Allow users to save companies to their "Tracklist" :bookmark:
Back End :gear:
V1 :rocket:
Admin page, that lets me add new domains manually :hammer_and_wrench:
Once added, company information (name, description, and traffic information for the past 3 months) will be fetched via the SimilarWeb API :calling:
Store the companies with respective information in MongoDB :floppy_disk:
Create an aggregation script, that allows the filtering and sorting (by traffic) in the frontend :mag_right:
Create an "update all" function, that automatically updates all companies on a monthly basis with new website traffic information via the SimilarWeb API (using bottleneck etc. for rate limiting on the API) :repeat:
V2 :rocket:
Create scraping scripts, that automatically scrape identified sources (e.g. ProductHunt, etc.) on a daily basis for newly launched companies :newspaper:
Automatically funnel scraped companies through SimilarWeb API to retrieve traffic information :calling:
User Auth, Protected Routes via Access & Refresh Token (via Cookies) :busts_in_silhouette:
Set up transactional Emails (via SendGrid) for Password reset, etc. :email:
Hook up payment workflows via the Stripe API and allow users to create and manage a "Pro Subscription" :credit_card:
V3 :rocket:
Identify and hook up more APIs that allow me to retrieve more useful information about each company (e.g. similar companies, etc.) :mag:
Build save to tracklist functionality :bookmark:
