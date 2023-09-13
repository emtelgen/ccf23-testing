## Website for the MSU Computing CloudFellowship

Website: https://msu-icer.github.io/cloudcomputingfellowship/

This is the source code for the building the website and materials for the 2023-2024 MSU Cloud Computing Fellowship, used by the fellowship organizers.   Students do not need to use this source code, simply visit the site above.  

See the home page of the site for information about the Cloud Computing Fellowship, or contact https://icer.msu.edu
 

### Building

The site was build with the amazing python package "MkDocs" and Markdown.   For details and full documentation visit [mkdocs.org](https://www.mkdocs.org).  The theme is the also amazing https://github.com/squidfunk/mkdocs-material

Mkdocs has a 'gh-deploy' command that uses the "gh pages branch" method (rather than the new github workflows method).   Hence this github project uses a branch for github pages

For MSU colleagues, to collaborate on this website, install as follows: 

```sh
git clone git@github.com:MSU-ICER/cloudcomputingfellowship.git

cd cloudcomputingfellowship.git
# create a python environment, if you like
pip install -r requirements.txt
mkdocs serve  # build and preview the site
# edit markdown files in /docs folder per mkdocs docs
git add docs
git commit -m "updated CCF website"
git push origin main
mkdocs gh-deploy 
```

---

Licensed as Creative Commons Attribution-NonCommercial 4.0 International License

![Creative Commons License](https://i.creativecommons.org/l/by-nc/4.0/88x31.png)

http://creativecommons.org/licenses/by-nc/4.0/
