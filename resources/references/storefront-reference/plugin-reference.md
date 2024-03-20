---
nav:
  title: Storefront plugins
  position: 20

---

# Storefront plugins and helper

This is a list of available javascript plugins and helpers that can be used and extended.

## Plugins

| Plugin                                 | Description                                                                                                                                                                                       | Notes                            |
|:---------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------|
| `AccountGuestAbortButtonPlugin`        | Used on the logout button to fire a `guest-logout` event after logging out from a guest session.                                                                                                  | ---                              |
| `AddToCartPlugin`                      | Submits the form that adds a product to the cart and opens the OffCanvasCart. E.g., used on product buy buttons.                                                                                   | ---                              |
| `AddToWishlistPlugin`                  | Adds or removes a product from the wishlist and toggles the indicator (heart icon) that displays if the current product is on the wishlist. Also updates the wishlist counter in the main header. | ---                              |
| `AddressEditorPlugin`                  | Opens a modal to edit the billing or shipping address.                                                                                                                                            | ---                              |
| `AjaxModalPlugin`                      | This class extends the Bootstrap modal functionality by adding an event listener to modal triggers that contain a special "data-url" attribute which is needed to load the modal content by AJAX. | ---                              |
| `BaseSliderPlugin`                     | Provides basic slider functionality to a container with sliding elements. Uses the "tiny-slider" framework in the background.                                                                     | ---                              |
| `BaseWishlistStoragePlugin`            | Provides basic storage logic to add, remove and get products from the wishlist. Used by the local storage wishlist (if user is guest) and the persisted wishlist (if used is logged in).            | ---                              |
| `BasicCaptchaPlugin`                   | Provides the JS functionality for the basic captcha that can be activated in storefront sales channel. Only works with a corresponding form.                                                    | ---                              |
| `BuyBoxPlugin`                         | Refreshes the buy box area on the product detail page after switching to a different product variant. Re-initializes the tax info modal.                                                          | ---                              |
| `CartWidgetPlugin`                     | Controls the cart widget in the main header that displays the total cart amount. Updates automatically if a product is added to the cart.                                                         | ---                              |
| `ClearInputPlugin`                     | Adds clear functionality to input fields.                                                                                                                                                         | ---                              |
| `CmsGdprVideoElement`                  | Shows a consent overlay before rendering an external CMS video element, e.g. from YouTube. Only when the user provides consent, the actual video will be loaded.                                           | ---                              |
| `CollapseCheckoutConfirmMethodsPlugin` | Displays a "show more" button when too many shipping or payment methods are shown. Used on the checkout page.                                                                                     | ---                              |
| `CollapseFooterColumnsPlugin`          | Enables collapsing containers (accordion) on mobile viewports for the columns in the page footer.                                                                                                 | ---                              |
| `CookieConfiguration`                  | Controls the detailed cookie configuration (displayed in an OffCanvas). Displays the available cookies with checkboxes and saves the selected user preference.                                    | ---                              |
| `CookiePermissionPlugin`               | Controls the cookie banner at the bottom of the page when no cookie preference is set. Can either save a preference directly via button or open the cookie configuration OffCanvas.               | ---                              |
| `CountryStateSelectPlugin`             | Renders an additional select box with country states (e.g. "North-Rhine-Westphalia") if a country was selected. E.g., used in the registration form.                                               | ---                              |
| `CrossSellingPlugin`                   | Used to re-initialize the product sliders when toggling between different cross-selling tabs that contain product sliders.                                                                        | ---                              |
| `DateFormat`                           | This plugin formats a date and converts it to the local timezone if the data attribute date-format is set.                                                                                        | ---                              |
| `DatePickerPlugin`                     | Controls the date picker component. Shows a datepicker UI when applied to an input field.                                                                                                         | ---                              |
| `EllipsisPlugin`                       | Used to expand or shrink a text.                                                                                                                                                                  | Deprecated and removed in v6.6.0 |
| `FadingPlugin`                         | Collapses or expands a Bootstrap collapse container with additional "more" or "less" links.                                                                                                       | Deprecated and removed in v6.6.0 |
| `FilterBasePlugin`                     | Provides basic functionality for a product listing filter. Communicates with the `ListingPlugin`. Other filters like "multi select" extend from this plugin class.                                | ---                              |
| `FlyoutMenuPlugin`                     | This Plugin handles the subcategory display of the main navigation.                                                                                                                               | ---                              |
| `FormAddHistoryPlugin`                 | Provides an API to push items into the browser history after a form was submitted. Only works on a `<form>` element.                                                                              | ---                              |
| `FormAjaxSubmitPlugin`                 | This plugin submits a form with ajax without reloading the page, instead of performing a regular form submit.                                                                                     | ---                              |
| `FormAutoSubmitPlugin`                 | This plugin automatically submits a form, when the element or the form itself has changed.                                                                                                        | ---                              |
| `FormCmsHandler`                       | Sends forms from the CMS (e.g. contact form) via ajax and renders additional error/success messages.                                                                                              | ---                              |
| `FormFieldTogglePlugin`                | Provides functionality to display or hide additional form fields without reloading the page. E.g., used in the registration form when shipping and billing addresses are different.                  | ---                              |
| `FormPreserverPlugin`                  | This plugin preserves a form, if the element or the form itself has changed. After a reload of the page the form is filled up with the stored values.                                             | ---                              |
| `FormScrollToInvalidFieldPlugin`       | This plugin scrolls to invalid form fields when the form is submitted.                                                                                                                            | ---                              |
| `FormSubmitLoaderPlugin`               | This plugin shows a loading indicator on the form submit button when the form is submitted.                                                                                                       | ---                              |
| `FormValidation`                       | This plugin validates fields of a form. Also styles the field elements with the bootstrap style if enabled.                                                                                       | ---                              |
| `GoogleAnalyticsPlugin`                | Adds all events for Google Analytics and configures the `gtag`. Only used when "Analytics" is activated in the sales channel.                                                                     | ---                              |
| `GoogleReCaptchaBasePlugin`            | Provides basic functionality to apply a Google reCAPTCHA to a `<form>` element. The JS-plugins for reCAPTCHA v2 and v3 extend this plugin.                                                        | ---                              |
| `GuestWishlistPagePlugin`              | Used on the `/wishlist` page/route to display the products currently on the wishlist. Displays wishlist items from local storage if the user is a guest.                                          | ---                              |
| `ImageZoomPlugin`                      | Enables functionality to zoom into an image, e.g. using the mouse wheel. Used inside the image zoom modal on the product detail page. Works together with `ZoomModalPlugin`.                      | ---                              |
| `ListingPlugin`                        | Provides the filter functionality of the product listing. Gets the current values of each filter, current sorting and pagination. Generates the requests and displays the new results.            | ---                              |
| `MagnifierPlugin`                      | Handles the magnifier lens functionality on the detail page.                                                                                                                                      | ---                              |
| `OffCanvasAccountMenu`                 | Opens the account dropdown menu ("user avatar" icon in header) inside an OffCanvas on mobile viewports.                                                                                           | ---                              |
| `OffCanvasCartPlugin`                  | Opens the shopping cart in an OffCanvas. Used on the shopping cart display in the main header.                                                                                                    | ---                              |
| `OffCanvasFilter`                      | Opens the listing filters inside an OffCanvas when the mobile "Filter" button is clicked. Only used on mobile viewports.                                                                          | ---                              |
| `OffCanvasTabs`                        | Used on mobile viewports to open or show contents in an OffCanvas that are shown in Bootstrap tabs on larger desktop viewports. E.g., used on the product detail page to open the reviews on mobile.  | ---                              |
| `OffcanvasMenuPlugin`                  | Displays the main category navigation inside an OffCanvas on mobile viewports. Triggered by the mobile "hamburger" menu icon.                                                                     | ---                              |
| `QuantitySelectorPlugin`               | Enables functionality to select a product's quantity. Controls the increase (+) or decrease (-) buttons. E.g., used on the product detail page or in the checkout.                                  | ---                              |
| `RatingSystemPlugin`                   | Controls the rating stars when the user is writing a product review and lets the user select a star rating between 1 and 5.                                                                       | ---                              |
| `RemoteClickPlugin`                    | This plugin is used to remotely click on another element.                                                                                                                                         | ---                              |
| `ScrollUpPlugin`                       | Displays a small button with an "arrow up" icon to scroll back to the top of the page. Used on all pages and only displayed when the user has scrolled down the page.                             | ---                              |
| `SearchWidgetPlugin`                   | Renders a dropdown with search result suggestions underneath the main headers search input field, as soon as the user starts to type a search term.                                               | ---                              |
| `SetBrowserClassPlugin`                | Adds CSS classes to the `<body>` element depending on the current device, e.g. `is-ipad`. These classes can be used to add styling for a specific device category.                                 | ---                              |
| `VariantSwitchPlugin`                  | This plugin submits the variant form with the correct data option. Used on the product detail page to switch between product variants.                                                            | ---                              |
| `WishlistWidgetPlugin`                 | Shows how many items are currently on the wishlist. Used by the wishlist "heart" icon inside the main header.                                                                                     | ---                              |
| `ZoomModalPlugin`                      | Opens a full-screen modal window with an image gallery. Can contain multiple images that the user can zoom into. Used on the product detail page.                                                 | ---                              |

