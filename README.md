# WPU disable posts

This plugin will disable all posts and default post taxonomies : category & post_tag.
Posts will be deleted if some are found.

Filter list :
---

```php
/* Re-Enable default taxonomies */
add_filter('wpudisableposts__disable__taxonomies', '__return_false');

/* Avoid destroying terms from default taxonomies */
add_filter('wpudisableposts__destroy_terms', '__return_false');

/* Avoid destroying old posts */
add_filter('wpudisableposts__destroy_posts', '__return_false');
```

