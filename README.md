# Shopify

Some code I have put together when editing the empire theme on Shopify

### Built With

* [Pixel Union](https://www.pixelunion.net/themes/empire/) - Website Theme
* [Freak Design](https://freakdesign.com.au/) - Great place to get some sneaky tips


## Table of content

- [Blog Recipe to Cart](#blog-recipe-to-cart)
- [Search Placeholder Random Text](#search-placeholder-random-text)
- [Cool Things](#cool-things)


## Blog Recipe to Cart

Add a list of items such as in a recipe to the cart from blog page on Shopify.

* Takes you to cart page not checkout page
* Different for each Blog
* Can change the quantity of each item (Which you can't do with Permalinks)

### Redirect to Checkout Page
* [Shopify Support](https://help.shopify.com/themes/customization/cart/use-permalinks-to-preload-cart) - Use permalinks to pre-load the cart

```
http://yourstore.com/cart/#{variant_id}:#{quantity}(,...)
```
```
http://your-store.myshopify.com/cart/70881412:1,70881382:1
```

### Redirect to Cart Page
* [Freakdesign Blog](https://freakdesign.com.au/blogs/news/add-multiple-products-to-cart-without-permalinks) - How to add multiple products to a Shopify cart without permalinks

```
http://yourstore.com/cart/add?id[]=#{variant_id}&id[]=#{variant_id}

```
```
http://your-store.myshopify.com/cart/add?id[]=70881412&id[]=70881382
```

## Search Placeholder Random Text

Selects a random array item for search bar placeholder from an array.

![alt text](https://github.com/pargyrop/shopify/blob/master/Search_Placeholder_Random/searchPlaceholderRandomText.gif)

## Cool Things
