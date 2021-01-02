My WP Theme Boilerplate
===

Based on [`Automattic/_s`](https://github.com/Automattic/_s).

Installation
---------------

### Requirements

`My WP Theme Boilerplate` requires the following dependencies:

- [Node.js](https://nodejs.org/)
- [Composer](https://getcomposer.org/)

### Quick Start

Clone or download this repository, change its name to something else (like, say, `megatherium-is-awesome`), and then you'll need to do a six-step find and replace on the name in all the templates. **Make sure to perform a case-sensitive search!**

1. Search for `'my_wp_theme_boilerplate'` (inside single quotations) to capture the text domain and replace with: `'megatherium-is-awesome'`.
2. Search for `my_wp_theme_boilerplate_` to capture all the functions names and replace with: `megatherium_is_awesome_`.
3. Search for `Text Domain: my_wp_theme_boilerplate` in `style.css`, `style-rtl.css` and `style.scss` and replace with: `Text Domain: megatherium-is-awesome`.
4. Search for <code>&nbsp;My_WP_Theme_Boilerplate</code> (with a space before it) to capture DocBlocks and replace with: <code>&nbsp;Megatherium_is_Awesome</code>.
5. Search for `my-wp-theme-boilerplate-` to capture prefixed handles and replace with: `megatherium-is-awesome-`.
6. Search for `MY_WP_THEME_BOILERPLATE_` (in uppercase) to capture constants and replace with: `MEGATHERIUM_IS_AWESOME_`.

Then, update the stylesheet header in `style.css`, the links in `footer.php` with your own information and rename `_s.pot` from `languages` folder to use the theme's slug. Next, update or delete this readme.

