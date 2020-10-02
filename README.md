## 🎨 gatsby-wordpress-blog

## Originally Created from Gatsby-WordPress-Theme-Phoenix

A Gatsby site using WordPress as a headless CMS.
Front end wiring in Gatsby/React.
Backend Content in WordPress.

## 🔥 Features

1. Uses React with Gatsby ( Blazing Fast )
2. PWA ( Works Offline )
3. Image Optimization ( blur effect )
4. ACF - Advanced Custom Fields ( from WP )
5. GraphQL ( in Gatsby and with wp-graphql on WordPress )
6. Blog Page with Pagination
7. Offline Search Feature
8. Categories, Archive Page, Custom Home Page
9. Custom Widgets, Menus

## 🚀 Set Up

### Gatsby Setup

- Rename [`env-example`] (e.g. .../site/env-example) to [`.env`] and add your WordPress SITE_URL in `site` directory :
  `SITE_URL=https://example.com`
- Make sure there aren't any trailing /'s in the URL

### WordPress Setup

1. Upload and activate all the plugins from wordpress/plugins folder of this repo, into your WordPress Site.

OR,

a. Clone the WordPress plugin [Headless CMS](https://github.com/imranhsayed/headless-cms) in your WordPress
plugin directory and activate it.

b. Clone and activate [wp-graphql](https://github.com/wp-graphql/wp-graphql) -test on ( v0.8.3 ) in WordPress plugin directory.
c. Clone and activate [wp-graphiql](https://github.com/wp-graphql/wp-graphiql) in WordPress plugin directory.
d. Clone and activate [wp-graphql-acf](https://github.com/wp-graphql/wp-graphql-acf) in WordPress plugin directory.
e. Install and activate [ACF WordPress plugin](https://wordpress.org/plugins/advanced-custom-fields/) in the WordPress.

2. - Set Header menu as `HCMS Header Menu`

   ![](demos/header-menu-demo.png)

   - Set Footer menu as `HCMS Footer Menu`
     ![](demos/footer-menu-demo.png)

3. You can also set text widgets in #HCMS Footer #1 and #HCMS Footer #2 under Appearance > Widgets in WordPress.
4. Import all the ACF data from `wordpress/acf-data` json file of this repo, into WordPress by going to WordPress Dashboard > Custom Fields > Tools > Import
5. Create a Home Page ( if there isn't one already )and make sure you have a home page and Location rule is set to Home page.
   ![](demos/acf-home-screenshot.png)
6. Add the ACF required data on the Home page from WordPress Dashboard from acf.
7. If not already done, set your site title, description and logo from WordPress customizer.
8. Make sure on the Home page that under Settings that the Permalink..URL Slug is set to home

**Open the source code and start editing however you'd like for add'l changes**
**To see your site in action type the following**

`npm run dev`

Your site is now running at `http://localhost:8000`!

_Note: You'll also see a second link: _`http://localhost:8000/___graphql`_. This is a tool you can use to experiment with querying your data. Learn more about using this tool in the [Gatsby tutorial](https://www.gatsbyjs.org/tutorial/part-five/#introducing-graphiql)._

## 🚀 Development

- Navigate into site’s directory.

```shell
yarn install      # Run this for the first time.
npm run dev      # During development.
npm run build    # When ready for production.
```

### Theme on npm

[gatsby-wordpress-theme-phoenix](https://www.npmjs.com/package/gatsby-wordpress-theme-phoenix)
