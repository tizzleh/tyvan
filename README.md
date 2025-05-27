# TyVan Conversions Website

This repository contains a simple static website to advertise a van conversion business. The site was created using plain HTML and CSS with remote placeholder images.

## Structure

- `site/index.html` - Home page with an overview and services section.
- `site/about.html` - About page describing the business.
- `site/contact.html` - Contact information and a simple contact form.
- `site/style.css` - Shared styling for the pages.

All images use `https://via.placeholder.com` so they can easily be replaced with real photos.

## Preview

You can view the site locally by opening any of the HTML files in your browser.

## Contact Form

The contact page includes a simple form that sends an email using the visitor's
email client. Update the `mailto:` address in `site/contact.html` to your own
to start receiving inquiries. For more advanced handling, you could connect the
form to an AWS Lambda function or another backend service.

## Hosting on AWS

To host this site on AWS you can use an S3 bucket configured for static website hosting:

1. Create a new S3 bucket and enable static website hosting.
2. Upload the contents of the `site/` folder to the bucket.
3. Set the index document to `index.html`.
4. Make the bucket public or use CloudFront as needed.

Once uploaded, you'll have a static site accessible from the bucket's endpoint or through a custom domain.


