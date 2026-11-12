# Instahyre Jobs Scraper & API - Last 24 Hours, India Tech Jobs

Instahyre jobs scraper and API: search India tech jobs on instahyre.com by skill, city and experience, newest first, and get each job's title, company, city, experience range in years, skills, job category, posting date and link, with the company's headcount band, founding year and tagline on every row. Turn on full details for the description and the company's industry, website, LinkedIn, tech stack, benefits and Glassdoor ratings.

Use it as an Instahyre API with no login and no API key, an Instahyre job scraper for a daily India job feed, or a hiring tracker for Bengaluru, Mumbai, Delhi NCR, Hyderabad, Pune, Chennai and remote (Work From Home) jobs, from the Apify Console, the Apify API, Python, JavaScript, n8n, Make or an AI agent, with JSON, CSV or Excel export. Available as an [Apify Actor](https://apify.com/anshumanatrey/instahyre-jobs-search). $0.00019 per job, $0.00023 with full details, $0.013 per run start, no login.

**Use it from an AI assistant:**

- **Claude** (claude.ai and the desktop app): [Add Instahyre Jobs to Claude](https://claude.ai/customize/connectors?modal=add-custom-connector&connectorName=Instahyre%20Jobs&connectorUrl=https%3A%2F%2Fmcp.apify.com%3Ftools%3Danshumanatrey%2Finstahyre-jobs-search), click Continue, sign in to Apify, Allow, and ask in plain words.
- **Claude Code:** `claude mcp add --transport http instahyre-jobs-search "https://mcp.apify.com?tools=anshumanatrey/instahyre-jobs-search"`, then run `/mcp` to sign in to Apify.
- **Codex:** `codex mcp add instahyre-jobs-search --url "https://mcp.apify.com?tools=anshumanatrey/instahyre-jobs-search"`, then `codex mcp login instahyre-jobs-search`.
- **Any other MCP client:** `https://mcp.apify.com?tools=anshumanatrey/instahyre-jobs-search`, signed in with Apify or an `Authorization: Bearer <APIFY_TOKEN>` header.

## What does it do?

- **Searches every open job on Instahyre.** On 2026-11-08 Instahyre listed 13,453 open jobs at 3,175 companies, at employers such as Accenture, Amazon, Flipkart, Myntra, Oracle, Deutsche Telekom Digital Labs, Disney, PwC and hundreds of startups.
- **The posting date Instahyre does not show.** Instahyre's search shows no date and keeps jobs listed for months; every row here has the day the job was posted, read from the job's own page, and the rows come newest first.
- **Experience on every row.** The years of experience each job asks for (`experienceMin` to `experienceMax`), and a filter that keeps the jobs open to your years: 3, a range such as 2-5, 5+ or fresher.
- **Skills match too.** A search word matches the job title or one of the skills Instahyre tags the job with: python is in 177 job titles but in 3,264 jobs' titles or skill tags (2026-11-08).
- **Indian places as people type them.** Bengaluru finds Bangalore, Gurugram finds Gurgaon, Delhi NCR, a state (Karnataka, Maharashtra) finds its cities, and Remote or Work from home typed alone finds Instahyre's remote jobs.
- **Company facts on every row.** Headcount band, founding year and tagline from Instahyre's company profile, and with full details the industry, website, LinkedIn, tech stack, benefits and Glassdoor ratings.
- **Checks job links.** Paste Instahyre job links and each comes back open, closed or not found.

## How is it different from other Instahyre scrapers?

- **Newest first, for real.** Instahyre orders its search by its own score and keeps jobs listed for months. On 2026-11-08 the first page of instahyre.com for python developer jobs in Bangalore was a median 117 days old (its oldest 626 days), and for jobs open to freshers a median 20 days (its oldest 1,322 days); the first 20 rows of this actor for the same searches were a median 34 days and 1 day old. Instahyre gives job numbers in the order jobs are posted (on 420 job pages from 2018 to today, the date never went back as the number grew), so the newest jobs are read first and dated from their pages.
- **A posting date on every row, and a posted-within filter.** Of the 9 Instahyre actors with 5 or more users (table below), s_actors gives the posting date on every job, and memo23 and parsebird with their paid details.
- **Experience range, skills, category and company headcount on the plain row,** with no extra charge. getascraper, memo23 and parsebird add the experience range only with their paid detail option; s_actors includes it in its price.
- **Matches words the way buyers mean them.** Instahyre's own search for python developer lists 6,439 jobs, and only 100 of them have both words in their title or in one skill tag (2026-11-08); this actor keeps the jobs that have every word of your search in their title or a skill tag, and reads Instahyre's ranking only as far as it keeps matching.
- **Internship stipends.** The one pay figure Instahyre shows: an internship's monthly stipend in rupees, its length in months and its start date.
- **You pay for what you get.** One charge per delivered row plus a $0.013 run start, and a spending limit stops the run cleanly with the jobs it paid for.

## When should I use it?

- **Job seekers and job boards:** new India tech jobs by skill, city, experience and date, on a daily schedule.
- **Recruiters and staffing teams:** who is hiring for a skill right now, which jobs come through an agency (`agencyName`), and how many years each role asks for.
- **Sales and market research:** companies hiring by city, size and founding year as a buying signal, with industry, website and LinkedIn when details are on.
- **Data teams and AI agents:** one clean, stable Instahyre feed through the API or MCP.

## How much does it cost to scrape Instahyre jobs?

Pay per event: $0.19 per 1,000 jobs, or $0.23 per 1,000 with full details, plus $0.013 per run start at the default 512 MB of memory. Apify's free $5 monthly credit covers about 15,600 jobs in runs of 100. Platform usage is included, and there is no monthly fee.

| Event | Price | When it is charged |
|---|---|---|
| Job | $0.00019 | One saved job, and one checked link that is closed or not found |
| Job with details | $0.00023 | One saved job with full details on |
| Run start | $0.013 per GB of memory | Charged by Apify when a run starts: once up to 1 GB, so $0.013 at the default 512 MB. It covers what a run costs before its first job |

Instahyre Jobs Scraper's Apify Store header, "from $0.11 / 1,000 jobs", shows the lowest discount-tier price: the GOLD price. FREE users (Apify's Free plan) pay the base price in the table, $0.00019 a job and $0.00023 with details; BRONZE (Starter) pays $0.00018 and $0.00022; SILVER (Scale) $0.00014 and $0.00017; GOLD (Business), PLATINUM and DIAMOND $0.00011 and $0.00013. The run start is a flat fee on every plan and the header never shows it.

| Run (Free plan price, default memory) | Cost |
|---|---|
| 100 newest jobs | $0.032 |
| 100 jobs with full details | $0.036 |
| 1,000 jobs | $0.203 |
| Every job on Instahyre, 13,453 on 2026-11-08 | $2.569 |

Number of jobs (`maxJobs`) and the run start set the most a run can cost, and a run stops at its spending limit with a message saying so.

## How does the price compare with other Instahyre scrapers?

Every actor on the Apify Store with Instahyre in its title and 5 or more users in the last 30 days, on 2026-11-08, ordered by users. Free-plan prices from each actor's current pricing.

| Actor | Users, 30 days | Per job | Start fee | Posting date |
|---|---|---|---|---|
| getascraper/instahyre-jobs-scraper | 326 | $0.00105, $0.00115 with its details | $0.00005 | No |
| getascraper/india-job-inventory-feed | 215 | $0.00199 | $0.00005 | Not for Instahyre jobs |
| memo23/instahyre-jobs-scraper | 81 | $0.0015, $0.003 with its details | $0.0001 | With details |
| seemuapps/india-tech-jobs-scraper | 25 | $0.004 | none | Not stated for Instahyre |
| themineworks/instahyre-jobs-scraper | 6 | $0.002 | $0.005 | No |
| parsebird/instahyre-jobs-scraper | 6 | $0.00099, $0.00169 with its details | $0.001 | With details |
| s_actors/instahyre-jobs-scraper | 6 | $0.000768 | $0.001 | Yes |
| rt-solutions/india-tech-jobs-scraper | 6 | $0.0015 | none | Not for Instahyre jobs |
| neverempty/instahyre-jobs | 5 | $0.002 | none | No |
| This actor | new | $0.00019, $0.00023 with details | $0.013 per GB, $0.013 at 512 MB | Yes, every row |

Where others are cheaper: this actor's run start, $0.013, is the highest of these actors (getascraper $0.00005, memo23 $0.0001, s_actors and parsebird $0.001, themineworks $0.005), so a run of fewer than 21 jobs costs less on s_actors/instahyre-jobs-scraper, which includes its details, posting dates and Glassdoor ratings at $0.000768 a job; from 21 jobs a run on, this actor costs less than any of them. Where others do more: getascraper and memo23 add an employer email lookup and a change-tracking mode that returns only new or changed jobs; here, schedule a run with Posted in the last set to 24 hours instead.

## Which inputs does it take?

Nothing is required. Type a skill or a job title and press Start, or press Start with the form empty for the newest jobs of every kind.

| Field | What it does |
|---|---|
| Skills or titles (`searchTerms`) | One per line. A job matches when its title, or one of its skill tags, has every word: react also finds React Native. A pasted Instahyre search link works too |
| City or state (`location`) | Bangalore, Mumbai, Delhi NCR, Karnataka, Bengaluru, Gurugram. India finds every job in India. Remote or Work from home typed alone asks for remote jobs; next to a city it changes nothing |
| Experience (`experienceYears`) | Your years: 3, a range such as 2-5, 5+ for five or more, or fresher. Keeps the jobs whose range overlaps yours |
| Remote or office (`workType`) | remote for Instahyre's Work From Home jobs, onsite for jobs in a city |
| Posted in the last (`postedWithin`) | 24 hours, 3 days, 7 days, 30 days (the default), any time, or your own period such as 2 weeks |
| Number of jobs (`maxJobs`) | How many, newest first: 100 by default, 0 for every match |
| Full details (`includeDetails`) | Adds the description as text and HTML and the company's industry, website, LinkedIn, tech stack, benefits and Glassdoor ratings |
| Leave out words (`excludeTerms`) | Drops jobs whose title has these words, such as senior or intern |
| Job type (`employmentType`) | full-time or intern: the only two kinds Instahyre lists |
| Company size (`companySize`) | small (up to 50 people), medium (50 to 200) or large (over 200) |
| Only these companies (`companies`) | Company names, such as Flipkart, or a company's Instahyre page (instahyre.com/jobs-at-zomato) |
| Job links to check (`jobUrls`) | Paste job links to check whether they are still open, instead of searching |

Example input:

```json
{
  "searchTerms": ["python developer"],
  "location": ["Bangalore"],
  "experienceYears": "3",
  "postedWithin": "30 days",
  "maxJobs": 100
}
```

## What does the output look like?

One row per job, newest first. These rows are from a local run of the example input (`{"maxJobs": 100}`) on 2026-11-08: the 100 newest jobs on Instahyre, all posted on 2026-11-07, in 85 s.

| Job title (`title`) | Company name (`company`) | Main city (`location`) | Experience from (`experienceMin`) | Experience up to (`experienceMax`) | Posted on (`postedAt`) |
|---|---|---|---|---|---|
| Senior ServiceNow Engineer | Morningstar | Mumbai | 6 | 8 | 2026-11-07 |
| Manager, Application Software Engineering | Oracle | Hyderabad | 9 | 13 | 2026-11-07 |
| Dot Net Fullstack Developer | Persistent Systems | Pune | 2 | 5 | 2026-11-07 |
| SAP BTP Technical - Senior Associate | PricewaterhouseCoopers (PwC) | Hyderabad | 5 | 9 | 2026-11-07 |
| IAM Developer | Wolters Kluwer | Pune | 3 | 5 | 2026-11-07 |

One row as JSON:

```json
{
  "title": "Manager, Application Software Engineering",
  "company": "Oracle",
  "location": "Hyderabad",
  "otherLocations": [],
  "workType": "onsite",
  "employmentType": "full-time",
  "department": "Software Engineering",
  "salary": null,
  "postedAt": "2026-11-07",
  "jobUrl": "https://www.instahyre.com/job-450563-manager-application-software-engineering-at-oracle-hyderabad/",
  "applyUrl": "https://www.instahyre.com/job-450563-manager-application-software-engineering-at-oracle-hyderabad/",
  "status": "open",
  "platform": "instahyre",
  "companySlug": null,
  "companyWebsite": null,
  "jobId": "450563",
  "checkedAt": "2026-11-08T01:47:07+00:00",
  "experienceMin": 9,
  "experienceMax": 13,
  "skills": ["Angular", "C#", "Java", "JavaScript", "React", "TypeScript", "Vue"],
  "jobFunctions": ["Engineering Management", "Full-Stack Development", "Other Software Development"],
  "companyEmployees": "1000+",
  "companySize": "large",
  "companyFounded": 1982,
  "companyTagline": "Create the future with us",
  "companyLogo": "https://media.instahyre.com/images/profile/base/employer/1532/70ec221bfd/oracle_logo.webp",
  "relocationOk": true,
  "agencyName": null,
  "internshipMonths": null,
  "internshipStart": null
}
```

Full details add `description`, `descriptionHtml`, `companySlug`, `companyWebsite`, `companyIndustry`, `companyLinkedin`, `companyTechStack`, `companyBenefits`, `companyRating`, `companyRatings` (Glassdoor's overall, work-life balance, salary and benefits, culture, career growth, diversity and recommend-to-a-friend scores), `companyPage`, and the place's `city`, `region` (the Indian state), `country` and `countryCode`. In a local run for sales or operations jobs in Mumbai with details on (2026-11-08, 100 rows), the description was filled on 100, the company website on 98, the industry on 90, LinkedIn on 87 and the Glassdoor rating on 49. A checked link that is closed or not found comes back with its `status`, company and link, and the other fields empty. A run also writes an `OUTPUT` record: how Instahyre was read, how many jobs matched and were saved, and any notes on how your input was read.

## How fast is it?

About three and a half minutes for the 100 newest jobs, measured on Apify on 2026-11-08 at the default 512 MB: the empty form took 215 s, python developer in Bangalore 86 s (66 jobs), jobs open to freshers 128 s (100 jobs), sales or operations jobs in Mumbai 122 s (100 jobs) and 173 s with full details, data scientist jobs asking 8 or more years from the last 30 days 209 s (44 jobs), and 500 jobs 970 s. Instahyre limits each address, not each run: about 20 searches a minute and 250 an hour, and about 1,000 job answers an hour; the 500-job run met both, and a run then reads the jobs' own pages instead of their answers. More memory does not make a run faster: the runs used 62 to 107 MB, and the same 100 newest jobs took 207 s at 1,024 MB.

## Common questions

### Where does the posting date come from?

Instahyre Jobs Scraper reads the posting date from each job's own page, where Instahyre states it for search engines (`datePosted`); Instahyre shows it nowhere in its search. Instahyre also gives job numbers in the order jobs are posted, so two pages posted on the same day date every job numbered between them, and a run reads only the pages it needs. On 2026-11-08, 20 of 20 delivered job links checked by HTTP carried the same date as their row.

### Why is newest first not the order on instahyre.com?

Instahyre Jobs Scraper orders jobs by when they were posted, while Instahyre's own search orders them by its own score, which mixes new jobs with jobs listed for months and puts the jobs it has not scored yet, often the newest, last. So the first page of instahyre.com and the first rows here differ for the same search; the counts are Instahyre's own (the `OUTPUT` record and the message say how many jobs Instahyre lists for your filters).

### How does the experience filter work?

Instahyre Jobs Scraper's Experience (`experienceYears`) keeps the jobs whose experience range overlaps yours. Type a number, a range, 5+ or fresher: 3 keeps jobs asking 2-5 or 3-7 years and leaves out 5-9; 2-5 keeps every job whose range touches 2 to 5 years, from 0-2 to 5-9; 5+ keeps the jobs open to five years or more; fresher (or 0) keeps the jobs open to freshers, internships included: every internship on Instahyre asks for 0-0 years. One number also goes to Instahyre's own search, which keeps jobs the same way; a range or 5+ is checked against each job's own range. On 2026-11-08, python developer in Bangalore with 2-5 gave the 20 newest of the 45 jobs whose range touches 2 to 5 years.

### What if a search finds nothing?

Instahyre Jobs Scraper says why in the run's message and in its `OUTPUT` record, and charges for no job. Instahyre's own search takes your words with the place, one number of years, work type, job type and company size, so when it has nothing there the message says so and what to loosen: on 2026-11-08, underwater basket weaving in Bangalore ended "No open job matched on Instahyre in 0 s. Instahyre has no job with your words inside your other filters: try fewer words, or loosen the place, period or other filters." The message also shows how your input was read.

### Why does a skill find jobs without it in the title?

A search word in Instahyre Jobs Scraper matches the job title or one of the skills Instahyre tags the job with, because people search Instahyre by skill: a Backend Engineer job tagged Python is a Python job. Each word must be in the same title or the same skill tag, so java does not find JavaScript and python developer needs both words together.

### Does it show salaries?

Instahyre shows no pay for full-time jobs, so Instahyre Jobs Scraper has none to give. For internships it gives the monthly stipend in rupees when the company shows it (`salary`, and with details `salaryMin`, `salaryMax`, `salaryCurrency` and `salaryPeriod`), with the internship's length and start date.

### Does it need a login or an API key?

Instahyre Jobs Scraper needs no Instahyre account and no API key: it reads the public JSON and pages that instahyre.com shows any visitor. Applying to a job needs an Instahyre account, on Instahyre. You need only an Apify account.

### Does it work on Apify's free plan?

Instahyre Jobs Scraper works on Apify's free plan, which pays the base price: $0.00019 a job plus the $0.013 run start. The free $5 monthly credit pays for about 15,600 jobs in runs of 100, at $0.032 a run.

### How often should I run it?

Running Instahyre Jobs Scraper once a day keeps a job feed fresh: set Posted in the last (`postedWithin`) to 24 hours and Number of jobs (`maxJobs`) to 0 to get every job posted that day. Set the run up under Schedules in Apify Console, and match rows on `jobId` to skip jobs you already have.

### How do I get every job of one company?

To get every open job of one company with Instahyre Jobs Scraper, type its name in Only these companies (`companies`), such as Flipkart, or paste its Instahyre page (instahyre.com/jobs-at-flipkart), and set Number of jobs (`maxJobs`) to 0. Only that company's jobs are read.

### How do I call it from the API, Python, JavaScript, n8n or an AI agent?

Instahyre Jobs Scraper runs from the Apify API, Python, JavaScript, n8n, Make or an AI agent over MCP. Each way uses your Apify token (Apify Console, Settings, API & Integrations) and takes the input as JSON keyed by the field names, such as `searchTerms` and `maxJobs`.

**API.** One call runs the actor and returns its rows (Apify stops that wait after 300 seconds; for bigger runs use a client below, which waits until the run ends):

```bash
curl -X POST "https://api.apify.com/v2/acts/anshumanatrey~instahyre-jobs-search/run-sync-get-dataset-items" \
  -H "Authorization: Bearer <YOUR_APIFY_TOKEN>" \
  -H "Content-Type: application/json" \
  -d '{"searchTerms": ["python developer"], "location": ["Bangalore"]}'
```

**Python** (`pip install apify-client`):

```python
from apify_client import ApifyClient

client = ApifyClient("<YOUR_APIFY_TOKEN>")
run = client.actor("anshumanatrey/instahyre-jobs-search").call(run_input={"searchTerms": ["python developer"], "location": ["Bangalore"]})
for row in client.dataset(run.default_dataset_id).iterate_items():  # apify-client 3+; on 2.x use run["defaultDatasetId"]
    print(row["title"], row["company"], row["location"], row["experienceMin"], row["experienceMax"], row["postedAt"])
```

**JavaScript** (`npm install apify-client`):

```js
import { ApifyClient } from 'apify-client';

const client = new ApifyClient({ token: '<YOUR_APIFY_TOKEN>' });
const run = await client.actor('anshumanatrey/instahyre-jobs-search').call({ searchTerms: ['python developer'], location: ['Bangalore'] });
const { items } = await client.dataset(run.defaultDatasetId).listItems();
for (const row of items) console.log(row.title, row.company, row.location, row.experienceMin, row.experienceMax, row.postedAt);
```

**n8n and Make.** In n8n, add the Apify node, pick Run an Actor and get dataset, choose this actor and paste the input JSON: the rows come out as n8n items. In Make, the Apify app's Run an Actor and Get Dataset Items modules do the same.

**AI agents (MCP).** Add `https://mcp.apify.com?tools=anshumanatrey/instahyre-jobs-search` to your MCP client and sign in with Apify, or send `Authorization: Bearer <YOUR_APIFY_TOKEN>`. The agent gets this actor as a tool and sees every input field by its JSON key.

### Is it legal to use?

Instahyre Jobs Scraper reads public job postings and company profiles that anyone can open without an account, and it collects no candidate data and no recruiter names. You are responsible for how you use the data, including Instahyre's terms and the privacy laws that apply to you, such as India's DPDP Act.

## Limitations

- Instahyre limits each address to about 20 searches a minute and 250 an hour, and to about one and a half job answers a second and 1,000 an hour. A run waits for these limits, reads job pages when the answers run out, says in its message how far it got, and marks the `OUTPUT` record partial when a limit cut it short. Jobs read from their pages have no agency, stipend or relocation flag. An internship's page shows no years of experience, so it gets 0-0, the range every Instahyre internship states in its own answer (64 of 64 on 2026-11-08): Experience 0 (fresher) keeps it, and 1 or more leaves it out.
- The posting date comes from each job's page, which Instahyre serves only to browsers; a run that cannot read the pages delivers the jobs without a date and says so.
- Instahyre shows no salary for full-time jobs and no hybrid work type: a job is in a city (onsite) or Work From Home (remote).
- A word search reads Instahyre's ranking until its pages stop matching; a job that has your words but ranks far below the rest can be missed (1 of 100 python developer jobs on 2026-11-08).
- Jobs Instahyre has not published yet are not listed: the newest job numbers are often unpublished for a day while Instahyre reviews them.
- About 1% of job places are free text outside Instahyre's own list of places (Thane, Abu Dhabi), so a state or country search does not find them; their city name still does.
- One title in the same cities with the same skill tags at one company is delivered once (159 such copies of 13,453 on 2026-11-08).
- The company list behind headcount and founding year was read on 2026-11-08; a company new to Instahyre gets them from its company page during the run.

## Who maintains it?

Built and maintained by **Anshuman Atrey** ([@AnshumanAtrey](https://github.com/AnshumanAtrey)), who publishes a portfolio of data and OSINT actors on Apify Store. For a feature request or a bug, message [LinkedIn](https://linkedin.com/in/anshumanatrey) (fastest), open an issue on the GitHub repo, or write through [atrey.dev](https://atrey.dev).

## Sibling actors

| Actor | What it searches |
|---|---|
| [Greenhouse Jobs Scraper](https://apify.com/anshumanatrey/greenhouse-jobs-search) | Jobs from every company on Greenhouse, searched live |
| [Lever Jobs Scraper](https://apify.com/anshumanatrey/lever-jobs-search) | Jobs from 2,300+ companies on Lever (jobs.lever.co), searched live |
| [Workday Jobs Scraper](https://apify.com/anshumanatrey/workday-job-search) | Jobs from every company on Workday (myworkdayjobs.com), searched live |
| [Ashby Jobs Scraper](https://apify.com/anshumanatrey/ashby-jobs-search) | Jobs from every company on Ashby (jobs.ashbyhq.com), searched live |
| [SmartRecruiters Jobs Scraper](https://apify.com/anshumanatrey/smartrecruiters-jobs-search) | Jobs from 2,900+ companies on SmartRecruiters, searched live |
| [Workable Jobs Scraper](https://apify.com/anshumanatrey/workable-job-search) | Jobs from every company on Workable, in one search |
| [Cornerstone Jobs Scraper](https://apify.com/anshumanatrey/cornerstone-jobs-search) | Jobs from every company on Cornerstone (csod.com), searched live |
| [Deel Jobs Scraper](https://apify.com/anshumanatrey/deel-jobs-search) | Jobs from every company on Deel ATS (jobs.deel.com), with pay |

For the people behind a company: [LinkedIn Profile Finder](https://apify.com/anshumanatrey/linkedin-harvester) turns an email into a public LinkedIn profile.

## Documentation

- Apify Store: https://apify.com/anshumanatrey/instahyre-jobs-search
- GitHub repo: https://github.com/AnshumanAtrey/instahyre-jobs-search (MIT license, see [LICENSE](LICENSE))
- The engine behind it: https://github.com/AnshumanAtrey/ats-jobs-engine

## Last updated

2026-11-08 (version 1.0)
