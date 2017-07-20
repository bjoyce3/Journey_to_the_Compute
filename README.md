# Journey to the Compute
Two day hands-on workshop for Docker, Singularity, and leveraging HPC and cloud resources.

# Journey to the Compute, Episode 1: Containers to Quiet the Dependency Hells

## Containers and why they're useful

## Where can you get containers
1. Pre-built containers
  * [Docker Hub](https://hub.docker.com/)
  * [Biocontainers](http://biocontainers.pro/)
2. Building your own containers
3. Limitations
  * Docker for Windows 
  * No Singularity
  	- Can convert Docker containers into Singularity containers on Windows
  	- [Docker2Singularity](https://hub.docker.com/r/tacc/docker2singularity/)

# Journey to the Compute, Episode 2: XSEDE Bound and Down, Dockered Up and Truckin'

## Bingo list of resources
- HPC
	1. National 
		a. [CyVerse Discovery Environment](de.cyverse.org)
		b. XSEDEComet (GPU!)		
	2. Local
		a. University of Arizona HPC (UA affiliates only)
- Cloud services
	1. Academic
		a. [CyVerse Atmosphere](atmo.cyverse.org)
		b. [Jetstream](https://use.jetstream-cloud.org/)
	2. Industry
		a. Amazon Web Services
		b. Google Cloud Services

---

# Peer-reviewed Publications
Kurtzer GM, Sochat V, Bauer MW (2017) Singularity: Scientific containers for mobility of compute. PLOS ONE 12(5): e0177459. https://doi.org/10.1371/journal.pone.0177459
Upendra Kumar Devisetty, Kathleen Kennedy, Paul Sarando, Nirav Merchant, Eric Lyons. Bringing your tools to CyVerse Discovery Environment using Docker. DOI: http://dx.doi.org/10.12688/f1000research.8935.3

# Tools and Cyberinfrastructure Documentation
[Bringing Analysis Apps to the CyVerse Discovery Environment](https://pods.iplantcollaborative.org/wiki/display/DEmanual/Dockerizing+Your+Tools+for+the+CyVerse+Discovery+Environment)
[Docker2Singularity](https://hub.docker.com/r/tacc/docker2singularity/) support moving Docker containers into Singularity containers in Windows and Mac.

----
# Useful Links
* [Clouds, Clusters, and Containers workshop](https://github.com/johnfonner/AKES2016)
* [Docker with CyVerse webinar and demo](https://github.com/upendrak/docker-webinar-1/blob/master/demo-1.md)

----

# Acknowledgements
This work was adapted from previous work done by Upendra Devisetty (@upendrak), Tyson Swetnam (@tyson-swetnam), and John Fonner (@johnfonner).

---

# Workshop Events
* [Meetup Day 1 June 2017](https://www.meetup.com/Tucson-Data-Science-Meetup/events/239386940/) 
  In case you're not familiar, shipping containers are responsible for moving most of the goods that you consume in your everyday. Without them, we'd be in trouble. It's also interesting to note they they transit from giant ships, to railways, to semi-trucks, and fit into the back loading dock of your local grocery because they are a uniform size. This same concept has been applied to computation. We'll start out by discussing the container technologies Docker and Singularity. We'll go over some use cases and highlight what containers won't do. Docker is NOT perfect. Then we'll break into hands-on setting up containers, finding pre-built containers, and running containers. 

  Bring a laptop! Or if you're really really strong you can bring a desktop. Ultimately, we'll move a Docker container into a Singularity container to set up for the July meet up.
  Attendees: 35

* [Meetup Day 2 July 2017](https://www.meetup.com/Tucson-Data-Science-Meetup/events/239386968/)
  We're gonna do what they say can't be done! 'Scaling up' compute is a tricky thing. Not only are there hardware issues to consider, but there are many secret sauce code streamlining fixes to deploy it on bigger compute. We're going to focus on how to move out to bigger compute, because that's generally the first step. Come join us! 
  Attendees: 31
