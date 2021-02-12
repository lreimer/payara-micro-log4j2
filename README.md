# Payara Micro with Log4J2

A custom Payara Micro variant using Log4J2 (async) as logging implementation.

## Building and Running

```bash
$ ./gradlew clean ass

$ cd build/libs/
$ java -Dlog4j2.contextSelector=org.apache.logging.log4j.core.async.AsyncLoggerContextSelector -Dlog4j.configurationFile=log4j2.xml -jar payara-micro-log4j2-5.2021.1.jar --logproperties logging.properties --nocluster
```


## Maintainer

M.-Leander Reimer (@lreimer), <mario-leander.reimer@qaware.de>

## License

This software is provided under the MIT open source license, read the `LICENSE`
file for details.