How Rich Are You, Really?

A free income percentile calculator for US households. Enter a pre-tax household income and instantly see what percentage of American households you out-earn.

Live demo → (replace with your GitHub Pages URL once deployed)

What it does
Takes a single input: annual pre-tax household income
Returns the percentile it falls into, relative to all US households
Shows a visual bar and a one-line, shareable result
Includes a "Copy my result" button for easy sharing
Data source

Percentile breakpoints are based on 2025 US household income data (income earned in 2024), from DQYDJ's analysis of IPUMS CPS microdata:

Percentile	Household income
25th	$41,401
50th (median)	$83,592
75th	$153,000
90th	$251,036
95th	$335,575
99th (top 1%)	$659,060

Percentiles between published data points are estimated by log-space interpolation, so results are close approximations rather than exact figures.

Tech

Single self-contained HTML file — no build step, no framework, no backend, no dependencies, no tracking. Works by dragging the file onto any static host.

Running locally

Just open index.html in a browser. No server or install required.

Deploying

Any static host works: GitHub Pages, Netlify, Vercel, Cloudflare Pages, etc. For GitHub Pages: upload index.html to this repo, then enable it under Settings → Pages.

Updating the data

Income percentile breakpoints will shift each year as new Census/IPUMS data is published. To refresh:

Find the latest household income percentile breakpoints (e.g. from DQYDJ's household income percentile calculator)
Update the points array near the top of the <script> section in index.html
Update the stats shown in the .stats block and the table above in this README
License

Free to use, modify, and deploy.

Content
