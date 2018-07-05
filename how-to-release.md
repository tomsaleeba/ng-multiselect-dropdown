You can release by:
```bash
# bump the version in package.json
git add .
git commit -m "bump version"
git tag -am "new release" v0.x.x
git push && git push --tags
yarn run build:lib
cd dist-lib
npm pack
# move the *.tgz file to *.tar.gz, as GitHub won't accept .tgz
# open https://github.com/tomsaleeba/ng-multiselect-dropdown/releases/tag/<your tag>
# edit the release and attach the *.tar.gz archive
```

You can then use the release in another project by doing:
```
yarn add https://github.com/tomsaleeba/ng-multiselect-dropdown/files/2165232/ng-multiselect-dropdown-0.1.8-tom1.tar.gz
```
