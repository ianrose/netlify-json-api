# netlify-rest-api

Build a RESTful JSON API on Netlify.

`go get github.com/poga/netlify-rest-api`

## Usage

First, prepare a CSV file named `users.csv`:

```csv
id,name,age
1,John,12
2,Marry,22
3,Jeff,18
4,Kate,30
5,Jerry,19
6,Alan,54
7,Sandy,49
```

Run `netlify-rest-api`:

```
netlify-rest-api users.csv http://YOUR-netlify-domain out/
```

Deploy `out/` to netlify.

Now you have a RESTful JSON API such as: `GET http://YOUR-netlify-domain/users.json`, `GET http://YOUR-netlify-domain/users.json?page=1` and `GET http://YOUR-netlify-domain/users/1.json`


## Todos:

- [ ] programmically deploy to netlify
- [ ] `POST`, `PUT`, and `DELETE` with proxy

## License

The MIT License
