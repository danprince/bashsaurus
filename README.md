# bashsaurus
Simple cycling Thesaurus in Bash.

```bash
$ bashsaurus simple
elementary
$ bashsaurus simple
uncomplicated
$ bashsaurus simple
unproblematic
```

Rather than presenting you with a full list of words, the script gives you a new synonym for a given word each time you run it. This continues until all the available synonyms have been depleted, at which point the list cycles again. It is designed to be used with a text editor plugin, which would allow you to cycle over synonyms for the word the cursor is currently above.

The synonyms are scraped from [www.thesaurus.com](http://www.thesaurus.com/).

## Install
```bash
git clone git@github.com:danprince/bashsaurus.git
cd bashsaurus
./bashsaurus

# optionally put it on your PATH
sudo ln -s $PWD/bashsaurus /usr/bin/bashsaurus
```

## Usage
```bash
$ bashsaurus fun
enjoyable
$ bashsaurus fun
pleasant
$ bashsaurus fun
entertaining
```

