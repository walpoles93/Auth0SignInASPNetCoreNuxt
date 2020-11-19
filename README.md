# Auth0 Sign In with ASP.NET Core & Nuxt

NOTE: For this project to work, you need to set your Auth0 secrets for both the ASP.NET Core project and the Nuxt project

## ASP.NET Core Secrets
- Navigate to project directory and run:
```
dotnet user-secrets set "Authentication:Auth0:Authority" "MyAuthority"
dotnet user-secrets set "Authentication:Auth0:Audience" "MyAudience"
```

## Nuxt Secrets
- Navigate to the root directory of the Nuxt project
- Create a .env file
- Add the following lines (using your own secrets)
```
AUTHENTICATION_AUTH0_DOMAIN=MyDomain
AUTHENTICATION_AUTH0_CLIENT_ID=MyClientId
AUTHENTICATION_AUTH0_AUDIENCE=MyAudience
```