# Template for AWS Amplify

Template for AWS Amplify with [devcontainer-for-aws](https://github.com/mats16/devcontainer-for-aws).

## How to use

### 1. Create a repo using this template

### 2. Configure AWS SSO and login

```bash
aws configure sso --profile default

aws sso login
```

#### Configure `credential_process`

If tools does not support AWS SSO, you need to configure `credential_process`.

```sh
aws configure set credential_process aws-sso-credential-process --profile default
```

### 3. Create new AWS CDK app

```bash
npx projen new awscdk-app-ts
````
