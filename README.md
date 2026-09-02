# Cache Autopilot

Cache Autopilot is a WordPress cache freshness plugin that keeps cached pages fresh after content changes — automatically. Instead of flushing everything on every save, it determines which pages are affected, purges those entries through your active cache plugin, and rebuilds them through controlled background warmup.

**Cache Autopilot Free is available on WordPress.org:**
[wordpress.org/plugins/cache-autopilot](https://wordpress.org/plugins/cache-autopilot/)

This repository contains the public changelog for Cache Autopilot:

* [Cache Autopilot changelog](https://ekesto.github.io/cache-autopilot-site/docs/changelog/cache-autopilot/)

Documentation lives on the product website. This repository exists primarily for release transparency and changelog history.

Visit the website:
[wpcacheautopilot.com](https://wpcacheautopilot.com)

## How it works

Cache Autopilot does not replace cache plugins. Cache plugins handle storage and delivery. Cache Autopilot handles cache freshness — determining which cached pages need to refresh after something changes.

Lifecycle:

1. Detect changes
2. Resolve affected URLs
3. Purge through the active cache adapter
4. Queue warmup requests
5. Rebuild cache through paced background execution

## Included engines

### Cache Invalidator

Determines which WordPress pages are affected by a change and purges their cached entries without unnecessarily clearing the entire cache.

Core capabilities include:

* Post and custom post type invalidation
* Archive and taxonomy targeting
* Gutenberg and block-theme structural support
* Presentation-change handling
* Supported form-plugin propagation
* Manual targeting and fallback modes
* Developer filters for custom workflows
* PRO integrations for advanced content relationships, Elementor, WooCommerce, ACF, multilingual sites and timed invalidation

### Cache Warmup

Rebuilds purged pages so visitors are less likely to hit cold cache entries.

Core capabilities include:

* Targeted preload for purged URLs
* Full-site cache preloading
* Auto-paced background execution via WP-Cron
* Priority ordering
* Diagnostics and run history

## Integrations

Cache Autopilot works alongside supported WordPress cache plugins and uses their URL-level purge capabilities.

Compatibility depends on the cache plugin and hosting environment.

See [Supported Integrations](https://wpcacheautopilot.com/docs/supported-integrations/) for the current compatibility list.

## Free and PRO

Cache Autopilot Free is a permanent standalone plugin available from the official WordPress.org Plugin Directory.

Cache Autopilot PRO adds advanced integrations and resolution capabilities for setups including Elementor, WooCommerce, ACF, multilingual sites, content relationships and timed invalidation.

Free and PRO share the same source codebase and aligned version numbers.

## Who it's for

Cache Autopilot is built for WordPress developers, agencies managing client sites, and technical site owners who need reliable cache freshness without relying on manual cache clears or unnecessary full-site purges.

## Links

WordPress.org:
[wordpress.org/plugins/cache-autopilot](https://wordpress.org/plugins/cache-autopilot/)

Website:
[wpcacheautopilot.com](https://wpcacheautopilot.com)

Documentation:
[wpcacheautopilot.com/docs](https://wpcacheautopilot.com/docs/)

Getting Started:
[wpcacheautopilot.com/docs/getting-started](https://wpcacheautopilot.com/docs/getting-started/)

Support:
[wpcacheautopilot.com/support](https://wpcacheautopilot.com/support/)

## Maintainer

Developed and maintained by Beat Schenkel (ekesto), an independent WordPress developer:
[ekesto.com](https://ekesto.com)
