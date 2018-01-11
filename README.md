# NPM Restore
Utility for restoring/migrating npm packages from version control.

## Usage
Edit `migrate` and list your package repositories under `repos=()`. The script expects one git repo per npm package, with a `package.json` in the root.
For best results, it is recommended to use npm version 5 and above to make use of local cache for package dependencies.

### Configuring your NPM client
Before running the migrate script, you may want to point your client to a private NPM registry and log in with your desired "push" user. Use the npm cli to configure these settings globally. e.g:
```bash
npm config set registry https://npm.mycompany.com
npm login
```
