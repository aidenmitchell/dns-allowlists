# DNS Allowlists

A collection of domain allowlists for DNS filtering systems, organized by category.

## Overview

This repository contains curated lists of legitimate domains that should be allowed through DNS filtering systems like Pi-hole, AdGuard Home, or NextDNS. These lists help prevent false positives where legitimate functionality gets blocked by overly aggressive DNS blocklists.

## Lists

### Unsubscribe Links

**Path:** `unsubscribe-links/domains.txt`

Contains domains used for legitimate email unsubscribe functionality. Blocking these domains can prevent users from being able to unsubscribe from mailing lists, which may violate regulations like CAN-SPAM or GDPR.

Current domains:
- `l.engage.canva.com` - Canva email engagement/unsubscribe links
- `ablink.seller.etsy.com` - Etsy seller notification unsubscribe links
- `subscriptions.pstmrk.it` - Postmark email service unsubscribe management
- `click.zoom.com` - Zoom email link tracking and unsubscribe

## Usage

### Pi-hole

1. Navigate to your Pi-hole admin interface
2. Go to Group Management > Adlists
3. Add the raw GitHub URL for the list you want to use
4. Update Gravity

### AdGuard Home

1. Go to Filters > DNS allowlists
2. Add a custom list using the raw GitHub URL
3. Save and update filters

### NextDNS

1. Go to Privacy > Allowlist
2. Add domains individually or import from the list

## Contributing

If you've found a legitimate domain that should be allowlisted, please:

1. Verify the domain serves a legitimate purpose
2. Open an issue or pull request with:
   - The domain name
   - Which category it belongs to
   - Why it should be allowlisted
   - Example of what breaks when it's blocked

## License

This project is released into the public domain. Use it however you'd like.
