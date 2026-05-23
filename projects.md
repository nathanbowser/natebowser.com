# Projects

A few systems I’ve spent real time with: visualization platforms, component libraries, website infrastructure, AI automation, and founder-close product work. Most of this is Spider Impact and the work around it: a single long-lived product where I built the visualization layer, then the libraries underneath, then the website and AI stack on top.

## Spider Impact visualization platform

Built the visualization and dashboard-editing platform behind Spider Impact: data stories, charting, earned value visuals, clustering explainers, shape tools, maps, and free-form dashboard editing. The centerpiece is a 10+ year dashboard editor for composing, editing, and presenting dashboard objects without losing stability.

- Dashboard canvas with Keynote-like editing in the browser: selection, marquee, snap lines, autoscroll, history stacks, RTL support, and Bezier connectors between dashboard objects.
- SVG shape library with 40+ fully customizable primitives, fills, strokes, handles, labels, and Keynote-like manipulation in the browser.
- Reusable chart engine with animated transitions, forecasting, labels, legends, axes, palettes, exports, and chart types across bar, line/area, pie, polar, map, treemap, timeline, funnel, process, pyramid, regression, waffle, and wafflegrid views.
- Earned value forecasting interactives with sliders for work completed and money spent, showing projected schedule and budget outcomes as assumptions move.
- D3 map components with projections, pan/zoom interaction, filled regions, bubbles, spikes, clustering, and dashboard-safe rendering.
- K-means-style clustering explainers that group records by mathematical distance, turning scattered customer data into segments people can act on.

Product UI is shown for engineering context. My work focused on implementation, component architecture, performance, and browser behavior.

## Impact component libraries

Product-grade UI primitives built because Spider Impact needed behavior that generic packages did not quite provide.

- Kalpa Tree: core Spider Impact navigation infrastructure; hierarchical D3 tree built for large browser datasets, streaming nodes, selection, drag/drop reparenting, and performance mode. It handles 50K+ nodes while keeping the browser responsive. Public GitHub: https://github.com/SpiderStrategies/kalpa-tree
- Enclosure: drag/drop layout engine for nested rows, columns, stacks, placeholders, and animated reflow.
- Cleaver: JSON exploration and path selection UI for making structured data easier to inspect and target.
- Rich Select: rich select for massive hierarchical datasets: hundreds of thousands of nodes, fast search, custom rendering, keyboard behavior, and product-specific selection rules.

Also built: Inception for stacked browser views, Vogue for image cropping, and other small UI utilities that solved specific product problems without becoming frameworks.

## Web, CMS, and AI architecture

Recently I’ve focused on the Spider Strategies website stack: static SEO architecture on AWS, Lighthouse and Core Web Vitals tuning, custom CMS tooling, sales lead flow, and a public agent service that makes site, support, and API knowledge readable to both humans and AI.

- SpiderStrategies.com: static site generator architecture, SEO content systems, visual pages, gated content, agent corpus, OpenAPI publishing, and S3/CloudFront deploy tooling.
- Public interactive explainers: data clustering and forecasting on https://www.spiderstrategies.com/business-intelligence/, plus EVM prediction charts and sliders on https://www.spiderstrategies.com/earned-value-management/.
- AWS operations: S3 publishing, CloudFront invalidation and response-header policies, CloudFront Functions for markdown negotiation, Route 53/DNS coordination, and staging/production deployment paths.
- Lead flow: contact and insight forms that connect marketing pages to sales workflows without turning the site into a brittle app.
- Weaver: custom CMS for blog, documents, images, gated assets, prompt overrides, GitHub-backed editing, and deploy workflows.
- Anansi: MCP and HTTP service behind agents.spiderstrategies.com, served through CloudFront with an EC2/nginx/Node origin, systemd deploys, health checks, and cited retrieval over website, support, and API corpora.
- Agent operations: practical workflows across Codex, Claude, Cursor, custom prompts, quality gates, and codebase-specific rules.

## Dash

Worked directly with the founder on Dash, an internal company spinoff that was eventually shut down but fed ideas and technology back into the main product. The work mixed modern-for-the-time frontend architecture with homegrown visualization and dashboard components.

- Dashboard app, widget framework, charts, gauges, goal widgets, and free-form canvas composition.
- Third-party integrations, OAuth flows, realtime push services, image processing, thumbnails, sitemaps, queues, and deployment/server tooling.
- Useful product lessons that later informed Spider Impact’s dashboard, visualization, and component architecture.

## Developer enablement and technical training

Before Spider Strategies, delivered enterprise software-development seminars and mentored developers on Java/JEE, Spring, Hibernate/JPA, application design, and best-practice coding. That training background now carries into AI adoption: helping engineers use agents as leverage without giving up clarity, ownership, or maintainability.

- Delivered seminars for large enterprise audiences, including Boeing, the IRS, FedEx, Wells Fargo, and Morgan Stanley.
- Served as lead instructor and mentor for a Java immersion initiative at a 100,000+ employee corporation.
- Wrote technical exercises and taught practical frameworks from real consulting experience rather than stale academic examples.
