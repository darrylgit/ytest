# ytest

## What is this???

This a dummy repository to test a Huksy / Yarnhook configuration before I make a pull request to a larger project. The goal is to have `yarn install` run automatically every time somebody does a merge.

## What do I do?

1. Fork this repo and then clone it onto your machine. Then, run `yarn install` \(hopefully just this once!\).

2. Let me know when you've cloned and installed everything. I'll then change the upstream package.json to include lodash.

3. When I've given you the word that I've added lodash, run these commands:

```
git fetch --all
git pull upstream
git merge upstream/master
```

4. If all goes well, lodash will be installed in your local project without you having to manually run `yarn install`.

Godspeed!
