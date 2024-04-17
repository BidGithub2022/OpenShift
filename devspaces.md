## Find the dev spaces operator

![Screenshot 2024-04-17 at 3 02 07 PM](https://github.com/BidGithub2022/OpenShift/assets/113651761/6ad8a434-2db4-4f9f-ae56-49b5f4fa70b4)

## Install the dev spaces operator

![Screenshot 2024-04-17 at 3 03 34 PM](https://github.com/BidGithub2022/OpenShift/assets/113651761/72b7dad3-183e-451c-8e3b-fc9597e35211)

![Screenshot 2024-04-17 at 3 04 33 PM](https://github.com/BidGithub2022/OpenShift/assets/113651761/54da1101-f96d-444f-b31c-a8a4e551528c)

## Create CheCluster custom resource

The CheCluster custom resource allows defining and managing Red Hat OpenShift Dev Spaces server installation. Based on these settings, the Operator automatically creates and maintains several ConfigMaps: che, plugin-registry, devfile-registry that will contain the appropriate environment variables of the various components of the installation. These generated ConfigMaps must NOT be updated manually.

![Screenshot 2024-04-17 at 3 08 08 PM](https://github.com/BidGithub2022/OpenShift/assets/113651761/b52cc9cd-937c-49c9-92c9-eb2d8fa68d27)

![Screenshot 2024-04-17 at 3 10 11 PM](https://github.com/BidGithub2022/OpenShift/assets/113651761/986e9a31-d963-4f83-8171-794c067e260a)

You can configure below based on your requirements. 

![Screenshot 2024-04-17 at 3 23 15 PM](https://github.com/BidGithub2022/OpenShift/assets/113651761/fc124193-c511-4f92-9b6e-03e8d564d38a)


Once the CheCluster Available, and you see a URL to Red Hat OpenShift Dev Spaces, access the dev spaces URL. You will have to authenticate the access.

![Screenshot 2024-04-17 at 3 26 31 PM](https://github.com/BidGithub2022/OpenShift/assets/113651761/d472d459-759d-4314-9e7d-b83f9d64138c)


Dev Spaces page would look like this. Start creating your workspace from GIT or samples.

![Screenshot 2024-04-17 at 3 27 44 PM](https://github.com/BidGithub2022/OpenShift/assets/113651761/4ca0057d-f93d-43da-ae2a-e3312d8a7ed4)


