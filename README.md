```md
 __      __       .__                               
/  \    /  \ ____ |  |   ____  ____   _____   ____  
\   \/\/   // __ \|  | _/ ___\/  _ \ /     \_/ __ \ 
 \        /\  ___/|  |_\  \__(  <_> )  Y Y  \  ___/ 
  \__/\  /  \___  >____/\___  >____/|__|_|  /\___  >
       \/       \/          \/            \/     \/ 
```
------

## ASCII Art Options

[Lettering](https://patorjk.com/software/taag/#p=display&f=Graffiti&t=Type%20Something%20)

When adding ASCII to our pages, I recommend putting it in a [*codeblock*](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks) so it is formatted correctly, ex:

````
```md
this is a code block 
```
````

Art here](https://www.asciiart.eu/), [here](https://asciiart.website/) and [here](https://steamcommunity.com/groups/asciiartamalgamation) -- just search!

## (Optional) Commit Message Formatting

https://www.conventionalcommits.org/en/v1.0.0/

And an optional template:

```bash
git config --local commit.template .gitmessage
```

## (Optional) Hooks

```bash
git config --local core.hooksPath .hooks

# you might need (but git should track this):
chmod +x .hooks/commit-message
```

## Github Workflows

`deploy`

Lint + build + deploy

`pr-validate`

Lint + build

# Labs

### Setup:

- create issues for each team member to add a _Letter_ page, ex: `a.md`
- set up branching workflow (`main` & `dev`)
- set up branch protection, requiring 1 or 2 approvals and PR to `dev

### Exercise 1:

- EVERYONE gets their page up as a PR
  - you can use `#issue-id` to tie it to an issue, ex: `closes #10`

Consider giving it an ASCII art [title](https://patorjk.com/software/taag/#p=display&f=Isometric1&t=Letter%20A):

ex:

`a.md`
```md
      ___       ___           ___           ___           ___           ___                    ___     
     /\__\     /\  \         /\  \         /\  \         /\  \         /\  \                  /\  \    
    /:/  /    /::\  \        \:\  \        \:\  \       /::\  \       /::\  \                /::\  \   
   /:/  /    /:/\:\  \        \:\  \        \:\  \     /:/\:\  \     /:/\:\  \              /:/\:\  \  
  /:/  /    /::\~\:\  \       /::\  \       /::\  \   /::\~\:\  \   /::\~\:\  \            /::\~\:\  \ 
 /:/__/    /:/\:\ \:\__\     /:/\:\__\     /:/\:\__\ /:/\:\ \:\__\ /:/\:\ \:\__\          /:/\:\ \:\__\
 \:\  \    \:\~\:\ \/__/    /:/  \/__/    /:/  \/__/ \:\~\:\ \/__/ \/_|::\/:/  /          \/__\:\/:/  /
  \:\  \    \:\ \:\__\     /:/  /        /:/  /       \:\ \:\__\      |:|::/  /                \::/  / 
   \:\  \    \:\ \/__/     \/__/         \/__/         \:\ \/__/      |:|\/__/                 /:/  /  
    \:\__\    \:\__\                                    \:\__\        |:|  |                  /:/  /   
     \/__/     \/__/                                     \/__/         \|__|                  \/__/    
```

- EVERYONE review one anothers PRs.
- EVERYONE merge YOUR OWN PR once it gets enough approvals.

### Exercise 2:

- INSTRUCTOR WILL create a `release-` branch to `main`
- INSTRUCTOR WILL __release it__
- INSTRUCTOR WILL `tag` it, ex: `v1.0`
- INSTRUCTOR WILL __merge back into `dev`__

### Exercise 3:

- EVERYONE WILL pick any letter; create a "word" page that links off that letter letter page.
- EVERYONE WILL push and open a PR
- **DO NOT MERGE** yet...

ex:

`a.md`
```md
      ___       ___           ___           ___           ___           ___                    ___     
     /\__\     /\  \         /\  \         /\  \         /\  \         /\  \                  /\  \    
    /:/  /    /::\  \        \:\  \        \:\  \       /::\  \       /::\  \                /::\  \   
   /:/  /    /:/\:\  \        \:\  \        \:\  \     /:/\:\  \     /:/\:\  \              /:/\:\  \  
  /:/  /    /::\~\:\  \       /::\  \       /::\  \   /::\~\:\  \   /::\~\:\  \            /::\~\:\  \ 
 /:/__/    /:/\:\ \:\__\     /:/\:\__\     /:/\:\__\ /:/\:\ \:\__\ /:/\:\ \:\__\          /:/\:\ \:\__\
 \:\  \    \:\~\:\ \/__/    /:/  \/__/    /:/  \/__/ \:\~\:\ \/__/ \/_|::\/:/  /          \/__\:\/:/  /
  \:\  \    \:\ \:\__\     /:/  /        /:/  /       \:\ \:\__\      |:|::/  /                \::/  / 
   \:\  \    \:\ \/__/     \/__/         \/__/         \:\ \/__/      |:|\/__/                 /:/  /  
    \:\__\    \:\__\                                    \:\__\        |:|  |                  /:/  /   
     \/__/     \/__/                                     \/__/         \|__|                  \/__/    

* [Aardvark](./aardvark.md)
```

`aardvark.md`
```md
       _.---._    /\\
    ./'       "--`\//
  ./              o \          .-----.
 /./\  )______   \__ \        ( hi!  )
./  / /\ \   | \ \  \ \       /`-----'
   / /  \ \  | |\ \  \7--- ooo ooo ooo ooo ooo ooo

```

### Exercise 4

- INSTRUCTOR will introduce changes (reorg to `letters/`) in `dev`
- INSTRUCTOR will then introduce a `hotfix` and get it released
  - Where does a hotfix start from?
- EVERYONE will need to get up to date with that `hotfix` 
- EVERYONE push their updates, address conflicts as needed
- INSTRUCTOR WILL merge (if we have time and want to try other things)

### Optional

- groups work on feature branches together.
- what happens when I squash someone's work?