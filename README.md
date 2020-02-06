# ytest

## What is this???

This a dummy repository to test a Huksy / Yarnhook configuration before I make a pull request to a larger project. The goal is to have `yarn install` run automatically every time somebody does a merge.

## What do I do?

Note: this test will require you to have Yarn and Node installed on your machine.

1. Fork this repo and then clone it onto your machine. Then, `cd` into the project you've cloned and run `yarn install` \(hopefully just this once!\).

2. Add my repo as an upstream:

```
git remote add upstream https://github.com/DanielJWagener/ytest.git
```

3. Let me know when you've got everything ready! I'll then change the upstream package.json to include lodash. I'll also push an index.js file that console logs lodash.

4. When I've given you the word that I've added lodash, run these commands:

```
git fetch --all
git pull upstream
git merge upstream/master
```

5. If all goes well, lodash will be installed in your local project without you having to manually run `yarn install`. You can test to make sure everything is working by running `node index.js` in the terminal.

Godspeed!
