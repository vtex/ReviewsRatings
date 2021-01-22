📢 Use this project, [contribute](https://github.com/vtex-apps/reviews-and-ratings) to it or open issues to help evolve it using [Store Discussion](https://github.com/vtex-apps/store-discussion).

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->

[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)

<!-- ALL-CONTRIBUTORS-BADGE:END -->

# Reviews and Ratings

Reviews & Ratings is a VTEX IO native solution that allows shoppers to submit reviews and ratings for products, as well as see them while navigating the store..

![reviews-and-ratings-app](https://user-images.githubusercontent.com/52087100/71026526-31e7d580-20e8-11ea-93d8-094c1e8af7cd.png)

## Configuration

### Step 1 - Installing the Reviews and Ratings app

Using your terminal, log in to the desired VTEX account and run the following command:

`vtex install vtex.reviews-and-ratings@2.x`

### Step 2 - Defining the app settings

1. In the account's admin dashboard, access `Apps > My Apps` and then click on the box for `Reviews and Ratings`:

![apps-reviews-and-ratings](https://user-images.githubusercontent.com/52087100/71026670-77a49e00-20e8-11ea-9e01-0cb4dec12a56.png)
_When using the admin v3_

![apps-reviews-and-ratings](https://user-images.githubusercontent.com/26655596/99747634-b772c300-2ab9-11eb-927b-cd03e89421af.png)
_When using the admin v4_

2. Once in the app's settings page, define the following settings according to the desired scenario:

![reviews-settings](https://user-images.githubusercontent.com/43498488/97418081-0e4d0880-1911-11eb-9b80-47b92bbdef93.jpg)

- **Allow Anonymous Reviews** - If unchecked, only logged-in shoppers will be able to review products.

- **Require Admin Approval** - Checking this box activates the review moderation system. Newly submitted reviews will not be displayed on the store website until an administrator approves them in the account's admin. For more details on this, access the Modus Operandi section below.

- **Ask For Reviewer's Location** - Checking this box activates an optional review field. Shoppers that submit reviews will be asked to fill in their current location (i.e. "Boston, MA").

- **Default all review accordions to open** - The app displays reviews on the product page inside collapsible accordions. Checking this box will cause _all_ review accordions to default to open when the page is loaded, with review text limited to 3 lines. Reviews with more than 3 lines of text will be truncated with an ellipsis and a `Show More` link that can be used to display the whole review text.

- **Number of open review accordions** - Checking this box allows you to set a specific number of review accordions (instead of all of them) to automatically open when the page is loaded, displaying all the review text. If the `Default all review accordions to open` setting is active, this option is ignored.

- **Display graph** - Checking this box allows you to display the reviews graph on the product details page.

- **Display stars in `product-rating-summary` if there are no reviews** - Checking this box allows you to display empty stars even if the product still has no reviews.

- **Display total reviews number on `product-rating-summary` block** - Checking this box allows you to display the total number of reviews for a product.

- **Display `Add review` button on `product-rating-summary` block** - Checking this box allows you to display an `Add review` button under the stars.

- **Display stars in `product-rating-summary` if there are no reviews** - Checking this box allows you to display empty stars even if the product still has no reviews.

- **Display total reviews number on `product-rating-summary` block** - Checking this box allows you to display the total number of reviews for a product.

- **Display `Add review` button on `product-rating-summary` block** - Checking this box allows you to display an `Add review` button under the stars.

### Step 3 - Declaring the app's blocks in your store theme

Once the app is configured, it is time to place the following blocks in your Store Theme app:

- `product-reviews` - This block can be added to the product page template (`store.product`). It renders a paginated list of reviews for the product being viewed, as well as a form for the shopper to add a new review.

- `product-rating-summary` - This block can be added to the product page template (`store.product`) and renders the average rating for the product being viewed as well as the number of reviews that have been submitted. If moderation is being used by the account, only approved reviews will count toward these figures.

- `product-rating-inline`: Similar to the previous block (`product-rating-summary`), but intended to be used in [product shelves](https://vtex.io/docs/components/all/vtex.shelf/). The block displays the product's average rating only.

## Modus Operandi

As described above, the app may be configured to use a **review moderation interface** where an administrator is responsible for approving the reviews before they are displayed on the store website.

To access and use the review moderation admin interface, follow the instructions below:

1. Enable the **Require Admin Approval** setting as described above.
2. In the admin dashboard, navigate to **Catalog > Reviews** using the admin's sidebar.
3. You may view either **Pending** or **Approved** reviews using the tabs at the top of the page.

Individual pending reviews may be either approved or deleted using the Kebab Menu (3 dots button) in the right column or selecting the checkbox in the left. Multiple reviews can also be selected using the checkboxes, being approved or deleted in bulk.

Approved reviews may be deleted as well, either individually or in bulk.

## Customization

In order to apply CSS customizations in this and other blocks, follow the instructions given in the recipe on [Using CSS Handles for store customization](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization).

| CSS Handles               |
| ------------------------- |
| `container`               |
| `formContainer`           |
| `graphBar`                |
| `graphBarContainer`       |
| `graphBarPercent`         |
| `graphContent`            |
| `graphContainer`          |
| `graphText`               |
| `graphTextLabel`          |
| `loginLink`               |
| `reviewComment`           |
| `reviewCommentRating`     |
| `reviewCommentsContainer` |
| `reviewCommentUser`       |
| `reviewNameUser`          |
| `reviewText`              |
| `reviewsHeading`          |
| `reviewsRating`           |
| `reviewsRatingAverage`    |
| `reviewsRatingCount`      |
| `star--empty`             |
| `star--filled`            |
| `star`                    |
| `starpicker`              |
| `stars`                   |
| `starsContainer`          |
| `summaryContainer`        |
| `summaryButtonContainer`  |
| `writeReviewContainer`    |
| `graphContent`            |
| `graphContainer`          |
| `graphText`               |
| `graphTextLabel`          |
| `graphBarContainer`       |
| `graphBar`                |
| `graphBarPercent`         |
| `summaryButtonContainer`  |
| `writeReviewContainer`    |

<!-- DOCS-IGNORE:start -->

## Contributors ✨

Thanks goes to these wonderful people:

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/khrizzcristian"><img src="https://avatars1.githubusercontent.com/u/43498488?v=4" width="100px;" alt=""/><br /><sub><b>khrizzcristian</b></sub></a><br /><a href="https://github.com/vtex-apps/reviews-and-ratings/commits?author=khrizzcristian" title="Code">💻</a></td>
    <td align="center"><a href="https://juliomoreira.pro"><img src="https://avatars2.githubusercontent.com/u/1207017?v=4" width="100px;" alt=""/><br /><sub><b>Julio Moreira</b></sub></a><br /><a href="https://github.com/vtex-apps/reviews-and-ratings/commits?author=juliomoreira" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

<!-- DOCS-IGNORE:end -->
