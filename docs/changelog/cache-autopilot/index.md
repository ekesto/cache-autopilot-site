---
layout: default
title: Cache Autopilot Changelog
---

## Cache Autopilot Changelog

> Note: Free and PRO packages share the same version number. Some releases may only affect PRO features, but version alignment keeps package compatibility, support, and upgrade paths consistent.

### 1.1.10
*Release Date 22nd August 2026*

* Enhancement: Polished the settings experience with clearer user search feedback and priority controls that follow the selected WordPress admin color scheme.
* Fix: Made warmup transport diagnostics clearer and more accurate about browser-profile requests and standard fallbacks.
* Fix: Prevented Elementor autosaves from triggering premature cache refreshes.

### 1.1.9
*Release Date 14th August 2026*

* Enhancement: Preserved the active WPML language after multilingual form changes.
* Enhancement: Updated WordPress compatibility to 7.1.
* Fix: Ensured shared block theme changes refresh all affected pages when template usage cannot be resolved completely.

### 1.1.8
*Release Date 13th August 2026*

* Enhancement: Warmup diagnostics are now cleaner, easier to understand, and more precise about browser-profile performance and fallbacks.
* Enhancement: Priority pages and Home now start multilingual full refreshes in the right order across configured languages.
* Enhancement: Improved settings navigation and made priority-page choices easier to refresh reliably.

### 1.1.7
*Release Date 12th August 2026*

* Enhancement: Improved targeted Brotli cache warming compatibility by routing browser-profile requests through the WordPress HTTP API.
* Enhancement: Full cache refreshes now begin rebuilding pages promptly after manual actions and automated updates.

### 1.1.6
*Release Date 29th July 2026*

* Improvement: Added a dedicated, lightweight kick for new warmup runs on sites using server cron, without triggering unrelated WordPress cron tasks.

### 1.1.5
*Release Date 28th July 2026*

* Fix: Prevented overlapping warmup runs from becoming stuck while preparing after concurrent plugin or theme updates.

### 1.1.4
*Release Date 27th July 2026*

* Fix: Improved targeted warmup coordination for late-arriving URLs and concurrent multilingual invalidations.
* Fix: Resolved WPML post type archive URLs in their target-language context.
* Fix: Made targeted run labels distinguish distinct content changes from related multilingual emissions.
* Enhancement: Improved warmup log clarity and status presentation.

### 1.1.3
*Release Date 7th July 2026*

* Enhancement: Release workflow optimizations.

### 1.1.2
*Release Date 6th July 2026*

* Security: Hardened trusted cache-clear handling and plugin access checks.
* Fix: Improved support-log protection, cron loopbacks, and internal storage prefixes.
* Fix: Resolved remaining Plugin Check naming warnings for legacy plugin constants.

### 1.1.1
*Release Date 25th June 2026*

* Fix: Preserved settings when deleting Free or PRO while the other edition remains installed.

### 1.1.0
*Release Date 23nd June 2026*

* Fix: Improved WordPress.org compatibility for plugin prefixes, admin notices, diagnostics data, and cache purge permissions.

### 1.0.2
*Release Date 19th June 2026*

* Fix: Improved Plugin Check compatibility for PRO integrations.

### 1.0.1
*Release Date 19th June 2026*

* Enhancement: Admin notification optimized for first installs.

### 1.0.0
*Release Date 18th June 2026*

* Initial public release of Cache Autopilot after extended production use on real WordPress sites, including large installations with more than 1,200 pages.
* Added Free/PRO-ready internal structure while keeping the free plugin fully functional on its own.
* Preserved historical changelogs for the former two separate plugins [Cache Invalidator](https://ekesto.github.io/cache-autopilot-site/docs/changelog/cache-invalidator/) and [Cache Warmup](https://ekesto.github.io/cache-autopilot-site/docs/changelog/cache-warmup/).
