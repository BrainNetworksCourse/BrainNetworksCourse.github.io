### Additional resources

The following resources are useful as background and/or for a further dive into the topics discussed in this course:

- [Networks: An Introduction, by Mark Newman](https://www.amazon.com/Networks-Introduction-Mark-Newman/dp/0199206651) - an outstanding introduction to the ideas behind graph theory and network analysis
- [Networks of the Brain, by Olaf Sporns](https://www.amazon.com/Networks-Brain-Press-Olaf-Sporns-ebook/dp/B005AT9ZOI/ref=sr_1_1?s=books&ie=UTF8&qid=1535385228&sr=1-1&keywords=sporns) - excellent overview of network neuroscience
- [Fundamentals of Brain Network Analysis, by Fornito, Zalesky, & Bullmore](https://www.amazon.com/Fundamentals-Brain-Network-Analysis-Fornito-ebook/dp/B01CRIU886/ref=sr_1_1?s=books&ie=UTF8&qid=1535384994&sr=1-1&keywords=fornito) - a deep dive into the concepts and methods behind brain network modeling

### Sources for open data

Here are a number of possible sources of open brain network data for the project:

- [Human Connectome Project](https://db.humanconnectome.org/) - massive human connectomics dataset (requires registration)
- [Allen Institute Mouse Brain Connectivity Atlas](http://connectivity.brain-map.org/)
- [CoCoMac macaque connectivity data](http://cocomac.g-node.org/main/index.php)
- [USC Multimodal Connectivity Database](http://umcd.humanconnectomeproject.org/)
- [StudyForrest](http://studyforrest.org/) - a large amount of data collected on humans watching Forrest Gump
- [WormAtlas](http://www.wormatlas.org/) - a database for C. Elegans data including connectvity
- [Core Nets](http://core-nets.org) - substantial database of macaque tract tracing data
- [Preprocessed Connectomes Project](http://preprocessed-connectomes-project.org/) - preprocessed human fMRI data
- [NeuroTycho](http://neurotycho.org/) - electrophysiological data

There are also two neuroscience-specific portals that you can use to search for relevant data:

- [SciCrunch](https://scicrunch.org) - this is a search engine that you can use to find datasets of interest across many different resources
- [NITRC](https://www.nitrc.org/) - another portal that provides the ability to search across many different data sets and databases

### Environment setup for Brain Networks course

For this course we will use a virtual machine that will allow everyone to have
an identical environment regardless of their operating system. You are of course
free to install all of the dependencies on your own system, but they are not
guaranteed to work (and some will certainly not work if you are on Windows).

To use the VM, first set up the following software on your computer:

- Install [VirtualBox](https://www.virtualbox.org/)

- Install [Vagrant](https://www.vagrantup.com/)

- Install [git](https://git-scm.com/) if you don't already have it.

### Creating your own fork of the class repository.

Go to github.com and log into your account.  Then go to the class repository:

[https://github.com/BrainNetworksCourse/brain-networks-course](https://github.com/BrainNetworksCourse/brain-networks-course)

Click the Fork button to create a fork of the repository in your github account.  This will allow you to make changes and submit them for inclusion in the main repository, and is the standard approach used for collaborative software development on github.


Clone the repository onto your computer:

```git clone https://github.com/<your github username>/brain-networks-course.git```

inserting your github username in the appropriate place in the URL.

### Setting up vagrant

Go into the repo directory and open the file called "vagrant_setup.rb" in your favorite text editor.  Change the following line:

```GITHUB_USERNAME = "poldrack"```

by replacing poldrack with your own github username.  Be sure to save the file and then commit it to your fork:

```
git add vagrant_setup.rb
git commit -m"changing github username"
git push origin master
```

### Provision the virtual machine

Run the following command to provision the
virtual machine (this will take a little while the first time you do it, and involves lots of downloading so be sure to do it from a good network):

  ```vagrant up```

Once the installation is done, then restart the virtual machine; to do this, go to the VirtualBox window for the VM (which should just show a login window), close the VM window, and choose "Power off the machine".  Then run ```vagrant up``` again to restart it.  At this point, a GUI window should appear for the VM, which we will use for our class exercises.

## Updating the VM

On occasion we will update the VM with new packages.  To pull the latest changes into your fork, you will first need to add the main repository as a remote to your repo:

```
git remote add upstream https://github.com/BrainNetworksCourse/brain-networks-course.git
```

After doing this once, you can then use the following command within the repo directory to pull the latest changes:

```
git pull upstream master
```

You may need to commit any changes you have made to other files in your repo, or use ```git checkout <filename>``` to pull a clean version if you don't need to keep the changes.

Once you have done this it should pull down the new Vagrantfile, and you can then run ```vagrant provision``` in the main repo directory which will rerun the provisioning and install any new software.  

### Some tips for using the VM

- I find the default screensaver to use up a lot of processing power, so I generally change it to a blank screen (under Preferences->Screensaver).
- You can add an ssh key for your VM so that you won't have to enter your github credentials each time you push or pull.  See [here](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/) for info on how to do this.  
