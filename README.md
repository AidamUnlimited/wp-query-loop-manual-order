# WordPress Query Loop Block — Sorting & Ordering Options (and What's Missing)

The WordPress Query Loop block lets you display posts, pages, and custom post types on any page using the block editor. It comes with built-in sorting options, but if you've ever needed to manually choose which posts appear first, you've probably discovered there's no way to do that.

This guide covers what the Query Loop block can and can't do when it comes to ordering — and how to get full manual control.

---

## Default Query Loop Sorting Options

The core Query Loop block includes these sorting options out of the box:

| Sort By | What It Does |
|---------|-------------|
| **Newest to oldest** | Posts sorted by publish date, most recent first (default) |
| **Oldest to newest** | Posts sorted by publish date, oldest first |
| **A → Z** | Alphabetical by title |
| **Z → A** | Reverse alphabetical by title |

If you're using the [Advanced Query Loop](https://developer.wordpress.org/block-editor/) plugin, you also get:

- Menu order
- Random
- Modified date
- Comment count

These cover basic use cases. But they all share the same limitation.

## What You Can't Do

**You can't manually pick which posts appear first.**

There's no drag-and-drop reorder. No "pin this post to position 1" option. No way to say "on this page, show Post A first, Post B second, and let the rest sort by date."

And the workarounds all have problems:

### Sticky Posts
WordPress sticky posts pin a post to the top — but it's global. Pin something on the homepage and it shows up pinned on your blog archive, your category pages, and everywhere else that post type appears.

### Menu Order
You can sort by menu order and assign numeric values to each post. But menu order is global too — if you set Post A to position 1, it's position 1 everywhere. You can't have Post A first on the homepage and Post C first on your services page.

### Changing Publish Dates
Some people backdate or future-date posts to force a specific order. This is fragile, breaks your sitemap, and falls apart every time you add a new post.

### Custom PHP Filters
Developers can write `pre_get_posts` filters to override the query for specific pages. This works but it's code-level, not accessible to editors, and has to be maintained as the site evolves.

### Abandoning Query Loop
Some people give up on dynamic queries entirely and hard-code posts into the layout. This gives full control over order but means every content change requires editing the page structure.

## The Missing Feature: Per-Block Manual Ordering

What most people actually need is:

- A way to **pin specific posts to the top** of a Query Loop block
- **Drag-and-drop reordering** within the block editor
- **Independent ordering per block, per page** — the homepage shows different featured posts than the blog page, even for the same post type
- Works with **any post type** — posts, products, portfolios, testimonials, team members
- **No global side effects** — reordering on one page doesn't affect any other page

This is what **Query Loop Order** does.

---

## Query Loop Order — Manual Post Ordering for Query Loop Blocks

**[Query Loop Order](https://wpqueryloopmanualorder.adamhusar.com/)** is a WordPress plugin that adds drag-and-drop manual ordering to every Query Loop block in the editor.

### How It Works

1. Select any Query Loop block (core or Advanced Query Loop)
2. Click "Reorder Posts" in the sidebar panel
3. A modal opens showing all posts matching the query
4. Pin posts to the top and drag them into order
5. Save — the editor preview updates immediately

The order is stored **per block**. Your homepage Query Loop can have a completely different manual order than your blog page, your shop page, or your landing page — even if they all query the same post type.

### Key Details

- **Per-block, per-page ordering** — each Query Loop block stores its own manual order independently
- **Two-zone interface** — pin specific posts to a manual zone at the top, the rest flow in their natural sort order below
- **Any post type** — posts, pages, WooCommerce products, portfolios, testimonials, team members, any CPT
- **Works with Advanced Query Loop** — hooks into the same query filter, compatible out of the box
- **Self-healing** — deleted or filtered-out posts are automatically removed from the manual order
- **Zero lock-in** — no custom blocks, no database tables. Deactivate the plugin and your blocks revert to default sort order. Reactivate and your manual order is still saved
- **No frontend JavaScript** — the plugin only loads assets in the block editor. Zero performance impact on the frontend
- **Live editor preview** — what you see in the editor is what your visitors see

### Common Use Cases

- **Portfolio sites** — feature your best case studies first, different projects on different service pages
- **WooCommerce stores** — curate which products appear first on homepage vs. shop vs. landing pages
- **Testimonials** — show the enterprise client quote on the homepage, the ROI quote on the pricing page
- **Real estate** — feature premium listings on the homepage, different properties on neighborhood pages
- **Team pages** — display partners before associates, different team leads on different department pages

### Pricing

Lifetime license. Pay once, use forever. All plans include every feature — you only choose how many sites to activate.

| Plan | Sites | Price |
|------|-------|-------|
| Starter | 1 | $19.99 |
| Developer | 10 | $49.99 |
| Agency | 50 | $99.99 |

**[Get Query Loop Order →](https://wpqueryloopmanualorder.adamhusar.com/)**

---

## Links

- **Website & purchase:** [wpqueryloopmanualorder.adamhusar.com](https://wpqueryloopmanualorder.adamhusar.com/)
- **Use case — Portfolio ordering:** [Creative agencies & portfolios](https://wpqueryloopmanualorder.adamhusar.com/use-cases/portfolio-case-studies.html)
- **Use case — WooCommerce products:** [WooCommerce product showcases](https://wpqueryloopmanualorder.adamhusar.com/use-cases/woocommerce-product-order.html)
- **Use case — Testimonials:** [Testimonials & social proof](https://wpqueryloopmanualorder.adamhusar.com/use-cases/testimonials-reviews.html)
- **Use case — Real estate:** [Property listings](https://wpqueryloopmanualorder.adamhusar.com/use-cases/real-estate-listings.html)
- **Use case — Team pages:** [Team & staff directory](https://wpqueryloopmanualorder.adamhusar.com/use-cases/team-staff-directory.html)
