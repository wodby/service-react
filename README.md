# React service for Wodby

Run statically built React applications on Nginx with [Wodby](https://wodby.com).

This service inherits the Nginx runtime and specializes its application build contract with the [React boilerplate](https://github.com/wodby/react-boilerplate). It is intended for use through the [React stack](https://github.com/wodby/stack-react) or from a custom Wodby stack.

## Manifest design

- Base service: `nginx` `2.0.0`, compatible with `^2.0.0`
- Runtime, endpoint, scaling, and Helm configuration: inherited from Nginx
- Build source connection: enabled
- Starter: React boilerplate

Validate the manifest with:

```sh
wodby service validate-manifest service.yml --org <org-id>
```

See the [service manifest reference](https://wodby.com/docs/2.0/services/template/) and [managed services index](https://github.com/wodby/services).
