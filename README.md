# adal-angular4 
[![Build status](https://ci.appveyor.com/api/projects/status/iwpwhyp6ymifxc4e?svg=true)](https://ci.appveyor.com/project/benbaran/adal-angular4)
[![npm version](https://badge.fury.io/js/adal-angular4.svg)](https://badge.fury.io/js/adal-angular4)


___

Angular 4+ Adal wrapper package. Can be used to authenticate Angular applications against Azure Active Directory v1 endpoint.
___

## Change Log

### 4.0.9

- Upgraded to Gulp version 4. Build options are now:

```
gulp watch    - watch for file changes do the build task
gulp build    - clean the dist directory and build the project
gulp commit   - bump version and add and commit files to git (for maintainers only)
gulp publish  - publish new npm version (for maintainers only)
```
### 4.0.1

- Updated to support latest version of adal-angular. Major version updated because of potentially breaking changes.

### 3.0.7

- Added an automatic login token refresh feature. It will refresh tokens at application load if there is a valid sign-in token. It will also refresh the login token 5 minutes before it expires.

### 3.0.1

- Updated to Angular 6, cleaned up files. THIS IS A BREAKING VERSION!

### 2.0.0

- Updated to Angular 5, cleaned up files. THIS IS A BREAKING VERSION!

### 1.1.11

- Fixed a bug where the valid scenario of refreshing an id_token is not handled - thanks to @alan-g-chen.

### 1.1.4

- Hash is now removed from url after login

### 1.0.1

- Added HTTP Interceptor for Angular 4.3.0+
- Updated all packages to newest versions

### Update and Build Instructions

```
git clone https://github.com/benbaran/adal-angular4.git

npm install -g @angular/cli@latest gulp@latest

del .\package-lock.json

ng update --all --force

npm install typescript@3.1.1

gulp build
```

### NPM Publish Instructions (For Maintainers Only)
```
git clone https://github.com/benbaran/adal-angular4.git

npm install -g @angular/cli@latest gulp@latest

del .\package-lock.json

ng update --all --force

npm install typescript@3.1.1

gulp publish
```

