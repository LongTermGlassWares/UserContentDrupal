# Drupal Content Upload and Orders
## Requirements
Platform: Drupal 9 and Commerce plugin

### Modules/Blocks
- The requirements below are based on content upload functionality of sites like the following:
  - https://app.rapiddirect.com
  - https://www.hubs.com/manufacture/
  - https://smartquote.fathommfg.com
  - https://www.xometry.com 

- Accept three types of _content_ upload from users:
  - Link
  - File upload
  - Plain Text

- Save _content_ uploaded to database (type, filename, data; same table). File upload is saved in filesystem.
- Associate _content_ with session (and user if logged in).
- After upload, show _content_ just added in database for user/session.
- Show list of _content_ in database associated with user/session.

### Commerce integration
- Implement Drupal's _Purchaseable Entity_ for each of the above _content_ types.
  - Base the price on length of file, URL, etc (for testing/demonstration).
- Allow user to _Add to Cart_
  - Different commerce item for each _content_ type.
  - Disallow adding the same unique/uploaded _content_ multiple times.
- After checkout completes, associate _content_ with ordered item.

### Multilingual support
- All text presented on the interface should be translatable by Drupal’s localization system.

## Deliverables
- Code for modules/blocks
- Instructions for installation and setup (database, website)

## Notes
 This is not setup and maintenance of a new Drupal site. The deliverables completed should give the functionality provided, and be able to be added to another existing site (by using Drupal's customizability correctly). Visual design expectations are minimal (but not zero).
