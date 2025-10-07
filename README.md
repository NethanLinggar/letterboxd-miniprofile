# letterboxd-miniprofile

A tool for displaying Letterboxd profiles in an embeddable iframe.

Inspired by [steam-miniprofile](https://github.com/gamer2810/steam-miniprofile) by gamer2810.

## How To Use

Load the following URL in an iframe:

```
https://nethanlinggar.github.io/letterboxd-miniprofile/?user=LETTERBOXD_USERNAME
```

### Parameters

- `user` - Your Letterboxd username (required)
- `favorites` - Set to `true` to display Top 4 films (optional)
- `unclickable` - Set to `true` to disable clicking (optional)

### Example

```html
<iframe
  src="https://nethanlinggar.github.io/letterboxd-miniprofile/?user=smeggy&favorites=true&unclickable=true"
  className="w-[332px] h-[280px]"
  allow="encrypted-media"
  allowFullScreen
  title="Letterboxd Embed"
/>
```
<img width="332" height="280" alt="nethanlinggar_github_io__letterboxd-miniprofile_-modified" src="https://github.com/user-attachments/assets/8aefd83d-c724-4736-853f-c218fe3280e4" />

## How It Works

The HTML file is hosted on GitHub Pages and receives data from a CORS server deployed on Vercel. Since Letterboxd has no public API, the server uses a Python web scraper to fetch profile data. The HTML then parses and displays the data accordingly.

## About

This is a personal tool of mine created to embed my Letterboxd profile on [my website](https://nethans-website.vercel.app/). It's intentionally minimal, but it gets the job done.
