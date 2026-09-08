# Technical SEO Specification

## Title

- unique per indexable page;
- clear primary intent;
- avoid stuffing.

## Meta Description

- useful and unique when practical;
- do not fabricate claims.

## Canonical

- canonical points to intended preferred production URL;
- avoid staging/dev canonical.
- pre-adoption templates may use placeholder/example origins, but final production readiness must not.

## H1

- one clear player-facing H1.

## Breadcrumbs

Recommended for nested content.

## Structured Data

Potential:

- `WebSite`
- `Article`
- `BreadcrumbList`
- `VideoGame` where appropriate
- FAQ only when visible FAQ exists and current policy supports it

Schema must match visible content.

## Sitemap

Include canonical indexable pages.

Final production sitemap URLs must use the intended production origin.

Exclude:

- noindex;
- private;
- thin placeholders;
- internal search results;
- duplicates.

## Robots

Do not accidentally block production pages or required assets.

Final production `robots.txt` must reference the sitemap on the intended production origin.

## Indexability

Every page intentionally:

- indexable;
- noindex;
- not public.

## URLs

- lowercase;
- stable;
- hyphen-separated;
- avoid unnecessary parameters/dates.

## Duplicate Prevention

Check:

- trailing slash;
- www/non-www;
- HTTP/HTTPS;
- uppercase;
- duplicate parameters;
- duplicate intent.

## Production Canonical / Domain Preflight

Before final production readiness:

- canonical URLs use the intended production origin;
- sitemap URLs use the intended production origin;
- `robots.txt` sitemap reference uses the intended production origin;
- no placeholder/example domain remains;
- no `vercel.app` canonical remains when a custom domain is the intended production URL;
- apex/www choice is explicit and consistent;
- redirects are consistent with the chosen canonical host;
- provider/deployment target alone is not proof of public launch;
- live production behavior is inspected.

Starter core must not guess the domain. The project/Human must provide the intended production origin and apex/www decision.

## Internal Linking

Use descriptive anchors.

Important Hubs should link to and receive links from relevant children.

## Images / Media SEO

Images:

- meaningful alt when appropriate;
- correct dimensions;
- stable aspect-ratio behavior to reduce layout shift;
- optimized file size;
- valid local/remote asset path;
- deliberate eager/lazy loading intent;
- avoid huge raw screenshots.

Video:

- embed responsively;
- include useful visible context;
- provide intentional visible fallback when iframe/player loading may fail or be blocked and blank output would look broken;
- use poster/preload behavior intentionally;
- warn on unusually large local video files based on observed behavior;
- do not add video schema unless it matches visible content and implementation.

Do not add a universal byte threshold, CDN abstraction, transcoding service, or generic performance framework unless a real project separately proves the need.

## v2.6 Coverage Note

Technical SEO correctness does not compensate for missing major content families, inaccessible navigation, unrecognizable first viewport, failed game recognition, unresolved high-priority media, stale screenshot evidence, semantically mismatched media, broken third-party failure states, or text-only player UX. Those are separate release gates in `QA_CHECKLIST.md`.
