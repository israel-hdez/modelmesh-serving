---
name: Upstream sync
about: Outlines the process to synchonize ODH fork with upstream repositories
title: "[MM] Synchronization with upstream repositories"
labels: ''
assignees: ''

---

* Export Environmental Variables and create pr_template.sh file
* Sync modelmesh repository(main branch)
* Sync modelmesh-runtime-adapter repository(main branch)
* Sync rest-proxy repository (main branch)
* Sync text-generation-inference repository(main branch)
* Sync caikit repository(main branch)
* Sync caikit-nlp repository(main branch)
* Sync caikit-tgis-backend repository(main branch)
* Sync modelmesh-serving repository(main branch)
* Sync kserve repository(master branch)
* Upgrade odh-model-controller to use kserve v0.11.0
* Create a new release branch from updated main branch
* Update odh-manifest (fast image)
* Create modelmesh-serving PR to test OpenShift CI
    * Updating ModelMesh to v0.11.0 (Step 1) openshift/release#43219
    * Updating ModelMesh to v0.11.0 (Step 2) openshift/release#43096
* Update Dockerfile.develop.ci/go.sum.develop/go.mod.develop repository for openshift-ci
* Create PR for each repository main branch
~~* Create a new release branch when upstream release a new version~~
* Update AutoMerger mapping for the created release branch
