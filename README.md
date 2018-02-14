# atxopendata.rocks website

This repo houses the City of Austin Open Data Website - atxopendata.rocks, a public resource website which informs, educates, and encourages the use of the [City of Austin Open Data Portal.](http://data.austintexas.gov)

### Where to Start? 

## Installation

Run each of the following steps to get the site up and running.

1. `git clone https://github.com/cityofaustin/atxopendata.rocks`
2. `cd https://github.com/cityofaustin/atxopendata.rocks`
3. `bundle install`
4. `./serve-blog`

You should be able to see the site at: http://127.0.0.1:4000/site/

## Enviroments

- **GitHub:** `gh-pages`


## Deployment 
We use Github Pages to host. To deploy a subfoldercontaining the site to GitHub Pages.

For this example, let’s pretend the subfolder containing your site is named `rocks`

**Step 1

Remove the `rocks` directory from the project’s .gitignore file (it’s ignored by default by Yeoman).

**Step 2

Make sure git knows about your subtree (the subfolder with your site).

`git add rocks && git commit -m "Initial rocks subtree commit"`

**Step 3

Use subtree push to send it to the gh-pages branch on GitHub.

`git subtree push --prefix `rocks` origin gh-pages`

Great! If your folder isn’t called `rocks`, then you’ll need to change that in each of the commands above.

