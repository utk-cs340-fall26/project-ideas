# Climate Influence Money Map

## A brief summary of the project idea  

Climate Money Map is a mobile app that makes it easy to trace how money and lobbying intersect with US climate policy. Users can look up a company, industry, legislator, or bill and see a clear view of campaign donations, lobbying activity, and legislative actions over time. The goal is not to tell people what to think, but to make primary records legible and comparable so accountability research doesn’t require expertise.

## What problem it solves  

Some of the biggest climate outcomes are driven by policy choices around energy, transportation, methane regulation, and permitting. Yet the public data that could help voters and researchers evaluate influence is fragmented across different databases, filed in inconsistent formats, and often buried behind jargon. People who want to understand who is trying to shape climate legislation usually have to bounce between many different sources spread out throughout the web. That friction keeps the “follow the money” story out of reach for most people and makes it easier for influence to operate unnoticed. This project lowers that barrier and includes citations so every claim can be verified.

## A list of major features  

- Legislator profiles with top funding sources, climate related vote history, and sponsored bills  
- Company and industry pages showing lobbying spend over time, issue areas, and bill references when available  
- Bill pages with status, vote outcomes, and related lobbying patterns by industry  
- Relationship visualizations that connect industries, committees, legislators, and key votes  
- Watchlists and notifications for new filings and major legislative events  
- Source first citations for every data point, linking to the original filing or record  
- Basic data quality tooling such as alias management for entity name matching and deduplication

## Technologies you plan to use (languages, tools, third-partyAPIs/libraries)  

- Mobile: React Native with TypeScript  
- Backend: Node.js using Express or NestJS  
- Database: PostgreSQL  
- Data ingestion: scheduled workers and parsers for bulk filings  
- APIs and datasets: FEC API for campaign finance, US Senate LDA lobbying filings for lobbying activity, and a congressional data source such as Congress.gov  
- Deployment: a simple cloud host for the API plus managed Postgres

## Who the intended users are and why they would want this  

This is for voters and advocates who want quick, credible context before contacting representatives or supporting campaigns, and for journalists and students who need a reliable research starting point with citations. They’d use it because it turns scattered public records into an understandable narrative without asking them to trust an opaque “score.”