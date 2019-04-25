# Plugin to use Vim as slide presentation software

This plugin creates a `presentation` file type, to create slides in Vim.

## Usage

A presentation file needs a `.pres` extension. Vim will then automatically
detect the filetype, use a dedicated syntax highlight and set a handful of
mappings to have amazing slides.

## Syntax

This filetype offers a few specific syntax elements:

- Comments: for some information not really needed for the presentation, but
still useful to have. Comments are lines starting with `% ` (no leading space,
and at least one space after the `%` sign).

- Title: A title is a line surrounded with `# ` and ` #`:

```
    # this is a title #
```

- Subtitle: A subtitle is a line surrounded with `## ` and ` ##`:

```
    ## this is a subtitle ##
```

- Key point: a Key point starts with a leading `* `

```
    * This is a key point
```

- Link to a `.pres` file: Just write a filename, if it ends with `.pres`, it
will be automatically detected.

- Code section (inline): A string surrounded with `` ` ``:

```
    This line contains `some code`
```

## Mappings

Use `<space><space>` or `<space>s` to go to the next slide.

Use `<space>a` to go to the previous slide.

### Debug mappings

Use `<space>f` to go to the first occurence of a `.pres` file in the current
file. I use it to quickly access filenames, combined with `gf` to make sure the
names are written properly.

## Improvements

Some new syntax elements could be created.

The colorscheme should be changed to be a light one, not dark.

## Example

An example of presentation can be found there:

https://github.com/padawin/vim-slides/tree/master/undotree
