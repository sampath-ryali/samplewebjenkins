# Sample Web Jenkins

This repository is a minimal Maven web application designed to build in Jenkins.

## Local build

Requires Java 17+ and Maven:

```bash
mvn clean package
```

The generated artifact is:

```text
target/samplewebjenkins.war
```

## Jenkins configuration

Use **Pipeline** and select **Pipeline script from SCM**, or configure a Maven build step with:

```text
clean package
```

The repository must be configured as `sampath-ryali/samplewebjenkins`. The console log you provided cloned a different repository, `sampath-ryali/samplejenkinsweb`, so update the Jenkins SCM URL if that was unintended.
