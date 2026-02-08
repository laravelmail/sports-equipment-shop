# Sports Equipment Shop

Professional marketing email template for Sports Equipment Shop promoting new products or special offers.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Retail, Sports & Fitness
- **Message Type:** Marketing
- **Tags:** promotion, sale, discount, special offer

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/sports-equipment-shop.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/sports-equipment-shop/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.sports-equipment-shop',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
