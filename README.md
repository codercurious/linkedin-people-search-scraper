# Linkedin people search scraper
Interested in using this scraper? Get it here: [Linkedin people search scraper](https://apify.com/curious_coder/linkedin-people-search-scraper?fpr=ve081&fp_sid=github_linkedin-people-search-scraper)
## How it works

This actor works on a logged in linkedin account, but doesn't require login details or 2FA as it does't login but uses already generated linkedin session information.

You need to pass linkedin cookies to this actor to use the existing session to access search results page and perform scraping.

You can customise and randomise the delay between scraping pages.

## Getting Started

Install [EditThisCookie](https://chrome.google.com/webstore/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg) chrome extension 

Login to your linkedin account

Click on the extension and export the linkedin cookies

Paste the cookies into this actor's `Linkedin cookie` input field

Go to [linkedin people search page](https://www.linkedin.com/search/results/people), search with required filters and once you are done, copy the full URL from address bar and pass it to this actor

Copy the link from address bar and paste it to actor `Search URL` input field

Enter start page and end page based on your requirements. You can access up to max 1000 results per search. 

Here is the sample output of this actor:

```
{
	"fullName": "Javeed Ashraf",
	"firstName": "Javeed",
	"lastName": "Ashraf",
	"id": "143153644",
	"location": "Bengaluru",
	"headline": "Software Engineer III at GitHub | Ex-Walmart",
	"profileId": "ACoAAAiIWewBj6_Brf4O_tuu22yge09fi23wBVg",
	"distance": "1st",
	"publicId": "javeedashraf1",
	"profileUrl": "https://www.linkedin.com/in/javeedashraf1"
}
```

## Use cases
### 1. Scrape linkedin company employees
Scrape list of employees of a linkedin company. Go to linkedin people search page and click on 'Company' filter and select the company.

### 2. Scrape linkedin event attendees
Scrape list of event attendees of a linkedin event. Go to desired linkedin event page and click on 'Attend' button and register yourself. Then you can see a link to see event attendees right above the button.
### 2. Scrape linkedin followers
Scrape list of people who are following a linkedin user. On linkedin search page, Select result type to 'People' and then click on 'All filters', then under 'Followers of user' filter, search for and select the linkedin user to find their followers
