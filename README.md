## UAAC BOSH Release


### Create a dev release

```
bosh create-release --name=uaac --force --timestamp-version --tarball=/tmp/uaac-boshrelease.tgz
bosh upload-release /tmp/uaac-boshrelease.tgz
```

### Create a final release

```
VERSION=x.y.z
bosh create-release --name=uaac --version=${VERSION} --final --tarball=/tmp/uaac-boshrelease.tgz
bosh upload-release /tmp/uaac-boshrelease.tgz
```