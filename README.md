# Ktor on Google App Engine flexible environment

This is a hello world Ktor app to get started on Google App Engine flexible environment with Kotlin + Gradle.

The secret sauce for me was ensuring `appengine` gradle plugin used the `app.yaml` file instead of the
`appengine-web.xml` file that I brought over from the setup with the standard GAE environment:
```groovy
apply plugin: 'com.google.cloud.tools.appengine-appyaml'    // force plugin to use app.yaml
```

This repository may be bloated with unnecessary code, and be poorly organised, I simply got it to work and stopped 🙃.