## Helpers

| Helper                  | Description                                                                                    | Notes |
|:------------------------|:-----------------------------------------------------------------------------------------------|:------|
| `ArrowNavigationHelper` | Helper to navigate between different items using the arrow keys. Used by `SearchWidgetPlugin`  | ---   |
| `CookieStorageHelper`   | Provides a nicer API to add or remove cookies.                                                 | ---   |
| `DateFormatHelper`      | Wrapper helper to format a date string or object using `Intl.DateTimeFormat`                   | ---   |
| `Debouncer`             | Wait for a defined amount of time. Basically a wrapper around `setTimeout`.                    | ---   |
| `DeviceDetection`       | Returns information about the current device, e.g. if it is a touch device.                    | ---   |
| `DomAccess`             | Helper function to access DOM elements in a unified way and improved error handling.           | ---   |
| `ElementReplaceHelper`  | Helper to replace a desired DOM element with another DOM element.                              | ---   |
| `FeatureSingleton`      | Offers an API to check if specific feature flags are currently activated.                      | ---   |
| `Iterator`              | Helper function to iterate over different data types in a unified way (array, objects etc.)    | ---   |
| `MemoryStorage`         | This class is mainly a fallback if the session, local or cookie storage fails.                 | ---   |
| `NativeEventEmitter`    | Event Emitter which works with the provided DOM element. The class isn't meant to be extended. | ---   |
| `StorageSingleton`      | Wrapper API that can use local, session or cookie storage in the background.                   | ---   |
| `StringHelper`          | Provides different string formatters, e.g. converting into "UpperCamelCase"                    | ---   |
| `ViewportDetection`     | Returns the currently active Bootstrap viewport, e.g. `LG` or `XL`                             | ---   |