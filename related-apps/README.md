# Related Apps Catalog

`v1/catalog.json` is the shared catalog used by the apps' related-app screens.

Apps select a group by `groups[].id`, then show published entries other than their own `bundleIdentifier`, ordered by `sortOrder`.

To add another product family, append another object to `groups`. To add an app without exposing it before release, set `isPublished` to `false` and change it after the App Store page becomes public.

Keep `appStoreId` as a string because StoreKit's app overlay accepts the App Store identifier as text. All URLs must use HTTPS.
