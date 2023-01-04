# railstotrails
[Rails to Trails Conservancy](https://www.railstotrails.org/) (RTC) based in Wahsington D.C. has conducted weekly analyses of national trail usage based on data gathered from 31 trail counters distributed across the country.

Original visualisation challenge on [MakeoverMonday](https://www.makeovermonday.co.uk/). See the [discussion](https://www.makeovermonday.co.uk/week-1-2021/) of the various submissions in 2021.
Corresponding [article on bbc](https://www.bbc.com/future/bespoke/made-on-earth/the-great-bicycle-boom-of-2020.html)

Jessica R built a capsone project on it [in Tableau](https://public.tableau.com/app/profile/jessica.pf/viz/CapstoneProject_16276628699320/Story1?publish=yes) and described it in an [article on medium](https://medium.com/@jessica.rpf/data-visualization-capstone-project-by-jessica-r-3c0155ce9f55)

## Dataset
Download from [data.world](https://data.world/makeovermonday/2021w1) into the folder data

Original [data source on RTC-website](https://www.railstotrails.org/COVID19/#trailcount)

## Python Environment Setup and Management
**Install** conda environment:
```sh
$ conda env create -f railstotrails.yml
```
**Update** the environment with new packages/versions:
1. modify railstotrails.yml
2. run:
```sh
$ conda env update --name railstotrails --file railstotrails.yml --prune
```
`prune` uninstalls dependencies which were removed from railstotrails.yml

**Use** environment:
before working on the project always make sure you have the environment activated:
```sh
$ conda activate railstotrails
```

**Check the version** of a specific package (e.g. `html5lib`) in the environment:
```sh
$ conda list html5lib
```

**Export** an environment file across platforms:
Include only the packages that were specifically installed. Dependencies will be resolved upon installation
```sh
$ conda env export --from-history > sample.yml
```

**List** all installed environments:
From the base environment run
```sh
$ conda info --envs
```

**Remove** environment:
```sh
$ conda env remove -n sample
```

## Additional Information
See "About Readmes" on Github
https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes
