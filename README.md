# DNS Allowlists

A collection of domain allowlists for DNS filtering systems, organized by category.

## Overview

This repository contains curated lists of legitimate domains that should be allowed through DNS filtering systems like Pi-hole, AdGuard Home, or NextDNS. These lists help prevent false positives where legitimate functionality gets blocked by overly aggressive DNS blocklists.

## Lists

### Unsubscribe Links

**Path:** `unsubscribe-links/domains.txt`

Contains domains used for legitimate email unsubscribe functionality. Blocking these domains can prevent users from being able to unsubscribe from mailing lists.

> [!WARNING]
> This list may allow some tracking links in emails, as marketing emails tend to use the same domain for all links in the email body.

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

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.