---
layout: default
title: Cache Autopilot Changelog
---

## Cache Autopilot Changelog

> Auto-generated from the plugin changelog. Source of truth lives in the plugin repository.

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
* Preserved historical changelogs for the former two separate plugins Cache Invalidator and Cache Warmup.
