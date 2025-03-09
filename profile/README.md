# MuNixCPR
**(noun)** :
1. _The act of attempting to revive a system that is neither dead nor dying. with terrariums[^1]_
1. _A collection of containerization alternatives in the same sense that a collection of jars with airholes are acceptable alternatives to say, hermetically sealed vaults._


> Seven ways to go through school  
> Either you're noticed or left out  
> Seven ways to get ahead  
> Seven ways to ...  
>
> ...  
> Sit me down,  
> Shut me up  
> ...  
>
> Six things without fail you must do  
> [Before spinning up the dev server ;)]  
>
> Though the server is never the same  
> You *will* try again  
>
> -Julian Casablancas (+Heraclitus +mfw)

## What?
*Regarding [MusicCPR](musiccpr.org) onboarding:* for some students, codespaces/docker containerization was unacceptably slow. I worked to help document the process for students who may be inexperienced on the commandline/with unix environments, but with technologies like Nix becoming more commonplace I figured this little side quest could act as a great excuse for me to familiarize myself with not only Nix, but a myriad other tools.

I'm not sure of the status of [tgm's](gtihub.com/hcientist) codespaces investigation, so this all may be moot...
*but again,* it's to get better with these tools and to feel more comfortable configuring and maintaining environments,   
since, *par les temps qui courent*, all my dev is done over ssh to various boxes distributed globally (I'm not even kidding, for the occasional sophomore who hears this and thinks I'm like kidding? for some reason?).


## Exploring:

1. `MuNixAnsible`
    - Ansible is the defacto standard for automation, provisioning, etc., and I need to get better at it.
    - This should entail playbooks for isos maybe; I'm still on the fence about this one.
1. `MuNixArchiso`
    - lightweight custom arch linux iso meant to be run by student in VM.
1. `MuNixPureFlake`
    - Pure nix approach with flakes is potentially most lightweight while still highly reproducible
1. `MuNixPureShell`
    - For a very fast ad hoc dev environment without too much anxiety about host machine
1. `MuNixFlakeContainer`
    - offers additional isolation when compared to pure nix approaches
    - uses `nix-devcontainer`, which in turn makes use of a bare debian image, assumedly lighter-weight than the image used for codespaces expl, but need to confirm.
    - allows easy spinup & development in a VSCode codespace (!!!)
1. `MuNixSystem`
    - This approach is the oddest, but one I am most excited for, if it is given the go ahead and students take up the offer. It entails configuring a system and making said system available for students to create user accounts and do MusicCPR development remotely.
    - This is to give me actual hands on practice administering/setting up:
        1. a box with actual users
        1. ephemeral storage
        1. Resource monitoring and allocation

#### *Mutantur, manent. non bis idem; sapent sat. seulement, tu souhaites*


[^1]: See also: *Containers*
