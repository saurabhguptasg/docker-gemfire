#
# GemFire 8 Locator Dockerfile
#
# https://github.com/dockerfile/java
# https://github.com/dockerfile/java/tree/master/oracle-java8
#

# Pull base gemfire image.
FROM pivotal/gemfire-base

ENV SERVER_NAME $(date +NAME%Y%m%H%M%S)

EXPOSE 40404
#ENTRYPOINT java -cp $GEMFIRE/lib/server-dependencies.jar com.gemstone.gemfire.distributed.ServerLauncher start $SERVER_NAME --server-port=40404 --locator=$LOCATOR_HOST[$LOCATOR_PORT]
#ENTRYPOINT gfsh start server --name=$(date +NAME%Y%m%H%M%S) --server-port=40404 --locators=$LOCATOR_HOST[$LOCATOR_PORT]
ENTRYPOINT gfsh


