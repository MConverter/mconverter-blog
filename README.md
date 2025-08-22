# Articles, images, and additional metadata for the [MConverter Blog](https://mconverter.eu/blog/)

## Directory structure and front matter

### [`articles`](articles)

This folder contains all blog articles.

File name: matches the URL slug, without the `.md` extension.
 - Example: `my_article.md` -> `https://mconverter.eu/blog/my_article/`

#### Front matter
| Key | Example Value | Required | Description | Notes |
|-----|---------------|----------|-------------|-------|
| `title` | `Welcome to the MConverter Blog!` | ✅ | Article title | Used for `<h1>` on the article page and on the grid of articles |
| `meta_title` | `Welcome to our blog!` | ❌ | Alternative title | Used for SEO meta `<title>` and social media `og:title` tags. If not provided, the `title` is used. |
| `description` | `In this post, we explain what you can expect to see here.` | ✅ | Article description | Used on the article page (full text) and on the grid of articles (truncated to 3 lines) |
| `meta_description` | `Find out what you can expect to see here.` | ❌ | Alternative description | Used for SEO `<meta name="description">` and social media `og:description` tags. If not provided, the `description` is used. |
| `image` | `easy_convert_files.webp` | ✅ | The file name of the main featured image | Must correspond to a file in the [`images`](images) directory, in a subdirectory with the same name as the article. The image should be in WebP format preferably. |
| `image_alt` | `Easily convert files online` | ✅ | Alt text for accessibility | The `alt` attribute of the main `<img>` tag |
| `date_added` | `2022-03-06` | ✅ | When the article was first published | Format: `YYYY-MM-DD` |
| `date_updated` | `2022-03-06` | ✅ | When the article was last modified | Format: `YYYY-MM-DD`. If the article hasn't been updated yet, the same value as `date_added` should be used. |
| `author` | `martin_minchev` | ❌ | Author identifier for the article | The identifier must match a file name in the [`authors`](authors) directory, without the `.md` extension. |
| `categories` | `["video_conversion", "tips_and_tricks"]` | ❌ | Array of category tags for organization | Used for filtering in the grid of articles. The identifier must match a file name in the [`categories`](categories) directory, without the `.md` extension. The categories on the article page are displayed in the order they are listed here. |
| `aside_cards` | `["50_percent_discount_pro", "mobile_app"]` | ✅ | Array of sidebar card identifiers | Used to display promotional content in the sidebar. The identifier must match a file name in the [`aside_cards`](aside_cards) directory, without the `.md` extension. The cards are displayed in the order they are listed here. |

#### Markdown content

The headings should start from `##`, which corresponds to the `<h2>` tag. Subheadings are `###`, etc.

All headings and subheadings become part of the article's table of contents.

When adding images to the article text, the file name must match a file located in the [`images`](images) directory, in a subdirectory with the same name as the article (i.e., where the featured image is located). The image should be in WebP format preferably.

If something cannot be achieved with Markdown only, you can use HTML as an alternative for that part of the article.

### [`aside_cards`](aside_cards)

This folder contains all sidebar cards.

#### Front matter
| Key | Example Value | Required | Description | Notes |
|-----|---------------|----------|-------------|-------|
| `heading` | `Enjoy a 50% Discount` | ✅ | Heading for the card | Used for the `<h2>` tag on the article page |

#### Markdown content

Use HTML for the CTA button. Clicking it automatically sends a GA4/Matomo event: `aside_click`, with the sidebar card's file name identifier as the event label/name.

### [`authors`](authors)

This folder contains all authors.

#### Front matter
| Key | Example Value | Required | Description | Notes |
|-----|---------------|----------|-------------|-------|
| `name` | `Martin Minchev` | ✅ | Author name | Used for the author's name on the article page |
| `job_title` | `Co-Founder & CTO` | ✅ | Author job title | Used for the author's job title on the article page, displayed below the name |
| `image_url` | `https://example.com/Martin.jpg` | ❌ | Author image URL | Must be a full absolute URL. If not provided, [this placeholder icon](https://mconverter.eu/img/avatar.webp) is displayed instead. |

### [`categories`](categories)

This folder contains all categories.

File name: matches the URL slug, without the `.md` extension.
 - Example: `my_cat.md` -> `https://mconverter.eu/blog/category/my_cat/`

#### Front matter

| Key | Example Value | Required | Description | Notes |
|-----|---------------|----------|-------------|-------|
| `heading` | `Image Conversion` | ✅ | Category heading | Used for the `<h1>` tag on the category page, the SEO `<title>` and social media `og:title` tags |

#### Markdown content

The category description is displayed on the category page, in the SEO `<meta name="description">` and social media `og:description` tags. For the SEO and social media tags, all formatting is removed.

### [`images`](images)

This folder contains the images to be used in articles.

The names of subdirectories correspond to the article file names, without the `.md` extension.

## Common questions

To hide an article or category page (e.g. while it's still work in progress), make it a hidden file: `.my_article.md`.

All Markdown links are do-follow by default. To include a nofollow link, add it as regular HTML instead: `<a href="https://example.com" target="_blank" rel="nofollow noopener">link</a>`

Allowed characters for the file names of articles, categories, etc.: lowercase Latin letters, numbers, and underscores `_`.
