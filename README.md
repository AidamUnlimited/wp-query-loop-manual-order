# WordPress Query Loop Block — Sorting Options & Manual Ordering

The Query Loop block sorts by date, title, or (with Advanced Query Loop) menu order, random, modified date, and comment count.

**What's missing:** there's no way to manually pick which posts appear first. No drag-and-drop. No "pin this post to position 1." No per-page control.

The common workarounds — sticky posts (global), menu order (global), faking publish dates (fragile), custom PHP filters (code-level) — all have the same problem: they apply the same order everywhere. You can't show Post A first on the homepage and Post C first on the services page.

---

## Query Loop Manual Order — Manual Post Ordering for Query Loop Blocks

**[Query Loop Manual Order](https://wpqueryloopmanualorder.adamhusar.com/)** is a WordPress plugin that adds drag-and-drop manual ordering to every Query Loop block in the editor.

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


**[Get Query Loop Manual Order →](https://wpqueryloopmanualorder.adamhusar.com/)**

---
