package(
    default_testonly = 1,
    default_visibility = ["//visibility:public"],
)

licenses(["notice"])  # Apache 2.0


java_library(
    name = "testing",
    srcs = glob(
        ["*.java"],
        exclude = [
            "FakeProxyConnectionMetadataProvider.java",
            "FakeQuotaServerClient.java",
        ],
    ),
    resources = [
        "logging.properties",
        "//java/google/registry:env/common/default/WEB-INF/datastore-indexes.xml",
        "//java/google/registry:env/common/default/WEB-INF/queue.xml",
    ] + glob(["*.csv"]),
    deps = [
        "//java/com/google/common/annotations",
        "//java/com/google/common/base",
        "//java/com/google/common/cache",
        "//java/com/google/common/collect",
        "//java/com/google/common/io",
        "//java/com/google/common/net",
        "//java/com/google/common/testing",
        "//java/com/google/common/util/concurrent",
        "//third_party/java/appengine:appengine-api-testonly",
        "//third_party/java/appengine:appengine-integration-testing",
        "//third_party/java/appengine:appengine-stubs",
        "//third_party/java/appengine:appengine-testing",
        "//third_party/java/appengine_gcs_client",
        "//third_party/java/auto:auto_value",
        "//third_party/java/bouncycastle",
        "//third_party/java/bouncycastle_bcpg",
        "//third_party/java/joda_money",
        "//third_party/java/joda_time",
        "//third_party/java/json",
        "//third_party/java/json_simple",
        "//third_party/java/jsr305_annotations",
        "//third_party/java/jsr330_inject",
        "//third_party/java/junit",
        "//third_party/java/mockito",
        "//third_party/java/objectify:objectify-v4_1",
        "//third_party/java/servlet/servlet_api",
        "//third_party/java/truth",
        "//java/google/registry/config",
        "//java/google/registry/dns:constants",
        "//java/google/registry/dns/writer",
        "//java/google/registry/flows",
        "//java/google/registry/model",
        "//java/google/registry/pricing",
        "//java/google/registry/request",
        "//java/google/registry/tmch",
        "//java/google/registry/util",
        "//java/google/registry/xml",
    ],
)

