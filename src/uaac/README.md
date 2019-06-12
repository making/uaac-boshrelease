```
bundle install --path vendor/bundle
tar czf uaac-vendor.tgz vendor
bosh --dir=../.. add-blob uaac-vendor.tgz uaac/uaac-vendor.tgz
```