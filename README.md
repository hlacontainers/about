# About the HLA containers project

The project contains the docker files and build instructions for the containerization of several [HLA Run-Time Infrastructure](https://en.wikipedia.org/wiki/High-level_architecture) products:

- Portico RTI: Portico is an open source and partial HLA RTI implementation, and can be found on GitHub at https://github.com/openlvc/portico.
- VTMaK RTI: The VTMaK RTI is a commercial and fully compliant HLA-RTI implementation. See https://www.mak.com.
- Pitch RTI: The Pitch RTI is a commercial and fully compliant HLA-RTI implementation. See http://pitchtechnologies.com.

The repositories under this project do not contain any VTMaK or Pitch proprietary product files due to the license restictions of these products. The build instructions in the various repositories indicate how to obtain the VTMaK and Pitch product files and how to build the Docker container images for these RTIs in your own Docker build environment. For the Portico RTI the product files are included in the repository.

## Docker Hub

Several of the images are automatically built and made available on the Docker Hub under the `hlacontainers` namespace, [at this link](https://hub.docker.com/u/hlacontainers):

````
https://hub.docker.com/u/hlacontainers
````

For the Pitch and VTMaK RTIs only skeleton images are built that do not include any vendor proprietary files. These skeleton images are not executable and require the vendor proprietary files to be mounted into the container in order to create a functioning product. Instructions can be found in the respective repositories. Only for the Portico RTI complete functioning Docker images are built and published on the Docker Hub.

Only when Pitch or VTMaK change their product license scheme we may be able to inlude their product files in this repository and offer ready to run functioning container images on the Docker Hub like we already do for Portico. Until that time the user can only create ready to run images from his own Docker build environment.

## Getting started

Pick your RTI of choice and navigate to the respective repositories to build the images. An example application is included in the start-me repository, including several Docker composition files.
 
Caveats:

- For the functioning of each RTI we refer to the user manual of the respective RTI.
- Knowledge about Docker and container networking is required!

## Change Log

| Version | Date       | Description                                                  |
| ------- | ---------- | ------------------------------------------------------------ |
| 1.0     | 3 Feb 2020 | Donation from [TNO](https://www.tno.nl/nl) to the community: repositories with Dockerfiles and build instructions for Portico, Pitch and VTMaK RTIs. Initial implementations date back to 2015. |
|         |            |                                                              |

## References

Obviously we hope that the following list evolves!

- IVCTool project at https://github.com/IVCTool

