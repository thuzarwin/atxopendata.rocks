# atxopendata.rocks website

This repo houses the City of Austin Open Data Website - atxopendata.rocks, a public resource website which informs, educates, and encourages the use of the [City of Austin Open Data Portal.](http://data.austintexas.gov)


## Installation

Run each of the following steps to get the site up and running.

1. `git clone https://github.com/cityofaustin/atxopendata.rocks`
2. `cd https://github.com/cityofaustin/atxopendata.rocks`
3. `bundle install`
4. `./serve-blog`

You should be able to see the site at: http://127.0.0.1:4000/site/

## Deployment 

We use Github Pages to host. 

To deploy, for this example, let’s pretend the subfolder containing your site is named `open`

Please follow the steps below to deploy to `gh-pages` from a `open` folder on the master branch. 

**Step 1

Remove the `open` directory from the project’s .gitignore file (it’s ignored by default by Yeoman).

**Step 2

Make sure git knows about your subtree (the subfolder with your site).

`open add rocks && git commit -m "Initial open subtree commit"`

**Step 3

Use subtree push to send it to the gh-pages branch on GitHub.

`git subtree push --prefix open origin gh-pages`

Great! If your folder isn’t called `open`, then you’ll need to change that in each of the commands above.

