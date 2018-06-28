# travelogues.github.io

This is the repository for the project website, hosted on [www.travelogues-project.info](www.travelogues-project.info).

## Installation

### Requirements

* [Jekyll](https://jekyllrb.com/), which is available for 
    * [Ubuntu Linux](https://jekyllrb.com/docs/installation/#ubuntu)
    * [MacOS](https://jekyllrb.com/docs/installation/#macOS)
    * [Windows](https://jekyllrb.com/docs/windows/) (not officially supported)

### Installation (local)

1. Download/clone this project.
2. Navigate to the directory and download/install the Ruby gems needed:

       cd travelogues.github.io
       bundle install --path vendor/bundle
       
3. Launch the website locally:

       bundle exec jekyll serve --incremental
       
   The website can be tested at `http://localhost:4000/`.
     
