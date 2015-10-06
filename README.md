# bashsaurus
Simple API driven Thesaurus in Bash.

```bash
$ bashsaurus simple
elementary
$ bashsaurus simple
uncomplicated
$ bashsaurus simple
unproblematic
```

Rather than presenting you with a full list of words, the script gives you a new synonym for a given word each time you run it. This continues until all the available synonyms have been depleted, at which point the list cycles again.

The script is designed to be used with a text editor plugin, which would allow you to cycle over synonyms for the word the cursor is currently above.

## Install
```bash
git clone git@github.com:danprince/bashsaurus.git
cd bashsaurus
./bashsaurus

# optionally put it on your PATH
sudo ln -s $PWD/bashsaurus /usr/bin/bashsaurus
```

## Usage
1. Get a free API key from [Big Huge Thesaurus][1].
2. Store the API key against a `BASHSAURUS_API_KEY` environment variable.

```bash
export BASHSAURUS_API_KEY=your_api_key_here

# test it works
echo $BASHSAURUS_API_KEY
your_api_key_here
```

[1]: https://words.bighugelabs.com/api.php
