android_sdk_repository(
    name = "androidsdk",
    path = "/Users/jingwen/sdk",
)

android_ndk_repository(
    name = "androidndk",
    path = "/Users/jingwen/ndks/r17b",
)

# Google Maven Repository
GMAVEN_TAG = "20180625-1"

http_archive(
    name = "gmaven_rules",
    strip_prefix = "gmaven_rules-%s" % GMAVEN_TAG,
    url = "https://github.com/bazelbuild/gmaven_rules/archive/%s.tar.gz" % GMAVEN_TAG,
)

load("@gmaven_rules//:gmaven.bzl", "gmaven_rules")

gmaven_rules()
