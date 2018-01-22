# Shopify

Some code I have put together when editing the empire theme on Shopify

### Table of content

- [Blog Recipe to Cart](#blog-recipe-to-cart)
- [Search Placeholder Random Text](#search-placeholder-random-text)
- [More Cool Shopify Tricks](#more-cool-shopify-tricks)
- [Credits](#credits)

#

## Blog Recipe to Cart

### Add list of items to cart for say aa Recipe
Add a list of items such as in a recipe to the cart from blog page on Shopify.

* Takes you to cart page not checkout page
* Different for each Article
* Can change the quantity of each item (Which you can't do with Permalinks)

[Freakdesign Blog](https://freakdesign.com.au/blogs/news/129660999-how-to-create-a-button-to-let-customers-repeat-their-previous-order) - How to create a button to let customers repeat their previous order

#### How to do this

1. Create a snippet in Shopify with [a relative link](recipe-to-cart.liquid)
2. Add this to your article page code where ever you want it
```
{% include 'recipe-to-cart' %}
```
3. On the article editer you can edit the code and past the following
4. Then add the variant_id, product_id and quantity - [How to fine these values](https://www.youtube.com/watch?v=42_4oP33euk)

### Permalink - Redirect to Checkout Page
[Shopify Support](https://help.shopify.com/themes/customization/cart/use-permalinks-to-preload-cart) - Use permalinks to pre-load the cart

```
http://yourstore.com/cart/#{variant_id}:#{quantity}(,...)
```
```
http://your-store.myshopify.com/cart/70881412:1,70881382:1
```

### Form - Redirect to Cart Page
[Freakdesign Blog](https://freakdesign.com.au/blogs/news/add-multiple-products-to-cart-without-permalinks) - How to add multiple products to a Shopify cart without permalinks

```
http://yourstore.com/cart/add?id[]=#{variant_id}&id[]=#{variant_id}
```
```
http://your-store.myshopify.com/cart/add?id[]=70881412&id[]=70881382
```

## Search Placeholder Random Text

Selects a random array item for search bar placeholder from an array.

```
Try searching for bananas 🍌
Try searching watermelon 🍉
Try searching citrus 🍋
Try searching dairy or eggs 🥚
```

![alt text](https://github.com/pargyrop/shopify/blob/master/Search_Placeholder_Random/searchPlaceholderRandomText.gif)

## More Cool Shopify Tricks


## Credits

* [Pixel Union](https://www.pixelunion.net/themes/empire/) - Website Theme
* [Freak Design](https://freakdesign.com.au/) - Great place to get some sneaky tips
