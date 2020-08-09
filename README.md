![Bash CI](https://github.com/pforret/bashew/workflows/Bash%20CI/badge.svg) 
![Shellcheck CI](https://github.com/pforret/bashew/workflows/Shellcheck%20CI/badge.svg)
![version](https://img.shields.io/github/v/release/pforret/bashew?include_prereleases)
![activity](https://img.shields.io/github/commit-activity/y/pforret/bashew)
![license](https://img.shields.io/github/license/pforret/bashew)
![repo size](https://img.shields.io/github/repo-size/pforret/bashew)

# bashew
bash script creator - from small stand-alone script to complex projects with CI/CD and testing

## Installation

* manually

        git clone https://github.com/pforret/bashew.git
        ln -s bashew/bashew.sh /usr/local/bin
    
* or with basher    

        basher install pforret/bashew
        
## Usage

### 1. create new bash script (without repo)

        bashew.sh script
    
### 2. create new bash project folder (with README.md ...)

        bashew.sh project

### 3. create a bash script repo, with CI/CD, with README, with tests, with versioning ... 

* on [github.com/pforret/bashew](https://github.com/pforret/bashew), click on '**Use this template**'
* then clone your new repo

        git clone https://github.com/<you>/<your repo>.git
        cd <your repo>
        ./bashew.sh init             # will ask for details and iniialise/clean up the repo

#### and then, if you have [semver.sh](https://github.com/pforret/semver):
        semver.sh push          # will commit and push new code
        semver.sh new patch     # will set new version to 0.0.1


----

  to be tested
  
### 4. git clone into new repo

        git clone --depth=1 https://github.com/pforret/bashew.git <newname>
        cd <newname>
        ./bashew.sh init             # will ask for details and iniialise/clean up the repo
