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

#add taxonomies

## add tags
### tags: ["black", "white"] 
#### on list page : <div>{{ if .Params.tags }}Tags:{{range .Params.tags}}<a href="{{ "/tags/" | relLangURL }}{{ . | urlize }}">{{ . }}</a> {{end}}{{end}}</div>

## add categories
### categories: ["summer", "winter"]
#### on list page : <div>{{ if .Params.categories }}<strong>Categories:</strong> {{range .Params.categories}}<a href="{{ "/categories/" | relLangURL }}{{ . | urlize }}">{{ . }}</a> {{end}}{{end}}</div>

## add custom taxonomies
### check config.toml / list.html

# add theme
## hugo new theme [name]

# add prebuilt theme
## git clone theme into themes folder
## add theme = "theme-name" to config.toml

# shortcodes
### {{< shortRound >}} html text {{< /shortRound >}}
### {{% shortRound %}} use percentage when encapsulating *markdown* {{% /shortRound %}} 

# Build and Deploy Hugo
## $ Hugo 
### Upload public contents to server.
## ** Delete public folder before each new build ** 