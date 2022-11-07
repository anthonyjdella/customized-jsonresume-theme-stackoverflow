# Customized JSON Resume Theme: Stack Overflow

🖼️ This is a tweaked version of the [Stack Overflow theme](https://github.com/phoinixi/jsonresume-theme-stackoverflow). Tweaked to fit my design preferences. Published on NPM and GitHub Registry.

## Notable Changes

* 2 Page version in PDF/printable mode 
* Added sections for speaking and articles
* Style changes

## Prerequisites

To build and start the local server, it needs to use the cli command, which is custom cli I tweaked.

`npm i @anthonyjdella/customized-resume-cli`

## How to Start

`npm run start`

## How to Change

* `resume.hbs` is the order of the resume.
* `theme/partials/` are the html files for each section
* `style.css` is the styling
* To make changes to the PDF/printable version, make changes in the `@print` section of `style.css`
* Change version number in `package.json`
* Deploy the changes via `npm publish --access public`
* To see changes from `resume.anthonydellavecchia.com` you need to go to the [registry project](https://github.com/anthonyjdella/customized-registry-functions), then cd into `functions`, run `npm i` and `npm update`, then `firebase deploy`.

<details>
  <summary>Click to expand README.md of the source repository!</summary>

# Stack Overflow theme for jsonresume [![npm version](https://badge.fury.io/js/jsonresume-theme-stackoverflow.svg)](http://badge.fury.io/js/jsonresume-theme-stackoverflow)

**Printable version with custom CSS**

[DEMO](https://themes.jsonresume.org/theme/stackoverflow)

## Getting started

### Install the command line

Create your resume in json on [jsonresume](https://jsonresume.org)

The official [resume-cli](https://github.com/jsonresume/resume-cli) to run the development server.

Go ahead and install it:

```
npm install -g resume-cli
```

### Install and serve theme

Clone the repository

```
git clone https://github.com/francescoes/jsonresume-theme-stackoverflow.git
```

And simply run:

```
resume serve
```

You should now see this message:

```
Preview: http://localhost:4000
Press ctrl-c to stop
```

To build your own resume, create a 'resume.json' file in the current folder and follow the [json resume schema](https://jsonresume.org/schema/)

### Social Profiles Icons

**Profiles supported with brand colors:**

github, stack overflow, linkedin, dribbble, twitter, facebook, pinterest, instagram, soundcloud, wordpress, youtube, flickr, google plus, tumblr, foursquare.

To have a social icon close the social link profile (or username) it is enough to set a `network` the name of the Social Network (es: 'Stack Overflow').

#### Support to extra fields

With stackoverflow theme it is possible to add:

- `keywords` to each 'work', 'publication' and 'volunteer' item
- `summary` to each 'interests' and 'education' item
- `location` to each 'work', 'education' and 'volunteer' item
- `birth` to 'basics'

example of the extra `location` object: 

```
"location": {
  "city": "Zürich",
  "countryCode": "CH",
  "region": "Switzerland"
} 
```
example of the extra `birth` object:

```
"birth": {
  "place": "New York",
  "state": "USA",
  "date": "1988"
}
```

## Contribution

Fork the project, add your feature (or fix your bug) and open a pull request OR

[Open an issue](https://github.com/francescoes/jsonresume-theme-stackoverflow/issues/new) if you find find or if you would like to have extra fields or changes 

## License

Available under the [MIT license](http://opensource.org/licenses/mit-license.php).
