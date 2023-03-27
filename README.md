# npm-package-test
Creating a npm package
#

### Steps to create npm package:

1) Create a github repository, run `git init` and run `git remote add <name> <repo-link>` (This way, the npm page will have the link of the repository.)
2) Run `npm init` (The package name is the one that the npm package will have)
3) Run `npm login` (Log in with your npm account)
4) Run `npm publish` (The first time you run this, it will create a package)
#
### Update the code: 
  After updating the code, you need to bump up the `package.json` version field and then run `npm publish`
#
### Notes: 
  - Make sure that you verified your email after creating the account.
  - You can use already created package names if you add use your account username: `@mateopineiroa/<package-name>`. Note that if you do this, by default it makes it a private package. But you can publish it as public using `npm publish --access=public`. Also, this can be made by default if you initialize npm using `npm init --scope=<username>`
#
### Test Package Locally
1) Run `npm link in the package folder (This will expose it to the local node modules folder of the pc).
2) In the project that you want to use the package, run `npm link <package-name>` (This will install the local npm package in the folder)
