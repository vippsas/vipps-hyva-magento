# Changelog
All notable changes to this project will be documented in this file.

The format is based on Keep a Changelog and this project adheres to Semantic Versioning.

## [1.1.0] - 2026-11-06
### Added
- Express opens Vipps/MobilePay in a modal on the store page rather than redirecting, the Hyvä side of
  the Vipps Widget SDK.

### Fixed
- The Express cart restore works on Hyvä.
- Closing, cancelling or approving in the Express widget ends in the shopper's own session, as in Luma:
  the cart comes back with the cancellation message, or the order confirmation is shown. A payment the
  shopper already approved for that cart is respected, so the widget goes to the order or to the cart
  instead of starting a second one.
- The Express button works on configurable products with the Widget SDK turned off.

### Changed
- Requires vipps/module-payment 3.1.0 or later.

## [1.0.0] - 2026-08-24
### Added
- Initial compatibility with vipps/module-payment >= 3.0.1
