# Keycloak Session Restrictor

An event listener for Keycloak, allowing only the last session to survive, if a user logs in on multiple browsers/devices.

## Building

`mvnw package -DskipTests`

## Usage

Compile it, build a JAR file and put it to the proper /deployments directory (standalone or domain, depending on your deployment/environment). Finally, you have to register the listener in the Events > Configuration section of your realm, to actually use it. Otherwise no events will be forwarded to the listener.

See https://www.n-k.de/2020/12/keycloak-session-restrictor.html for more details
