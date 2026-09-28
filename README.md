# Cache Autopilot

Cache Autopilot is a WordPress cache freshness plugin built around **two separate engines working together**:

* **Cache Invalidator** determines which pages are affected by a change and purges those cached entries through your existing cache plugin.
* **Cache Warmup** rebuilds the purged pages safely in the background.

Together, they provide targeted cache refresh without unnecessarily flushing the entire site cache.

**Cache Autopilot Free is available on WordPress.org:**  
[wordpress.org/plugins/cache-autopilot](https://wordpress.org/plugins/cache-autopilot/)

This repository contains the public changelog history for Cache Autopilot Free and PRO:

* [Cache Autopilot changelog](https://ekesto.github.io/cache-autopilot-site/docs/changelog/cache-autopilot/)

Full documentation lives on the product website. This repository exists primarily for release transparency and changelog history.

Website:  
[wpcacheautopilot.com](https://wpcacheautopilot.com)

## How it works

Cache Autopilot does not replace your cache plugin. Your cache plugin handles cache storage and delivery; Cache Autopilot handles cache freshness through its two engines.

Lifecycle:

1. Cache Invalidator detects a change
2. It resolves the affected pages
3. Those URLs are purged through the active cache plugin
4. Cache Warmup takes over
5. The purged pages are rebuilt through paced background HTTP requests

This keeps unaffected pages cached while refreshing the pages that actually need it.

## Cache Invalidator

Cache Invalidator is the decision layer. It determines which pages are affected by a change and sends those URLs to the active cache adapter.

Free includes support for:

* Posts and custom post types
* Post type, taxonomy and date archives
* Configurable archive pagination
* Comments and relevant meta changes
* Gutenberg and block-theme structures
  * Templates
  * Template parts
  * Synced patterns
  * Navigation
  * Global styles
* Supported form-plugin propagation
* Menus, widgets, Customizer and theme changes
* Relevant WordPress settings
* WooCommerce
* Manual URL targeting
* Selected-page, all-page and full-purge fallback modes
* Developer filters for custom resolution workflows
* Debug and support logging

PRO adds advanced resolution capabilities including:

* Elementor
* ACF relationships
* Custom content relationships
* Multilingual sites
* Timed invalidation
* Access-control role and user overrides
* Advanced Post Type configuration

When Cache Autopilot cannot safely determine every affected page, it can fall back to broader refresh behaviour rather than leave stale content behind.

## Cache Warmup

Cache Warmup is the execution layer. After affected pages are purged, it rebuilds them through controlled background HTTP requests.

Capabilities include:

* Targeted preload of purged URLs
* Full-site cache preloading
* Paced background execution
* Automatic batch sizing
* Priority ordering
* Manual URL exclusions
* Diagnostics and run history

The result is less cold-cache traffic after content changes and fewer reasons to manually clear an entire site cache.

## Integrations

Cache Autopilot works alongside supported WordPress cache plugins and uses their URL-level purge capabilities.

Supported integrations currently include cache plugins such as LiteSpeed Cache, WP Rocket, FlyingPress, Cache Enabler, Breeze and others.

Compatibility depends on the cache plugin exposing a reliable URL-level purge mechanism and, in some cases, the hosting environment.

See [Supported Integrations](https://wpcacheautopilot.com/docs/supported-integrations/) for the current compatibility list.

## Free and PRO

**Cache Autopilot Free is a permanent, useful standalone plugin — not a trial.**

It includes Cache Warmup, WordPress content and presentation handling, Gutenberg and block-theme support, WooCommerce, supported forms, developer extension points and all supported cache adapters.

**Cache Autopilot PRO** adds advanced integrations and content propagation capabilities for more complex WordPress setups, including Elementor, ACF relationships, multilingual sites, custom relationships, timed invalidation and access-control configuration.

Free and PRO share the same source codebase and aligned version numbers.

## Who it's for

Cache Autopilot is built for WordPress developers, agencies and technical site owners who want reliable cache freshness without relying on manual cache clears or unnecessary full-site purges.

A typical workflow is:

> You build the site.  
> You configure Cache Autopilot.  
> You hand it over.
>
> Client publishes.  
> The right pages refresh.

## Links

**Cache Autopilot Free on WordPress.org**  
[wordpress.org/plugins/cache-autopilot](https://wordpress.org/plugins/cache-autopilot/)

**Website**  
[wpcacheautopilot.com](https://wpcacheautopilot.com)

**Documentation**  
[wpcacheautopilot.com/docs](https://wpcacheautopilot.com/docs/)

**Getting Started**  
[wpcacheautopilot.com/docs/getting-started](https://wpcacheautopilot.com/docs/getting-started/)

**Supported Integrations**  
[wpcacheautopilot.com/docs/supported-integrations](https://wpcacheautopilot.com/docs/supported-integrations/)

**Support**  
[wpcacheautopilot.com/support](https://wpcacheautopilot.com/support/)

## Maintainer

Developed and maintained by Beat Schenkel (ekesto), independent WordPress developer:

[ekesto.com](https://ekesto.com)
