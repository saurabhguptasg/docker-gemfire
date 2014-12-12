#
# GemFire 8 Locator Dockerfile
#
# https://github.com/dockerfile/java
# https://github.com/dockerfile/java/tree/master/oracle-java8
#

# Pull base gemfire image.
FROM pivotal/gemfire-base

EXPOSE 10335
ENTRYPOINT java -cp $GEMFIRE/lib/locator-dependencies.jar com.gemstone.gemfire.distributed.LocatorLauncher start locator1 10335

