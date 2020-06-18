# How to set up to use jekyll to preview website locally on Windows10

Use the same setup as for ARCHER2 Website  
https://github.com/ARCHER2-HPC/archer2-website/blob/master/README_local_jekyll_on_win10_instructions.md
to install bundler and jekyll

Navigate to your github/cirrus-website 

You need bundler version 2.0.2 on your Win10 computer to edit the ARCHER2 website, so we need to tell the CirrusWebsite to accept this version (instead of the very old version it is currently looking for).

Edit the file airspace-jekyll.gemspec using your preferred text editor

Line 16 change the version of bundler

currently reads

     spec.add_development_dependency "bundler", "~> 1.12"

update it to 

     spec.add_development_dependency "bundler", "~> 2.0.1"
  
In the folder github/cirrus-website
 
    bundle install
 
That gets all the dependencies
 
Then run 
 
    bundle exec jekyll serve 
 
and you can view the website at localhost:4000 in your browser

## Important (I think) 

Make sure 
* Gemfile
* airspace-jekyll.gemspec

are not tracked in git (add to your gitignore)
so the above changes do not propagate!


This worked for me but no promises!