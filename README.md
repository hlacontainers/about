# About the HLA containers project

The project contains the docker files and build instructions for the containerization of several [HLA Run-Time Infrastructure](https://en.wikipedia.org/wiki/High-level_architecture) products:

- Portico RTI: Portico is an open source and partial HLA RTI implementation, and can be found on GitHub at https://github.com/openlvc/portico.
- VTMaK RTI: The VTMaK RTI is a commercial and fully compliant HLA-RTI implementation. See https://www.mak.com.
- Pitch RTI: The Pitch RTI is a commercial and fully compliant HLA-RTI implementation. See http://pitchtechnologies.com.

The repositories under this project do not contain any VTMaK or Pitch proprietary product files. The build instructions in the various repositories indicate how to obtain the product files and how to build the Docker container images.

## Docker Hub

Several of the images are automatically built and made available on the Docker Hub under the `hlacontainers` namespace, [at this link](https://hub.docker.com/u/hlacontainers):

````
https://hub.docker.com/u/hlacontainers
````

For the commercial RTIs only skeleton images are built that do not include any vendor proprietary files. These skeleton images are not executable and require the vendor proprietary files to be mounted into the container in order to create a functioning product. Instructions can be found in the respective repositories. Only for the Portico RTI a complete functioning Docker image is built that includes all the required files.

A complete functioning container image for the commercial RTIs can only be built and used when the required products are in place and the related license conditions are met.

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

