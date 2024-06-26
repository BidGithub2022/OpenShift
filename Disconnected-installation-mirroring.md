## About disconnected installation mirroring
You can use a mirror registry to ensure that your clusters only use container images that satisfy your organizational controls on external content. Before you install a cluster on infrastructure that you provision in a restricted network, you must mirror the required container images into that environment. To mirror container images, you must have a registry for mirroring.

---

## Creating a mirror registry
If you already have a container image registry, such as Red Hat Quay, you can use it as your mirror registry. If you do not already have a registry, you can create a mirror registry using the mirror registry for Red Hat OpenShift.

You must have a container image registry that supports Docker v2-2(see the reference link below) in the location that will host the OpenShift Container Platform cluster, such as one of the following registries:
- Red Hat Quay
- JFrog Artifactory
- Sonatype Nexus Repository
- Harbor

--- 

## Mirroring images for a disconnected installation
You can use one of the following procedures to mirror your OpenShift Container Platform image repository to your mirror registry:

- Mirroring images for a disconnected installation

- Mirroring images for a disconnected installation using the oc-mirror plugin

---

## Below steps are for  Mirroring images for a disconnected installation using the oc-mirror plugin:
The following steps outline the high-level workflow on how to use the oc-mirror plugin to mirror images to a mirror registry:

1. Create an image set configuration file.

2. Mirror the image set to the mirror registry by using one of the following methods:

    - Mirror an image set directly to the mirror registry.

    - Mirror an image set to disk, transfer the image set to the target environment, then upload the image set to the target mirror registry.

3. Configure your cluster to use the resources generated by the oc-mirror plugin.

4. Repeat these steps to update your mirror registry as necessary.

---

The following steps outline the Detail workflow on how to use the oc-mirror plugin to mirror images to a mirror registry:

[Preparing mirror host: installing oc mirror CLI and configure credentials](https://docs.openshift.com/container-platform/4.15/installing/disconnected_install/installing-mirroring-disconnected.html#mirroring-preparing-your-hosts)

1.  Image set configuration file defines which OpenShift Container Platform releases, Operators, and other images to mirror, along with other configuration settings for the oc-mirror plugin:
   
    [Creating the image set configuration](https://docs.openshift.com/container-platform/4.15/installing/disconnected_install/installing-mirroring-disconnected.html#oc-mirror-creating-image-set-config_installing-mirroring-disconnected)

2.  You can choose between 2 options here while mirroring an image set to image registry:
    
    [Mirroring an image set in a partially disconnected environment](https://docs.openshift.com/container-platform/4.15/installing/disconnected_install/installing-mirroring-disconnected.html#mirroring-image-set-partial)
    
    [Mirroring an image set in a fully disconnected environment](https://docs.openshift.com/container-platform/4.15/installing/disconnected_install/installing-mirroring-disconnected.html#mirroring-image-set-full)

3. Configure your cluster to use the resources generated by the oc-mirror plugin:
   
   [Configuring your cluster to use the resources generated by oc-mirror](https://docs.openshift.com/container-platform/4.15/installing/disconnected_install/installing-mirroring-disconnected.html#oc-mirror-updating-cluster-manifests_installing-mirroring-disconnected)

4. Repeat these steps to update your mirror registry as necessary:
   
   [Keeping mirror registry content up to date](https://docs.openshift.com/container-platform/4.15/installing/disconnected_install/installing-mirroring-disconnected.html#updating-mirror-registry-content)

---

**Reference links:**

[Disconnected installation mirroring](https://docs.openshift.com/container-platform/4.15/installing/disconnected_install/index.html)

[Docker v2-2](https://docs.docker.com/registry/)

[OpenShift Downloads](https://console.redhat.com/openshift/downloads)
