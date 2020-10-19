_Staticast_ is a podcast website [template](https://github.com/Cecilapp/staticast#readme), powered by [Cecil](https://cecil.app) and can be deployed in few seconds with [Netlify](https://app.netlify.com/start/deploy?repository=https://github.com/Cecilapp/staticast&stack=cms).
<!-- break -->
## Installation

### Manually

_Staticast_ is a theme for Cecil, so you need to download and run Cecil to build your website, then you can publish it where you want.

1. Be sure PHP is available
2. [Download _Staticast_](https://github.com/Cecilapp/staticast/archive/master.zip) and install theme with `composer install`
3. [Download `cecil.phar`](https://github.com/Cecilapp/Cecil/releases/latest/download/cecil.phar) and move it to the root of _Staticast_

### Automatically

Use the button to get your own copy of the repository.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Cecilapp/staticast&stack=cms)

This will setup everything needed for running your website, with a CMS:

- A new repository in your GitHub account
- Continuous Deployment to Netlify's CDN
- Control users and access with Netlify Identity
- Manage content with Netlify CMS

## Usage

### Create a new episode

1. Add the MP3 file in `static` directory
2. Create a new Markdown file in `content/episodes`

Example (`episode-1.md`):

```yaml
---
title: "Episode #1"
episode:
  file: /episode-1.mp3
---
Description of the episode.
```

### Preview locally

1. Run `php cecil.phar serve`
2. Open `http://localhost:8080`

### Publish

1. Run `php cecil.phar build`
2. Copy `_site` folder to your web server

### Configuration

See the [`config.yml`](https://github.com/Cecilapp/staticast/blob/master/config.yml) file and more precisely the `podcast` section.
