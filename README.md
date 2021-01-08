My WP Theme Boilerplate
===

Based on [`Automattic/_s`](https://github.com/Automattic/_s).

Installation
---------------

### Requirements

`My WP Theme Boilerplate` requires the following dependencies:

- [Node.js](https://nodejs.org/)
- [Composer](https://getcomposer.org/)

### Getting Started

#### 1. Customize _s Files

Clone or download this repository, change its name to something else (like, say, `megatherium-is-awesome`), and then you'll need to do a six-step find and replace on the name in all the templates. **Make sure to perform a case-sensitive search!**

1. Search for `'my-wp-theme-boilerplate'` (inside single quotations) to capture the text domain and replace with: `'megatherium-is-awesome'`.
2. Search for `my_wp_theme_boilerplate_` to capture all the functions names and replace with: `megatherium_is_awesome_`.
3. Search for `Text Domain: my_wp_theme_boilerplate` in `style.css`, `style-rtl.css` and `style.scss` and replace with: `Text Domain: megatherium-is-awesome`.
4. Search for <code>&nbsp;My_WP_Theme_Boilerplate</code> (with a space before it) to capture DocBlocks and replace with: <code>&nbsp;Megatherium_is_Awesome</code>.
5. Search for `my-wp-theme-boilerplate-` to capture prefixed handles and replace with: `megatherium-is-awesome-`.
6. Search for `MY_WP_THEME_BOILERPLATE_` (in uppercase) to capture constants and replace with: `MEGATHERIUM_IS_AWESOME_`.

Then, update the stylesheet header in `style.css`, the links in `footer.php` with your own information and rename `_s.pot` from `languages` folder to use the theme's slug. Next, update or delete this readme.

#### 2. Editing the Project Variables

Configure the project paths and other variables inside the `wpgulp.config.js` file. This is a compulsory step.

#### 3. Install dependencies

Open your project (WordPress theme) folder and run the installation.

```sh
npm install
```

#### 4. Start your project

Once the installation is done, you can run the start script within your project (WordPress theme) folder.

```sh
npm start

# To stop press CTRL (⌃) + C
```


#### 5. More Scripts/Tasks (optional step) 

To optimize images and generate WP POT translation file, or generate a RTL stylesheet you can run the following commands

```sh
# To optimize images.
npm run images

# To generate WP POT translation file.
npm run translate

# To generate RTL stylesheets and Sourcemap.
npm run styles-rtl

# To generate theme/plugin zip file without extranious files.
npm run zip
```


