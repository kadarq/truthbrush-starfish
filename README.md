# truthbrush
Truthbrush is an API client for Truth Social. Truthbrush is built and maintained by the [Stanford Internet Observatory](https://io.stanford.edu). 

Currently, this tool can: 

* Search for users, statuses, or hashtags
* Pull a user's followers
* Pull users a given user follows 
* Pull a user's statuses
* Pull the list of "People to Follow" or suggested users
* Pull all "trending" hashtags
* Pull all "trending" Truth posts
* Pull all ads
* Pull a user's metadata

Truthbrush is designed for academic research, open source intelligence gathering, and data archival. It pulls all of the data from the publicly accessible API.



## Installation

Truthbrush is not yet available on PyPI. To install it, clone the repository and run `pip install .`. Provided your `pip` is setup correctly, this will make `truthbrush` available both as a command and as a Python package. **Note that Truthbrush requires Python 3.8 or higher.**

After installation, you will need to set your Truth Social username and password as environmental variables. 

`EXPORT TRUTHSOCIAL_USERNAME=foo`
`EXPORT TRUTHSOCIAL_PASSWORD=bar`

## CLI Usage

```text
Usage: truthsocial [OPTIONS] COMMAND [ARGS]...

Options:
  --help     Show this message and exit.


Commands:
  followers    Pull a user's followers.
  following    Pull users a given user follows.
  search       Search for users, statuses or hashtags.
  statuses     Pull a user's statuses
  suggestions  Pull the list of suggested users.
  tags         Pull trendy tags.
  trends       Pull trendy Truths.
  ads          Pull ads.
  user         Pull a user's metadata.
``````

**Pull all a user's followers**

```bash
truthbrush followers HANDLE
```

**Pull all users a given user followers**

```bash
truthbrush following HANDLE
```

**Search for users, statuses, or hashtags**

```bash
truthbrush search
```


**Pull all statuses (posts) from a user**

```bash
truthbrush statuses HANDLE
```

**Pull all "People to Follow" (suggested) users**

```bash
truthbrush suggestions
```
**Pull all trendy tags**

```bash
truthbrush tags
```
**Pull all ads**

```bash
truthbrush ads
```

**Pull all of a user's metadata**

```bash
truthbrush user HANDLE
```

## Contributing

Contributions are encouraged! For small bug fixes and minor improvements, feel free to just open a PR. For larger changes, please open an issue first so that other contributors can discuss your plan, avoid duplicated work, and ensure it aligns with the goals of the project. Be sure to also follow the [code of conduct](CODE_OF_CONDUCT.md). Thanks!

## Wishlist

Support for the following capabilities is planned:

- ...nothing right now! (Got an idea? Submit an issue/PR!)
