# Keycloak SAML Identity Provider RelayState Propagator

In Keycloak, there is currently no way to pass through a RelayState in the IdP-initiated SSO scenario, that means from the initiating IdP to Keycloak to the target application. This IdP mapper puts IdP RelayState into a user sesion note, which, when used in combination with User Session Note client mapper, makes it possible to propagate RelayState to the final SAML assertion or OIDC tokens.

