# Documentation

## Development

Install packages

```
npm install
```

Add gitmojis:

```
npm i -g gitmoji-cli
gitmoji -c
```

Update contributors:

```
npm run contributors
# make commit
```

Deploy

```
# on master branch
npm run build

git switch gh-pages
cp dist/* .

# make commit and push
```

