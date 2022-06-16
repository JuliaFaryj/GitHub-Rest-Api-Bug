# GitHub-Rest-Api-Bug

Found github rest api bug in get repository (https://docs.github.com/en/rest/repos/repos#get-a-repository).

## How to replicate the bug
1. Make sure repo A and repo B do NOT exist
2. Create repo A
3. Get repo A - returns info about repo A
4. Update repo A and change name to B - renames A to B
5. Get repo B - returns info about repo B
6. Get repo A - returns info about repo B (error)

## How to run code
To run code you need to have Python installed with followings modules
1. requests
2. pytest

