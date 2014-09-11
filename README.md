## HTCAT Buildpack

Get the Super fast binary GET library htcat (https://github.com/htcat/htcat) into your Heroku app

## Use

Set up multibuildpack https://github.com/ddollar/heroku-buildpack-multi.

add this buildpack to your `.buildpacks` file.

```
$ echo 'https://github.com/schneems/htcat_buildpack' >> .buildpacks
```

Then whatever buildpack you normally use (like heroku ruby)

```
$ echo 'https://github.com/heroku/heroku-buildpack-ruby' >> .buildpacks
```


Then deploy

## Verify

Use

```
$ heroku run bash
```

Then in the shell, run

```
$ htcat --version
```

## License

MIT