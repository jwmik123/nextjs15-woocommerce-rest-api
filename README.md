# Next.js 15 E-commerce Template with WooCommerce & WordPress

A modern, high-performance e-commerce template built with Next.js 15, integrating WooCommerce REST API, WordPress GraphQL, and Mollie Payments. Perfect for businesses looking to combine the power of WordPress content management with Next.js frontend capabilities.

## Important

Please note that mollie implementation done, you can easily switch it to other payment gateway by changing the code in the `lib/mollie/index.ts` file. f.e. you can use `Stripe` or `Paypal` or `Klarna` or `Bank Transfer` etc.

I will be implementing more payment gateways in the future.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Features

- **Next.js 15**: Utilizing the latest features including App Router, Server Components, and improved image optimization
- **WordPress Integration**: Seamless content management through WordPress GraphQL API
- **WooCommerce REST API**: Full e-commerce capabilities with product management, cart functionality, and order processing
- **Mollie Payments**: Secure payment processing with support for multiple payment methods
- **TypeScript**: Full type safety across the entire application
- **Tailwind CSS**: Modern, responsive design with utility-first CSS
- **Server-Side Rendering**: Optimized for SEO and performance
- **Authentication**: JWT-based authentication with WordPress

## Prerequisites

- Node.js 18.17 or later
- WordPress installation with WooCommerce plugin
- WordPress GraphQL plugin
- Mollie account and API keys

## Getting Started

1. Clone the repository:

```bash
git clone https://github.com/yourusername/nextjs15-woo-wordpress-template
cd nextjs15-woo-wordpress-template
```

2. Install dependencies:

```bash
npm install
```

3. Configure environment variables:

```bash
cp .env.example .env.local
```

Edit `.env.local` with your WordPress, WooCommerce, and Mollie credentials:

```
NEXT_PUBLIC_WORDPRESS_URL=
NEXT_PUBLIC_WORDPRESS_API_URL=
WC_CONSUMER_KEY=
WC_CONSUMER_SECRET=
MOLLIE_API_KEY=
NEXT_PUBLIC_SITE_URL=
```

4. Start the development server:

```bash
npm run dev
```

## Configuration

### WordPress Setup

1. Install required plugins:
   - WooCommerce
   - WPGraphQL
   - WPGraphQL for WooCommerce
2. Enable REST API endpoints
3. Configure CORS headers

### WooCommerce Configuration

1. Generate API keys in WooCommerce settings
2. Configure shipping zones and tax rates
3. Set up product categories and attributes

### Mollie Setup

1. Create a Mollie account
2. Configure webhook URLs
3. Set up preferred payment methods

## Project Structure

```
├── app/
│   ├── api/
│   ├── cart/
│   ├── products/
│   └── checkout/
├── components/
│   ├── cart/
│   ├── products/
│   └── checkout/
├── lib/
│   ├── wordpress/
│   ├── woocommerce/
│   └── mollie/
└── types/
```

## Features in Detail

- **Product Catalog**

  - Dynamic product listing
  - Advanced filtering and search
  - Real-time inventory management

- **Shopping Cart**

  - Persistent cart state
  - Dynamic pricing updates
  - Multiple currency support

- **Checkout Process**

  - Multi-step checkout
  - Address validation
  - Order summary
  - Multiple payment methods through Mollie

- **User Account**
  - Order history
  - Saved addresses
  - Wishlist functionality

## Contributing

Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support, please open an issue in the GitHub repository or contact us at support@yourdomain.com.

## Acknowledgments

- Next.js team for the amazing framework
- WordPress and WooCommerce communities
- Mollie team for their excellent payment solutions
