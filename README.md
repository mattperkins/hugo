# run dev server / drafts
## hugo server -D

# start new hugo project
## hugo new site [project name]

# add content
## hugo new page.md
## hugo new dir1/page2.md

# overwrite auto generated list pages
## hugo new dir1/_index.md

# create list page for sub-sub directories
## hugo new dir2/dir3/_index.md

# archetypes
## create a new file in archetypes folder called posts.md
## populate with desired custom front-matter meta data. 
## $hugo new posts/[page-name] creates new page in posts dir with custom archetypes

# add theme
## hugo new theme [name]

# add prebuilt theme
## git clone theme into themes folder
## add theme = "theme-name" to config.toml

