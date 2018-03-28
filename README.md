<p align="center">
  <img src='https://github.com/eugrdn/screenshots/blob/master/sk-title.png' />
</p>

## Stack

Both of the apps are written on TS 2.7.2

### Native
- react-native
- react-apollo + other...
- react-native-router-flux

### Service
- express
- pg
- sequelize
- apollo-server-express
- jsonwebtoken (auth)

## Updating models

API is fully typized. To update typings for the models on the client from the service, there should be used a 
```bash
npm run gql-gen
```
command that will generate types through the graphql API (`./common/typings/types.d.ts` will be generated automatically). This command will check graphql schemas, so it requires running service.
