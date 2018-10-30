# codeceptjs-axios

codeceptjs-http is [CodeceptJS](https://codecept.io/) helper which wraps [axios](https://github.com/axios/axios) library to
perform requests. It's alternative helper that provides more flexible request management.

### Configuration

This helper should be configured in codecept.json/codecept.conf.js

-   `baseURL`: base HTTP url.

Example:

```json
{
   "helpers": {
     "AXIOS" : {
       "require": "codeceptjs-axios",
       "baseURL": "http://localhost:8080"
     }
   }
}
```

## sendGetRequest

Send HTTP request, response will be availible as return value.

```js
I.sendGetRequest('/api/users.json');
```

**Parameters**

-   `url` - endpoint path. Can be relative or absolute
-   `headers` - (optional) to include token in the headers for example

## sendPostRequest

Send HTTP request, response will be availible as return value.

```js
I.sendPostRequest('/api/users.json', { "email": "user@user.com" });
```

**Parameters**

-   `url` - endpoint path. Can be relative or absolute
-   `payload` - the request body to send
-   `headers` - (optional) to include token in the headers for example

## sendPatchRequest

Send HTTP request, response will be availible as return value.

```js
I.sendPatchRequest('/api/users.json', { "email": "user@user.com" });
```

**Parameters**

-   `url` - endpoint path. Can be relative or absolute
-   `payload` - the request body to send
-   `headers` - (optional) to include token in the headers for example

## sendPutRequest

Send HTTP request, response will be availible as return value.

```js
I.sendPutRequest('/api/users.json', { "email": "user@user.com" });
```

**Parameters**

-   `url` - endpoint path. Can be relative or absolute
-   `payload` - the request body to send
-   `headers` - (optional) to include token in the headers for example

## sendDeleteRequest

Send HTTP request, response will be availible as return value.

```js
I.sendDeleteRequest('/api/users/1');
```

**Parameters**

-   `url` - endpoint path. Can be relative or absolute
-   `headers` - (optional) to include token in the headers for example