# Mobile Shopee

A PHP online store for mobile phones. The home page loads products from MySQL, and each product has its own page.

## Pages

- `index.php` shows the home page: banners, top sale, special price, new phones, and a blog section
- `product.php?item_id=` shows one product (name, brand, price, and image)
- `cart.php` shows the shopping cart layout

Top sale and the other product sections read from the `product` table.

## Tech Stack

- PHP
- MySQL (`mysqli`)
- Bootstrap 4
- Owl Carousel
- Font Awesome

## Requirements

- PHP with the `mysqli` extension
- MySQL
- A local server such as Apache, or PHP's built-in server

## Database

Connection settings are in `database/DBController.php`:

| Setting | Value |
| --- | --- |
| Host | `localhost` |
| User | `root` |
| Password | empty |
| Database | `shopee` |

Create the database and a `product` table with at least these columns:

- `item_id`
- `item_name`
- `item_brand`
- `item_price`
- `item_image`

`item_image` should be a path such as `./assets/products/1.png`.

## Run

From the project folder:

```bash
php -S localhost:8000
```

Then open `http://localhost:8000`.
