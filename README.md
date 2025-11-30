# Workable.com Scraper

![banner](https://i.ibb.co/6RhmjDKZ/workable.png)

Automate job data extraction from Workable.com, one of the leading job platforms used by companies worldwide. This powerful scraper collects comprehensive job listings including positions, company details, requirements, and benefits across all industries and locations. Perfect for recruiters monitoring job market trends, HR professionals analyzing hiring patterns, and researchers studying employment opportunities. Get structured data in JSON format with detailed information about job types, workplace arrangements, and company information.

<p align="center">
  <img src="https://apify-image-uploads-prod.s3.us-east-1.amazonaws.com/DevbkY3adMTBuoECt-actor-uZc19CJDttLwZq6ah-hQIsYloty4-idSnpuCQdy_1759818308900.jpeg" alt="Workable.com Scraper" style="height: 60px; margin-right: 15px;" /><a href="https://apify.com/lexis-solutions/workable-com-scraper" target="_blank">
    <img src="https://img.shields.io/badge/Try%20it%20on-Apify-0066FF?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDA4IiBoZWlnaHQ9IjQwOCIgdmlld0JveD0iMCAwIDQwOCA0MDgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxnIGNsaXAtcGF0aD0idXJsKCNjbGlwMF8zNDFfNDE1NykiPgo8cGF0aCBkPSJNMjE4LjY5NSAxMDRIMzAwLjk3QzMwMi42NDMgMTA0IDMwNCAxMDUuMzU3IDMwNCAxMDcuMDNWMjMyLjc2NkMzMDQgMjM1Ljc3OCAzMDAuMDgzIDIzNi45NDUgMjk4LjQzNCAyMzQuNDI1TDIxNi4xNTkgMTA4LjY5QzIxNC44NDEgMTA2LjY3NCAyMTYuMjg3IDEwNCAyMTguNjk1IDEwNFoiIGZpbGw9IndoaXRlIi8+CjxwYXRoIGQ9Ik0xODkuMzA1IDEwNEgxMDcuMDNDMTA1LjM1NyAxMDQgMTA0IDEwNS4zNTcgMTA0IDEwNy4wM1YyMzIuNzY2QzEwNCAyMzUuNzc4IDEwNy45MTcgMjM2Ljk0NSAxMDkuNTY2IDIzNC40MjVMMTkxLjg0IDEwOC42OUMxOTMuMTU5IDEwNi42NzQgMTkxLjcxMyAxMDQgMTg5LjMwNSAxMDRaIiBmaWxsPSJ3aGl0ZSIvPgo8cGF0aCBkPSJNMjAyLjU5MSAyMDQuNjY4TDEwOS4xMjcgMjk4LjgzNUMxMDcuMjI5IDMwMC43NDcgMTA4LjU4MyAzMDQgMTExLjI3OCAzMDRIMjk2LjhDMjk5LjQ4MyAzMDQgMzAwLjg0MiAzMDAuNzcgMjk4Ljk2NyAyOTguODUyTDIwNi45MDggMjA0LjY4NUMyMDUuNzI2IDIwMy40NzUgMjAzLjc4MiAyMDMuNDY4IDIwMi41OTEgMjA0LjY2OFoiIGZpbGw9IndoaXRlIi8+CjwvZz4KPGRlZnM+CjxjbGlwUGF0aCBpZD0iY2xpcDBfMzQxXzQxNTciPgo8cmVjdCB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEwNCAxMDQpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==&logoColor=white" alt="Try it on Apify" style="border-radius: 12px; height: 60px;" />
  </a>
</p>


👋 Welcome to the Workable.com Scraper, an actor designed to help you gather job listings from Workable.com! With this actor, you can easily search for jobs across different industries and locations worldwide.

## Use Cases

## 📊 Actor Stats

| Stat | Value |
|------|-------|
| **Version** | `0.0.3` |
| **Last Update** | Nov 30, 2025 |

---



Here are some typical scenarios in which the Workable.com Scraper can be useful:

- **Job Seekers** can use the scraper to find positions matching their skills and location preferences
- **Recruiters** can use the scraper to monitor market trends and competitor job postings
- **HR Professionals** can use the scraper to analyze hiring patterns and salary ranges
- **Market Researchers** can use the scraper to study employment trends across different industries and regions

## Input 📥

To use this actor, you need to provide the following input:

- Field: **query**
  - Type: string
  - Required: Yes
  - Description: Search query for job titles, skills, or keywords
- Field: **maxItems**
  - Type: integer
  - Required: No
  - Description: Maximum number of items to scrape
  - Default: 10
- Field: **since**
  - Type: string
  - Required: No
  - Description: Filter results by date. Supports relative formats (d7, m1, y1) or absolute dates (YYYY-MM-DD)
  - Default: "m1" (past month)
  - Examples:
    - `"d7"` - Last 7 days
    - `"m1"` - Last month
    - `"y1"` - Last year
    - `"2024-01-15"` - Since January 15, 2024
- Field: **proxyConfiguration**
  - Type: object
  - Required: No
  - Description: Your proxy configuration from Apify
  - Default: Uses Apify Proxy with no specific proxy groups

## Output 📤

An example output looks like this:

```json
{
  "url": "https://apply.workable.com/coresite/j/FF99CB5CDD/",
  "searchQuery": "Project Manager",
  "searchDate": "2025-10-01T22:28:22.631Z",
  "originalTitle": "Senior Construction Project Manager (SV9) (1693) - CoreSite",
  "originalSnippet": "The Construction Senior Project Manager is responsible for overseeing all aspects of assigned capital construction projects.",
  "jobTitle": "Senior Construction Project Manager (SV9) (1693)",
  "company": "CoreSite",
  "logoUrl": "https://workablehr.s3.amazonaws.com/uploads/account/logo/373150/logo",
  "location": "Santa Clara, California, United States",
  "jobType": "Full time",
  "jobDepartment": "Construction",
  "jobWorkplace": "Hybrid",
  "salary": "$150,000 - $175,000",
  "description": "DescriptionAbout CoresiteAt CoreSite, we empower a more connected future through high-performance data centers...",
  "requirements": "RequirementsKnowledge, Skills & Abilities: Ability to thrive in a hybrid work environment...",
  "benefits": "BenefitsNot only does CoreSite have a fun, team-focused work environment...",
  "deadline": "",
  "postedDate": "2025-09-03",
  "extractedAt": "2025-10-01T22:28:50.073Z",
  "source": "workable"
}
```

## How many listings can the Workable.com Scraper extract?

The Workable.com Scraper uses pagination to extract job listings from Workable.com. You can control the number of listings to scrape by setting the `maxItems` input parameter. If you don't set the `maxItems` parameter, the scraper will extract up to 10 listings by default.

## Date Filtering 📅

The scraper supports powerful date filtering to help you find the most relevant and recent job postings:

- **Relative Date Formats**: Use `d7` for last 7 days, `m1` for last month, `y1` for last year
- **Absolute Date Formats**: Use `YYYY-MM-DD` format for specific dates (e.g., `2024-01-15`)
- **Default Behavior**: If no `since` parameter is provided, the scraper defaults to the last month (`m1`)

### Example Usage

```json
{
  "query": "software engineer",
  "maxItems": 50,
  "since": "d7"
}
```

This will find software engineer jobs posted in the last 7 days, up to 50 results.

## Why use the Workable.com Scraper?

- ⚡️ **Fast** - The scraper efficiently handles complex job postings and company information.

- 🤙 **Easy to use** - Simply input your search criteria and let the scraper handle the complexities of job data extraction.

- 🌐 **Comprehensive** - Extracts detailed job information including descriptions, requirements, benefits, and company details.

- 📅 **Date-Filtered** - Filter results by specific time periods to find the most recent and relevant job postings.

- ☑️ **Well-Maintained** - The scraper is maintained by the Lexis Solutions team, ensuring reliable performance.

## Limitations

- The scraper will return a maximum of 1000 results per search.
- Some job postings may have limited information depending on how companies structure their listings.

## FAQ 💬

- **What is Workable.com?**

  Workable.com is a leading job platform used by companies worldwide to post job openings and manage their hiring process. It's used by startups to Fortune 500 companies.

- **How can I find jobs on Workable.com?**

  You can find jobs by visiting Workable.com and using their search function. The Workable.com scraper automates this process by extracting listings based on your specified criteria.

- **Can I use the Workable.com scraper to apply for jobs?**

  No, the Workable.com scraper is for data extraction and analysis only. It should not be used to submit applications or interact with the website directly.

- **What types of jobs can the Workable.com scraper find?**

  The scraper can find any type of job listed on Workable.com, including:

  - Full-time positions
  - Part-time jobs
  - Contract roles
  - Remote positions
  - Hybrid positions
  - Executive positions

- **How does the date filtering work?**

  The `since` parameter allows you to filter job postings by their publication date. You can use relative formats like `d7` (last 7 days), `m1` (last month), or `y1` (last year). You can also use absolute dates in `YYYY-MM-DD` format. This helps you find the most recent and relevant job opportunities.

- **What if the website changes?**

  Website changes may affect the scraper's functionality. In such cases, our team will update the scraper to maintain compatibility. We regularly monitor and maintain our scrapers to ensure reliable operation.

## Need to scrape other job platforms?

Here are some other job platform scrapers you might find useful:

- Germany 🇩🇪

  - [Arbeitsagentur Scraper](https://apify.com/lexis-solutions/bundesagentur-fur-arbeit-arbeitsagentur-scraper)

- Netherlands 🇳🇱

  - [Werk.nl Scraper](https://apify.com/lexis-solutions/werk-nl-scraper)

- United Kingdom 🇬🇧

  - [Reed.co.uk Scraper](https://apify.com/lexis-solutions/reed-co-uk-scraper)
  - [TotalJobs Scraper](https://apify.com/lexis-solutions/totaljobs-scraper)

- France 🇫🇷

  - [HelloWork Scraper](https://apify.com/lexis-solutions/hellowork-scraper)

- Switzerland 🇨🇭

  - [Jobs.ch Scraper](https://apify.com/lexis-solutions/jobs-ch-scraper)

---

👀 p.s.

Got feedback or need an extension?

Lexis Solutions is a [certified Apify Partner](https://apify.com/partners). We can help you with custom solutions or data extraction projects.

Contact us over [Email](mailto:info@lexis.solutions) or [LinkedIn](https://www.linkedin.com/company/lexis-solutions)
