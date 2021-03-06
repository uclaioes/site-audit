# Site audit

Performance and accessibility review to help design a better user experience

## Google Lighthouse

Google Lighthouse is an open-source, automated tool for improving the quality of web pages. It can be run in [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools) or installed locally and run from the command line.

- [Google Lighthouse](https://developers.google.com/web/tools/lighthouse)
- [Get Started using Lighthouse](https://developers.google.com/web/tools/lighthouse/#get-started)
- [Using Lighthouse on Chrome DevTools](https://developers.google.com/web/tools/lighthouse#devtools)
- [Using Lighthouse on command line](https://developers.google.com/web/tools/lighthouse/#cli)

---

## Cheatsheet

### Install

`npm install -g lighthouse`

See all options

`lighthouse --help`

To run an audit, use `--output` flags to export json, html or both. use `--view` to view report in browser.

`lighthouse https://www.ioes.ucla.edu --output json --output html --view`

`lighthouse https://www.ioes.ucla.edu --output html --view`

`lighthouse https://www.sustain.ucla.edu --output html --view`

### Test on a site with authentication

When installed globally via `npm i -g lighthouse` or `yarn global add lighthouse`,
`chrome-debug` is added to your `PATH`. This binary launches a standalone Chrome
instance with an open debugging port.

1. Run `chrome-debug`. This will log the debugging port of your Chrome instance
1. Navigate to your site and log in.
1. In a separate terminal tab, run `lighthouse http://mysite.com --port port-number` using the port number from chrome-debug.
1. ex. `lighthouse https://dev.ioes.ucla.edu --port portnumber --output json --output html --view` with json and html outputs.

### View and share reports

- [Share repots online](https://developers.google.com/web/tools/lighthouse#report-viewer)
- [Share reports as JSON](https://developers.google.com/web/tools/lighthouse/#json)
- [Share reports as GitHub Gists](https://developers.google.com/web/tools/lighthouse/#gists)
- [Lighthouse viewer](https://googlechrome.github.io/lighthouse/viewer/)

Reports are saved in the directory command is run. If you want to output path to another folder use `--output-path`

ex: `lighthouse --output json --output-path <path/for/output.json>`

To view a report that's been saved as a Gist:

Add `?gist=<ID>` to the Viewer's URL, where `<ID>` is the ID of the Gist.

`https://googlechrome.github.io/lighthouse/viewer/?gist=<ID>`

Open the [Viewer](https://googlechrome.github.io/lighthouse/viewer/), and paste the URL of a Gist into it. Or upload the json file.

---

## IoES Lighthouse reports
### [www.ioes.ucla.edu](https://www.ioes.ucla.edu)

All test results are saved in the [reports](https://github.com/uclaioes/site-audit/tree/master/reports) folder in this repo. 

### 2021

1. [2021-02-19 / 99, 100, 100,100](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu_2021-02-19_14-56-51.report.html)
1. [2021-02-19 / 98, 100, 100, 100](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu_2021-02-19_14-28-48.report.html)
1. [2021-02-19 / 80, 100, 100, 100](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu_2021-02-19_09-07-57.report.html)


### Past reports

1. [2020-01-09 4:38PM](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu_2020-01-09_16-35-29.report.html)
1. [2019-11-26 13:54pm, desktop, CPU throttling 4x slowdown simulated](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu_2019-11-26_13-54-52.report.html)
1. [2019-11-26 10:06am, desktop, CPU throttling 4x slowdown simulated ](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu-2019-11-26-T10-06-44.html)
1. [2019-11-26 10:00am, desktop, no CPU throttling](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu-2019-11-26-T10-00-29.html)
1. [2019-11-26 9:56am, mobile, CPU throttling 4x slowdown simulated](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu-2019-11-26-T09-56-21.html)
1. [2019-11-26 9:50am, mobile, CPU throttling 4x slowdown simulated](https://uclaioes.github.io/site-audit/reports/www.ioes.ucla.edu_2019-11-26_09-50-39.report.html)


---


## Google links

- [Web Fundamentals](https://developers.google.com/web/fundamentals)
- [Design and UX Basics](https://developers.google.com/web/fundamentals/design-and-ux/ux-basics)
- [Auditing Performance](https://developers.google.com/web/fundamentals/performance/audit)
- [Accessibilty Basics](https://developers.google.com/web/fundamentals/accessibility)
- [Auditing Accessiblity](https://developers.google.com/web/fundamentals/accessibility/how-to-review)

---

## Online Course

- [Website Performance Optimization by Google](https://www.udacity.com/course/website-performance-optimization--ud884)

